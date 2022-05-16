<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 Footprinting y reconocimiento

    .bg_imgfondo1_t1
      .row.align-items-center(data-aos="fade-right") 
        .col-12.col-md-7
          p.m-0.mb-2 El <em>footprinting</em> se define como el proceso de creación de un plano o mapa de la red y los sistemas de una organización; igualmente, a la recopilación de información también se le conoce como “<em>footprinting</em>” (huella) de una organización. Este se comienza por determinar el sistema, la aplicación o la ubicación física del objetivo y, una vez que se conoce esta información, se reúne información específica sobre la organización utilizando métodos no intrusivos.
          .cajon.color-acento-contenido.px-5.py-4.mb-5.mb-md-0(data-aos="fade-right")
            p.m-0 Se puede tomar como ejemplo, la propia página web de la organización que puede proporcionar un directorio de personal o una lista de las biografías de los empleados, lo que resulta útil si el pirata informático necesita utilizar un ataque de ingeniería social para alcanzar el objetivo. 
        .col-12.col-md-5
          figure
            img(src='@/assets/curso/tema1/img01.svg' data-aos="zoom-in-down") 
    
    .row.mb-4
      .col-12.col-md-4
        figure
          img.d-none.d-lg-block.posit_img02_t1(src='@/assets/curso/tema1/img02.png' data-aos="zoom-in-down") 
      .col-12.col-md-4
        .tarjeta.bg_color3.p-3.margin1.height1(data-aos="fade-left")
          .row
            .col-md-2
              figure
                img.img400(src='@/assets/curso/tema1/img05.svg', alt='Texto que describa la imagen')
            .col-md-10
              h3.mt-2 Tenga presente
            p.m-0.ms-2 La información que el hacker busca durante la fase de huella es cualquier elemento que dé pistas sobre la arquitectura de la red, el servidor y los tipos de aplicaciones donde se almacenan los datos valiosos.
      .col-12.col-md-4
        .tarjeta.bg_color3.p-3.margin1(data-aos="fade-left")
          .row
            .col-md-2
              figure
                img.img400(src='@/assets/curso/tema1/img05.svg', alt='Texto que describa la imagen')
            .col-md-10
              h3.mt-2 Importante
            p.m-0 Antes de que se pueda lanzar un ataque o un exploit, lo que el hacker también busca es el sistema operativo y la versión, así como los tipos de aplicaciones deben ser descubiertos para que se pueda lanzar el ataque más efectivo contra el objetivo.

    p Estos son algunos de los datos que se deben reunir, sobre un objetivo, durante el <em>footprinting</em>:

    .row.mb-4
      .col-12.col-md-3.align-self-end
        ul
          li 
            i.fas.fa-check-circle
            |  Nombre de dominio.
          li 
            i.fas.fa-check-circle
            |  Bloques de red.
          li 
            i.fas.fa-check-circle
            |  Servicios y aplicaciones de red.
          li 
            i.fas.fa-check-circle
            |  Arquitectura del sistema.
          li 
            i.fas.fa-check-circle
            |  Sistema de detección de intrusos.
      .col-12.col-md-3.align-self-end
        ul
          li 
            i.fas.fa-check-circle
            |  Mecanismos de autenticación.
          li 
            i.fas.fa-check-circle
            |  Direcciones IP específicas.
          li 
            i.fas.fa-check-circle
            |  Mecanismos de control de acceso.
          li 
            i.fas.fa-check-circle
            |  Números de teléfono.
          li 
            i.fas.fa-check-circle
            |  Direcciones de contacto.
      .col-12.col-md-6
        figure
          img(data-aos="fade-left")(src='@/assets/curso/tema1/img03.png')

    p.mb-4 Una vez que esta información es compilada, puede dar a un hacker una mejor visión de la organización, donde se almacena la información valiosa y cómo se puede acceder a ella. 

    #t_1_1.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 1.1	Concepto y generalidades

    .bg_fondo2tema1
      .row.justify-content-center
        .col-12.col-md-7.align-self-end.mt-5.margintop_1
          p.mb-4 El <em>footprinting</em> es el proceso de reunir la mayor cantidad de información posible sobre un sistema/red objetivo para identificar diferentes formas de intrusión en la red de una organización. 
          p.mb-4 Dentro de los procesos más comunes de esta técnica están:
          .row.justify-content-center
            .col-12.col-md-10
              ul
                li 
                  i.fas.fa-check-circle
                  |  Recoger información básica.
                li 
                  i.fas.fa-check-circle
                  |  Encuentra la versión del sistema operativo, la edición del servidor web, etc.
                li 
                  i.fas.fa-check-circle
                  |  Obtener información de DNS usando Whois, etc.
                li 
                  i.fas.fa-check-circle
                  |  Busca vulnerabilidades y explota para lanzar ataques.
        .col-12.col-md-5.align-self-center.mt-5.margintop_1
          figure
            img(data-aos="fade-left")(src='@/assets/curso/tema1/img06.png')
        
      .row.justify-content-center.mt-5
        .col-12.col-md-12
          .cajon.color-secundario.px-5.py-4(data-aos="fade-right")
            p.m-0 El <em>footprinting</em> es el primer paso en el hacking ético e implica la recolección de información sobre el objetivo y su entorno. En esta etapa se puede recopilar información importante que luego es útil en las etapas posteriores del hacking ético. 

      p.mt-4 El <em>footprinting</em> se puede llevar a cabo de diferentes formas, entre las que se destacan:

    ImagenInfograficaB.color-primario
      template(v-slot:imagen)
        figure
          img(src='@/assets/curso/tema1/imginfografica.svg')

      div(x="55.4%" y="21.3%" tooltip="1. OSINT (Open Source INTelligence)")
        .row.justify-content-between
          .col-12.col-md-6
            h5.mb-4 1. OSINT (Open Source INTelligence)
            p.mb-4 En la práctica, esto tiende a significar información encontrada en internet, pero técnicamente cualquier información pública entra en la categoría de OSINT, ya sean libros o informes en una biblioteca pública, artículos en un periódico o declaraciones en un comunicado de prensa.
            p.mb-4 El OSINT también incluye información que puede encontrarse en diferentes tipos de medios: en texto, en imágenes, vídeos, seminarios web, discursos públicos y conferencias.
          .col-12.col-md-6
            figure
              img(src='@/assets/curso/tema1/img07.svg')
      div(x="45.1%" y="76.1%" tooltip="6. Objetivos del <em>footprinting</em>)")
        .row.mb-5
          .col-12.col-md-12
            h5 6. Objetivos del <em>footprinting</em>
        .row.justify-content-center.align-items-center
          .col-md-1
            p.m-0.font_1 Recopilar información de red
          .col-md-3
            .verticalLine 
              ul
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Nombre de dominio.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Nombres de dominio internos.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Direcciones IP que sean alcanzables en la red de la colectividad.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Sitios web Rogue páginas web de información privada.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  TCP y UDP, servicios que se ejecutan.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Protocolos de red.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  Puntos VPN.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  ACs.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text.small  IDS que ejecutan.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Analógico / números de teléfono digitales.
                li
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Los mecanismos de autenticación.
          .col-md-1
            p.m-0.font_1 Recopilar información del sistema
          .col-md-3
            .verticalLine 
              ul
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Los nombres de usuario y de grupo.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Banderas del sistema.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Las tablas de enrutamiento.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Información de SNMP.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  La arquitectura del sistema.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Tipo de sistema remoto.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small Los nombres de sistema.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Contraseñas.
          .col-md-1
            p.m-0.font_1 Recopilar información de la organización
          .col-md-3
            .verticalLine 
              ul
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Detalles del empleado.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Página web de la organización.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Directorios de la empresa.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Direcciones y teléfonos.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  Antecedentes de la organización.
                li 
                  <i class="fas fa-circle fa-xs" style= "color:#E01650"></i>
                  strong.m-0.text-small  News: artículos notas de prensa.


    
    Separador

    #t_1_2.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 1.2	Herramientas y Google Hacking

    .row.justify-content-center.align-items-center.mb-5.mt-4           
      .col-lg-12 
        .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="fade-down")
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img08.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p.m-0 Dentro del hacking ético, existen diferentes herramientas para poder realizar un reconocimiento de huellas o <em>footprinting</em>. Este proceso busca información pública o privada que pueda ser objeto de un ataque.
              br

    p.m-o.text-center Para ello, se pueden realizar diferentes actividades, como las que se describen a continuación:

    .tarjeta-color.bg_color6.p-5.mb-5  
      SlyderA.mb-5(:datos="datosSlyder")
        .row.justifiy-content-around
          .col-md-5(data-aos="fade-right")
            h5.mb-4 Herramientas de creación mirroring sitio web
            p.m-0.mb-4.mb-md-0 Estas aplicaciones pueden reconocer automáticamente la estructura de cierta página o brindar una interfaz al usuario, en donde este pudiera seleccionar los campos que son de interés dentro del documento; de esta forma, no es necesario escribir manualmente un código para realizar tareas.
          .col-md-7
            figure
              img(data-aos="fade-left")(src='@/assets/curso/tema1/img09.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.mb-4 Creación de un reflejo de sitio web
            p.m-0.mb-4.mb-md-0 Crear un reflejo de un sitio web no es lo mismo que hacer una copia de seguridad. El reflejo es descargar una copia de todos los archivos que componen el sitio (imágenes, archivos CSS y JavaScript), así como versiones estáticas del HTML. Es fácil conseguir que la gente almacene esta réplica que, a diferencia de la copia de seguridad, se verá igual que el sitio web, pero es importante entender que un espejo de sitio web no es una copia exacta, es una copia estática, lo que significa que no puede hacer nada dinámico como iniciar sesión, editar mensajes o publicar comentarios.
          .col-md-7
            figure
              img(src='@/assets/curso/tema1/img10.png', alt='Texto que describa la imagen')
        .row.justifiy-content-around
          .col-md-5
            h5.mb-4 WebHTTrack
            p.m-0.mb-4.mb-md-0 Aplicación que permite la descarga a un directorio local de una parte o de todo un sitio web: imágenes, PDF, etc. para poder estudiarlo posteriormente sin conexión a internet. Permite distinguir entre los enlaces internos y los externos, traccionando los primeros y excluyendo los segundos, lo que reduce el tiempo de maniobra.
          .col-md-7
            figure
              img(src='@/assets/curso/tema1/img11.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.mb-4 HTTRack permite
            p.m-0.mb-4.mb-md-0 Permite descargar un sitio de la World Wide Web, desde Internet a un directorio local, construyendo recursivamente todos los directorios, obteniendo HTML, imágenes y otros archivos del servidor a su computadora. HTTrack organiza la estructura de enlaces relativa del sitio original: simplemente abre una página del sitio web "reflejado" en el navegador y podrá navegar el sitio, de enlace en enlace, como si lo estuviera viendo en línea. HTTrack también puede actualizar un sitio duplicado existente y reanudar descargas interrumpidas.
          .col-md-7
            figure
              img(src='@/assets/curso/tema1/img12.png', alt='Texto que describa la imagen')
        .row.justifiy-content-evenly
          .col-md-5
            h5.mb-4 Seguimiento de comunicaciones de correo electrónico
            p.m-0.mb-4.mb-md-0 El seguimiento a correos electrónicos es un método para controlar y espiar los correos electrónicos entregados al destinatario. Los rastreadores de correo electrónico son extensiones del navegador para Chrome que agrega, automáticamente, una imagen de 1x1 píxel al cuerpo del correo electrónico que se envía; una vez que un destinatario lo abra, su navegador solicita obtener esa imagen del servidor donde está alojado, esta solicitud se analizará indicando que el correo electrónico se ha abierto.
          .col-md-7
            figure
              img(src='@/assets/curso/tema1/img13.png', alt='Texto que describa la imagen')
      
    .row.justify-content-center
      .col-12.col-lg-10
        .tarjeta.bgr2.mb-5.mb-md-0(data-aos="fade-up")
          .row.justify-content-center.align-items-center
            .col-8.col-sm-6.col-md-5.mb-4.mb-md-0
              img(src="@/assets/curso/tema1/img14.png")

            .col-md-6.col-lg-6
              h4.mb-4.ms-4.ms-md-0 Algunas herramientas para el footpringting
              p.mb-4.text.small.ms-4.ms-md-0 Conozca, sucintamente, algunas herramientas, con sus particularidades, a través de las cuales es posible hacer reconocimiento de huellas o <em>footprinting</em>. Explore el Anexo_1_HerramientasYGoogleHacking.
              
              a.boton.bgr1.margin2(:href="obtenerLink('/downloads/OKEst_Anexo_1_HerramientasYGoogleHacking.docx')" target="_blank" type="application/pdf")
                span Descargar
                i.fas.fa-file-download
              img.posit.img116(src="@/assets/curso/tema1/img15.png")   
    
    Separador.mt-5.mt-md-0

    #t_1_3.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 1.3 Contramedidas

    p.m-0.mb-4(data-aos="fade-right") Dentro del <em>footprinting</em> o huellas, se debe tener en cuenta que las contramedidas que se pueden realizar son múltiples, dependiendo del trato que se les pueda dar, según el caso que se presente.

    .row.justifiy-content-center.align-items-center(data-aos="fade-right")
      .col-12.col-md-6
        p.mb-4 Para una mejor comprensión del proceso de mitigación de ellas, se presentan a continuación algunas consideraciones importantes:
        ul.lista-ul
          li 
            i.fas.fa-check-circle
            |  Configurar routers para restringir las respuestas a la solicitud de <em>footprinting</em>.
          li 
            i.fas.fa-check-circle
            |	Configurar servidores de internet para evitar la fuga de información y desactivar los protocolos no deseados.
          li 
            i.fas.fa-check-circle
            |	Bloquear los puertos con la configuración adecuada del firewall.            
          li 
            i.fas.fa-check-circle
            |	Utilizar un IDS que se pueda configurar para rechazar el tráfico sospechoso y recoger los patrones de <em>footprinting</em>.
          li 
            i.fas.fa-check-circle  
            |	Evaluar la información antes de publicarla en el sitio web / internet.
          li 
            i.fas.fa-check-circle
            |	Realizar técnicas de <em>footprinting</em> y eliminar cualquier información sensible encontrada.
          li 
            i.fas.fa-check-circle
            |	Evitar que los motores de búsqueda almacenen caché de una página web y el uso de registro de servicios anónimos.
          li 
            i.fas.fa-check-circle
            |	Desactivar la lista de directorios y utilizar Split DNS.
      .col-12.col-md-6(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema1/img16.png', alt='Texto que describa la imagen')

    .row.justify-content-center.align-items-center.mb-5.mt-4           
      .col-lg-12 
        .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="flip-down")
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img17.png')})`}"
          )
          .bloque-texto-g__texto.p-4
            p <b>Pentesting de <em>footprinting</em></b>
            br
            br
            p El pentest de <em>footprinting</em> se utiliza para determinar la información de la organización, a disposición del público en Internet: arquitectura de red, sistemas operativos, aplicaciones y usuarios. El pentester intenta reunir la mayor cantidad de información posible acerca de la organización destino en internet y otras fuentes accesibles al público.
              br  
    
    p.m-0.text-center.mb-4(data-aos="fade") El <em>footprinting</em> es el primer paso por realizar dentro de la prueba de penetración; se deben tener presentes los siguientes aspectos:

    
    .row.justify-content-center.align-items-center.mb-5
      .col-12.col-md-4
        .tarjeta.bg_color2.p-3.margintop_2
          .row.justifiy-content-center
            .col-md-6.d-flex.align-self-center
              figure.mb-5
                img.img100.margin3(src='@/assets/curso/tema1/img18.svg')
          .row.justifiy-content-center
            .col-md-12  
              h4.text-center.margin4 El fingerprinting 
      .col-12.col-md-4
        .tarjeta.bg_color2.p-3.margintop_2 
          .row.justifiy-content-center
            .col-md-6.d-flex.align-self-center
              figure.mb-4
                img.img90.margin5(src='@/assets/curso/tema1/img05.svg')
          .row.justifiy-content-center
            .col-md-12  
              h4.text-center.margin4 La actividad del <em>footprinting</em>

    p.m-0.mb-5.text-center Los doce pasos principales a seguir en la prueba de penetración de <em>footprinting</em> son:

    
    .row.mb-5
      .col-md-7.mb-5.mb-md-0(data-aos="fade-right")
        LineaTiempoD.color-secundario
          p(numero="1" titulo="Obtener la autorización correcta") Realice siempre las pruebas de penetración con autorización, el primer paso en una prueba de penetración es inducir la correcta autorización de la organización. Esto puede o no incluir a los directores del sistema.
          
          p(numero="2" titulo="Definir el alcance de la evaluación") La definición del alcance de la evaluación de la seguridad podría ser un requisito para el proceso de prueba de la pluma, el alcance de la evaluación determina la gama de sistemas dentro de la red para comprobar, por lo tanto, los recursos que pueden utilizarse para probar también determinan las limitaciones del pentester. 
          
          p(numero="3" titulo="Realizar el <em>footprinting</em> a través de los motores de búsqueda") Usar los motores de búsqueda de huellas como Google, Yahoo! Search, Ask, Bing, y Dog pile para reunir los datos de la organización objetivo como los detalles de los empleados, las páginas de acceso y los portales de intranet, entre otros, eso puede ayudar en la actividad de ingeniería social y variedades alternativas de ataques a sistemas avanzados.
          
          p(numero="4" titulo="Realizar el <em>footprinting</em> a través de servicios web") Realizar el <em>footprinting</em> a través de servicios web como Net craft, Pip, Google Finance y Google Alerts para reunir datos relativos al sitio web de la organización objetivo, los empleados, el competidor, la infraestructura y los sistemas operativos.

          p(numero="5" titulo="Realizar el <em>footprinting</em> a través de sitios de redes sociales") Realizar la impresión del pie para recoger los objetivos del órgano objetivo del empleado de la nación de la impresión del pie, datos de perfiles personales en sitios de redes sociales como Facebook, rvlySpace, LinkedIn, Twitter, Interest, Google+, etc. Esto puede ayudar en la actividad de ingeniería social, además, usarás los motores de búsqueda de personas para obtener datos de algunas personas objetivo.

          p(numero="6" titulo="Realizar el <em>footprinting</em> del sitio web") Realizar el <em>footprinting</em> de un sitio web usando herramientas como Burp Suite, web information Extractor, Track web site duplicator, Metabolite. Website-Watcher para crear un mapa detallado de la estructura y diseño del sitio web.
      .col-md-5.mb-5.mb-md-0
        figure
          img(data-aos="fade-left")(src='@/assets/curso/tema1/img19.png')
    .row.mb-5
      .col-md-5.mb-5.mb-md-0
        figure
          img(data-aos="fade-right")(src='@/assets/curso/tema1/img20.png')
      .col-md-7.mb-5.mb-md-0
        LineaTiempoD.color-secundario(data-aos="fade-left")        
          p(numero="7" titulo="Realizar la huella del correo electrónico") Hacer el <em>footprinting</em> del correo electrónico utilizando herramientas como Yes ware, y Contractility para reunir datos sobre la ubicación física de un individuo. Usar esto para realizar ingeniería social la que, a su vez, podría ayudar en el mapeo de la red de la organización objetivo. Analizar los encabezados de los correos electrónicos ayudará a reunir datos como la dirección IP del remitente, el servidor de correo del remitente, la dirección del remitente, la información y la hora de recepción de los bytes de los servidores de correo electrónico del remitente, el sistema de autenticación utilizado por el servidor de correo del remitente, el nombre completo del remitente, etc.

          p(numero="8" titulo="Recopilar la inteligencia competitiva") Reunir inteligencia competitiva usando herramientas como Hoover's, LexisNexis, o Business Wire. Estas herramientas extraen datos de la competencia como su fecha de establecimiento, ubicación, análisis de progreso, autoridades superiores, análisis de productos, detalles de marketing, etc.
          
          p(numero="9" titulo="Realizar el <em>footprinting</em> de WHOIS") Realizar el <em>footprinting</em> utilizando herramientas como WHOIS es la búsqueda del convertidor de IP por lotes para extraer los datos relativos a los dominios explícitos, se capturan datos como la dirección IP, el nombre del propietario del dominio, el nombre del registrante y los detalles de contacto, incluyendo números de teléfono e identificaciones de correo electrónico; el conocimiento se utilizará para crear un mapa detallado de la red de la organización y reunir datos personales.

          p(numero="10" titulo="Realizar el <em>footprinting</em> del DNS") Usando herramientas como DNs, DIG y DNS para trabajar, anfitriones clave dentro de la red y para realizar ataques de ingeniería social, resolver el nombre de dominio para averiguar sobre su dirección IP, registros DNS, etc.

          p(numero="11" titulo="Realizar el <em>footprinting</em>") Aquí se usan herramientas como Path analyzer pro, Visual Route, y GEO Spider. La red varía y los datos alternativos con respecto a la red del objetivo ayudan a dibujar el diagrama de la red del objetivo.

          p(numero="12" titulo="Realizar ingeniería social") Aplicar técnicas de ingeniería social como Eavesdropping, Shoulder surfing, Dumpster diving, la suplantación de identidad en sitios de redes sociales y el phishing para reunir datos esenciales sobre la organización objetivo, a través de la ingeniería social, se reunirá los elementos de seguridad de la organización objetivo en uso, las versiones del sistema operativo y el software, los datos de la disposición de la red, las direcciones IP, así como los nombres de los servidores y el personal vital.



  </template>

<script>
export default {
  name: 'Tema1',
  components: {},
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
