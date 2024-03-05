<script lang="ts" setup>
    import { ref } from 'vue';
    const caracteristicas = ref([
        {
            atributo: 'Fácil', 
            descripcion: 'Crea una cuenta, envía tu documentación y comienza a utilizar nucleus en un par de horas'
        },
        {
            atributo: 'Seguro', 
            descripcion: 'Por su tecnología digital nucleus es imposible de hackear o robar'
        },
        {
            atributo: 'Administrable', 
            descripcion: 'Añade o transfiere fondos a tu banco, añade limites o controla tus gastos'
        }
    ])

</script>

<template>

    <main class="nucleus">
        <h2 class="nucleus__heading">¿Qué es?</h2>
        <div class="nucleus__contenedor">
            <div class="nucleus__grid">
                <div class="nucleus__imagen">
                    <img src="../assets/img/app_2.svg" alt="app nucleus">
                </div>

                <div class="listado">
                    <div v-for="(caracteristica, index) in caracteristicas" :key="index" class="listado__elemento">
                        <h2 class="listado__heading">{{ caracteristica.atributo }}</h2>
                        <p class="listado__texto">{{ caracteristica.descripcion }}</p>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped></style>