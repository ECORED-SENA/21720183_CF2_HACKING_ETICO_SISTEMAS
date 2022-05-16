<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5     
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción

    .bg_fondointro
      .row
        .col-12.col-md-8.posit_text
          p.m-0.mb-4 En el mundo digital de hoy, hay una gran cantidad de información al alcance de casi cualquier persona, lo cual se ha convertido en uno de los activos más importantes para las organizaciones. Con el uso de las tecnologías de información y comunicación y su avance tan vertiginoso, aparecen agentes internos y externos que pueden poner en riesgo los sistemas de información, los datos almacenados y hasta la infraestructura tecnológica. Es así como el hacking ético se ha convertido en una herramienta de gestión para la seguridad.
          .tarjeta-color.bg_color1.p-3(data-aos="fade-right")
            p.m-0.text-white Es así, como para comenzar con el estudio de este componente, se invita a explorar el recurso que a continuación se propone. Le deseamos todos los éxitos en esta experiencia de formación:
        .col-12.col-md-4
          figure
            img.posit_1_intro(data-aos="fade-left")(src="@/assets/curso/introduccion/img02.png", alt="Texto que describa la imagen")

      .row.justify-content-center.mt-4
        .col-12.col-md-12.posit_relative    
          figure.mb-5
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/TtKdy3RoBg4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
      

    
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
