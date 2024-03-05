<script lang="ts" setup>
    import { ref } from 'vue'

    const testimoniales = ref([
        {
            texto: 'Excelente app, muy sencillo de manejar y enviar dinero',
            autor: '- Juan De la torre'
        },
        {
            texto: 'La aplicación es increíble, me facilita mucho la vida financiera',
            autor: '- María Rodríguez'
        },
        {
            texto: 'Muy útil para realizar transacciones rápidas y seguras',
            autor: '- Pedro Gómez'
        },
        {
            texto: 'La interfaz es intuitiva, lo que hace que sea fácil de usar',
            autor: '- Ana López'
        },
        {
            texto: '¡Increíble servicio! Nunca había sido tan fácil enviar dinero a mis amigos',
            autor: '- Luis Fernández'
        },
        {
            texto: 'Me encanta la rapidez con la que puedo realizar mis operaciones financieras',
            autor: '- Laura Martínez'
        }
    ])

</script>

<template>

    <section class="testimoniales">
        <div class="testimoniales__contenedor">
            <h2 class="testimoniales__heading">Testimoniales</h2>

            <div class="testimoniales__grid">
                <div v-for="(testimonial, index) in testimoniales" :key="index" class="testimonial">
                    <p class="testimonial__texto">{{ testimonial.texto }}</p>
                    <p class="testimonial__autor">{{ testimonial.autor }}</p>
                </div>
            </div>
        </div>
    </section>


</template>

<style scoped></style>