<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h2 Enumeración de activos

    .row.justify-content-center.align-items-center.mb-5.mt-4           
      .col-lg-10 
        .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="flip-down")
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema3/img01.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p.m-0 El inventario de activos o llamada enumeración, es una actividad que se debe de realizar en primera instancia para poder llevar a cabo un proceso de gestión de la seguridad de un sistema; es de vital importancia conocer sus recursos físicos, infraestructura, personas, <em>software</em>, entre otros, que son parte de la cadena de valor de la organización y estos, a su vez, sean protegidos para evitar ataques de ciberdelincuentes. Las amenazas a las cuales se encuentran expuestos, cada vez, son mayores y de gran tecnología.
              br  

    .bg_fondo1_t3
      Separador

      #t_3_1.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
        h2 3.1.	Conceptos y generalidades

      p.m-0.mb-4(data-aos="fade-right") La enumeración se define como el proceso de extracción de nombres de usuario, nombres de máquinas, recursos de red, recursos compartidos y servicios de un sistema. En esta fase, el atacante crea una conexión activa con el sistema y realiza consultas dirigidas para obtener más información sobre el objetivo. 

      p.m-0.mb-4(data-aos="fade-right") La información reunida se utiliza para identificar las vulnerabilidades o los puntos débiles de la seguridad del sistema y trata de explotarlos en la fase de obtención del sistema. 

      p.m-0.mb-4(data-aos="fade-right") Estos son los tipos de información enumerados por los intrusos:

      .row.justify-content-center
        .col-12.col-md-8
          figure
            img(data-aos="fade-up-right")(src='@/assets/curso/tema3/img02.svg')
      
      Separador

    #t_3_2.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
        h2 3.2.	Técnicas de enumeración
    
    p.m-0.mb-4 Existen muchas formas de recopilar datos, como los usuarios de la red, las tablas de enrutamiento y la información del protocolo simple de gestión de redes (SNMP).

    p.m-0.mb-4 A continuación, se analizan las posibles formas en que un atacante podría enumerar una red objetivo:

    .tarjeta-color.bg_color6.p-5.mb-5  
      SlyderA.mb-5(:datos="datosSlyder")
        .row.justifiy-content-evenly(data-aos="fade-right")
          .col-md-5
            h5.mb-4 Extraer los nombres de usurario que utilizan identificadores de correo electrónico.
            p.m-0.mb-4 Generalmente, la ID de correo electrónico contiene dos partes: nombre de usuario y nombre de dominio. La estructura de la dirección de correo electrónico es <b>"nombredeusuario@nombrededominio"</b>.
            p.m-0 Ejemplo: <b>xyz@live.com</b> 
            | <b>xyz</b>, carácter que precede al símbolo “@”, es el nombre de usuario.
            p.m-0 <b>live.com</b>, carácter que sucede al símbolo “@” es el nombre de dominio.
          .col-md-7(data-aos="fade-left")
            figure
              img(src='@/assets/curso/tema3/img03.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.mb-4 Extraer los nombres de usuario utilizando SNMP.
            p.m-0.mb-4.mb-md-0 Mediante el uso de las API de SNMP, los atacantes pueden adivinar las cadenas a través de las cuales pueden extraer el nombre de usuario requerido.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/img04.png', alt='Texto que describa la imagen')
        .row.justifiy-content-around
          .col-md-5
            h5.mb-4 Extraer información con las contraseñas predeterminadas.
            p.m-0.mb-4.mb-md-0 Hay muchos recursos en línea que publican muchas contraseñas predeterminadas asignadas por el fabricante para sus productos. A menudo, los usuarios olvidan cambiar las contraseñas predeterminadas que ayudan a un atacante a enumerar sus datos fácilmente.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/img05.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.m-0 Fuerza bruta. 
            h5.m-0.mb-4 Directorio activo. 
            p.m-0.mb-4.mb-md-0 El directorio activo de Microsoft es susceptible a una debilidad de enumeración de nombres de usuario en el momento de la validación de entrada proporcionada por el usuario. Esto es consecuencia de un error de diseño en la aplicación. El atacante se beneficia de ello y explota la debilidad para enumerar nombres de usuario válidos.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/img06.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-4
            h5.mb-4 Extracto de los grupos de usuarios de las ventanas.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/img07.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.mb-4 Extraer información mediante DNS zona de transferencia.
            p.m-0.mb-4.mb-md-0 Un atacante puede obtener información topológica valiosa sobre la red interna del objetivo utilizando la transferencia de zona DNS.
          .col-md-7
            figure
              img(src='@/assets/curso/tema3/img08.png', alt='Texto que describa la imagen')

    Separador

    #t_3_3.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
        h2 3.3	Contramedidas

    p.m-0.mb-4 Durante la enumeración se recoge, sistemáticamente, información y se identifican los sistemas individuales, los pentesters examinan los sistemas en su totalidad; esto permite evaluar las debilidades de seguridad que no necesariamente se derivan de un problema técnico. 
  
    .row.justify-content-center.align-items-center.mb-5.mt-4           
      .col-lg-10 
        .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="flip-down")
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema3/img09.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p.m-0 Una protección con contraseña, técnicamente segura, puede, por ejemplo, resultar inútil si los atacantes pueden ver la entrada de la contraseña de un usuario a través de una ventana; durante la enumeración, los pentesters recogen información sobre posibles debilidades que se verifican o refutan durante la fase de explotación.
              br  

    p.margin_left1 <em>Pentesting</em>: de enumeración:

    .row.justify-content-center(data-aos="fade-right")
      .col-12.col-md-6
        ul
          li 
            i.fas.fa-check-circle
            |  <b>Encontrar el rango de red</b>
            p.m-0 (utilizar herramientas como Whols Lookup y Graphical DNS Zones).
          li
            i.fas.fa-check-circle
            |  <b>Calcular la máscara de subred</b>
            p.m-0 (utilizar herramientas como Subnet Mask Calculator).
          li 
            i.fas.fa-check-circle
            |  <b>Realizar descubrimiento</b> 
            p.m-0 (utilizar herramientas como Nmap (nmap sP)).
          li 
            i.fas.fa-check-circle
            |  <b>Realizar enumeración NetBIOS.</b>
          li 
            i.fas.fa-check-circle
            |  <b>Realizar enumeración DNS</b> 
            p.m-0 (utilizar herramientas como nslookup y The men y Mice Suite).
          li 
            i.fas.fa-check-circle
            |  <b>Realizar análisis de puertos</b> 
            p.m-0 (utilizar herramientas como Nmap (mmap sS)).
          li 
            i.fas.fa-check-circle
            |  <b>Utilizar herramientas como SuperScan, NetBIOS Enumerator y PsTools suite.</b>
      .col-12.col-md-4(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema3/img10.png')


    
            
</template>

<script>
export default {
  name: 'Tema3',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
