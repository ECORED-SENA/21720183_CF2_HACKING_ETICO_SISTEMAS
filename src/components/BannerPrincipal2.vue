<template lang="pug">
.banner-principal
  .container.tarjeta.position-relative(
    :style="{'background-image': globalData.fondoBannerPrincipal ? `url(${globalData.fondoBannerPrincipal})` : 'none'}"
  )
    .row.banner-principal__row.position-relative.justify-content-center.align-items-center
      .col-lg-7.col-xxl-6.py-4.py-sm-5.banner-principal__info.ps-5
        .banner-principal__componente
          h1.mb-0(v-html="globalData.componenteFormativo")
        .col-lg-12
          .banner-principal__descripcion
            p.mb-0(v-html="globalData.descripcionCurso")
        .banner-principal__accion
          router-link.boton(:to="{name: iniciarLnk.nombreRuta }")
            span.me-1 Iniciar
            i.fas.fa-angle-right

      .col-lg-5.d-none.d-lg-block.px-0.position-relative.img-p
        img(:src="globalData.imagenBannerPrincipal")
    .imagen_flotante_1: img.img-fluid(src="@/assets/curso/portada/flot1.svg").d-none.d-lg-block
    //-.imagen_flotante_2: img(src="@/assets/curso/portada/flot2.svg").d-none.d-lg-block
    //-.imagen_flotante_3: img(src="@/assets/curso/portada/flot3.svg").d-none.d-lg-block
    //-.imagen_flotante_4: img(src="@/assets/curso/portada/flot4.svg").d-none.d-lg-block
    //-.imagen_flotante_5: img(src="@/assets/curso/portada/cara5.svg").d-none.d-lg-block
    //-.imagen_flotante_6.banner-principal__img: img(src="@/assets/curso/portada/estre5.svg").d-none.d-lg-block
    
  

</template>

<script>
import mixins from '../components/plantillaMixins'
export default {
  name: 'BannerPrincipal',
  mixins: [mixins],
  computed: {
    globalData() {
      return this.$config.global
    },
  },
}
</script>

<style lang="sass">
.img-p
  top: 67px
  right: -4%
  max-width: 100%
  height: auto
.fondo-contenido
  position: absolute
  padding: 0px
  z-index: 2
  height: 100%
  width: 100%
.banner-principal__info
  padding-left: 80px  !important
  z-index: 3


.banner-principal
  p, h1, h2, h3, h4, h5, h6
    color: $color-banner-text
    @media (max-width: $bp-max-xs)
      margin-left: -50px
      width: 290px

  .tarjeta
    background-color: #FFC664
    background-size: cover
    //background-position: center
    height: 507px
    @media (max-width: $bp-max-xs)
      height: 570px

  &__info
    display: flex
    flex-direction: column
    justify-content: center

  &__programa
    display: flex
    align-items: center
    margin-bottom: 20px

  &__componente
    margin-bottom: 20px
    padding-right: 190px
    h1
      line-height: 1.1em

      @media (max-width: $bp-max-xs)
        font-size: 2em
        margin-left: -50px
        width: 258px

  &__descripcion
    margin-bottom: 60px
    padding-right: 71px

  &__accion
    @media (max-width: $bp-max-xs)
      margin-left: -50px
      margin-top: -25px

  &__row
    @if $banner-principal-img-x == 'derecha'
      justify-content: space-between
    @else
      justify-content: space-around
      .banner-principal__img
        padding-right: 1.5rem!important
      @media (min-width: $bp-min-sm)
        .banner-principal__img
          padding-right: 3rem!important

  //&__img
    animation: scale 5s ease-in-out infinite alternate
    @if $banner-principal-img-y == 'arriba'
      align-self: flex-start
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-bottom: 3rem!important
    @else if $banner-principal-img-y == 'abajo'
      align-self: flex-end
      padding-top: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
    @else
      align-self: center
      padding-top: 1.5rem
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
        padding-bottom: 3rem!important

.imagen_flotante
  &_1
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 435px
    top: -1%
    right: 12%
  &_2
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 96px
    top: 63%
    right: 4%
  &_3
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 133px
    bottom: 29%
    right: 19%
  &_4
    animation: scale 3s ease-in-out infinite alternate
    @if $banner-principal-img-y == 'arriba'
      align-self: flex-start
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-bottom: 3rem!important
    @else if $banner-principal-img-y == 'abajo'
      align-self: flex-end
      padding-top: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
    @else
      align-self: center
      padding-top: 1.5rem
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
        padding-bottom: 3rem!important
    position: absolute
    width: 124px
    bottom: 27%
    left: 58%
    z-index: 99
  &_5
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 92px
    top: 44%
    left: 59%
    z-index: 99
  &_6
    //animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 239px
    top: 55%
    right: 2%
    z-index: 99
  &_7
    animation: float1 2.5s ease-in-out infinite alternate
    position: absolute
    width: 50px
    bottom: 10%
    right: 3%
    z-index: 99
  &_8
    filter: blur(1px)

    animation: float1 3s ease-in-out infinite alternate
    position: absolute
    width: 50px
    bottom: 20%
    right: 8%
    z-index: 99

@keyframes float1
  0%
    transform: translateY(20px)

  100%
    transform: translateY(0px)
@keyframes float2
  0%
    transform: translatex(20px)

  100%
    transform: translatex(0px)

@keyframes scale
  0%
    transform: scale(1.1)

  100%
    transform: scale(1)


@media (max-width: $bp-max-md)
  .fondo-contenido
    display: none
  .fondo-contenido2
    background-repeat: no-repeat
    background-size: cover
</style>
