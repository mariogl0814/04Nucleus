<script lang="ts" setup>
    import {ref} from 'vue'

    const descripciones = ref([
        { texto: 'Nucleus es seguro e imposible de clonar'},
        { texto: 'Utiliza tu cara o tu dedo para confirmar un deposito o registrar una cuenta'},
        { texto: 'Paga en un establecimiento con una tarjeta de crédito que se desactiva una vez que has hecho tu compra'},
    ])
</script>

<template>

    <section class="seguridad">
        <div class="seguridad__contenedor">
            <h2 class="seguridad__heading">Nucleus es seguro</h2>
            <div class="seguridad__grid">
                <div class="listado">
                    <div v-for="(descripcion,index) in descripciones" :key="index" class="listado__elemento">
                        <p class="listado__texto">{{descripcion.texto}}</p>
                    </div>
                </div>

                <div class="seguridad__imagen">
                    <img src="../assets/img/seguridad.png" alt="seguridad nucleus">
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped></style>