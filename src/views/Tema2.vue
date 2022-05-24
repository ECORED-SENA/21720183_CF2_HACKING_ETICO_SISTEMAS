<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 2
      h2 Escaneo de redes y dispositivos
    
    .bg_fondo1_t2
      .row.justify-content-center.align-items-center.mb-5.mt-4           
        .col-lg-10 
          .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="flip-down")
            .bloque-texto-g__img(
              :style="{'background-image': `url(${require('@/assets/curso/tema2/img01.png')})`}"
            )
            .bloque-texto-g__texto.p-4
              p.m-0 El escaneo en redes y dispositivos dentro de un sistema busca encontrar todo tipo de vulnerabilidades para identificar fallas en la seguridad, es el segundo paso a realizarse después de un levantamiento de huellas. Es de suma importancia apropiar conocimientos básicos y esenciales para aplicar herramientas que ayuden a determinar este tipo de acciones, orientadas a la seguridad e integridad de la información e infraestructura de una organización.
                br  

      p.m-0 Sabiendo lo anterior, se invita a profundizar a través del siguiente video en los principales conceptos y generalidades del escaneo de redes y dispositivos. Se sugiere llevar registro de los aspectos más relevantes en una libreta personal de apuntes:

      .row.justify-content-center(data-aos="fade-up")
        .col-12.col-md-12.posit_relative2    
          figure.mb-5
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/W2xX-bc0aj8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
      
      Separador

      #t_2_1.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
        h2 2.1	Concepto y generalidades

      .row.justify-content-center.align-items-center.mb-5.mt-4           
        .col-lg-10 
          .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5(data-aos="flip-down")
            .bloque-texto-g__img(
              :style="{'background-image': `url(${require('@/assets/curso/tema2/img02.png')})`}"
            )
            .bloque-texto-g__texto.p-4
              p.m-0 Para que un <em>hacker</em> ético pueda realizar exploraciones a los sistemas y redes, debe determinar las metodologías de escaneo, las cuales se pueden resumir en: comprobación de sistemas vivos, comprobación de puertos abiertos, captura de banderas, análisis de búsqueda de vulnerabilidades, dibujo de diagramas de red, preparación de <em>proxies.</em>
                br  

      p.m-0.mb-4 Tenga en cuenta las siguientes particularidades de las exploraciones y escaneos que puede realizar el hacker ético:

      .row.justify-content-center
        .col-12.col-md-12
          .tarjeta-color.p-5.mb-5.bg_color10
            SlyderA(tipo="b").color_bot_slyder1_t1
              .row.justify-content-around
                .col-md-5(data-aos="fade-right")
                  h4.mb-4 Comprobación de sistemas vivos escaneo ICMP
                  p.m-0.mb-4.mb-md-0 El ICMP (<em>Internet Control Message Protocol</em>) es un protocolo que los dispositivos de red (por ejemplo, los enrutadores) utilizan para generar mensajes de error cuando los problemas de la red impiden que los paquetes IP pasen.
                .col-md-7
                  figure
                    img(data-aos="fade-left")(src='@/assets/curso/tema2/img03.png', alt='Texto que describa la imagen')
              .row.justify-content-around
                .col-md-5
                  h4.mb-4 Ping ICMP
                  p.m-0.mb-4.mb-md-0 El Ping utiliza dos códigos ICMP: 8 (solicitud de eco) y 0 (respuesta de eco). Cuando se emite el comando Ping en el <em>prompt</em>, el programa Ping envía un paquete ICMP que contiene el código 8 en el campo <em>Type</em>; la respuesta tendrá un tipo de 0. El programa multiplica por el espacio entre el envío del paquete de solicitud de eco y la llegada de la respuesta. Así, puede obtener el "tiempo de ida y vuelta" de un paquete a la red de destino dada y de vuelta.
                .col-md-7
                  figure
                    img(src='@/assets/curso/tema2/img04.svg', alt='Texto que describa la imagen')
              .row.justifiy-content-around
                .col-md-5
                  h4.mb-4 Paquete de solicitud de eco
                  p.m-0.mb-4.mb-md-0 Es inusual en el sentido de que es el único paquete ICMP que se envía sin ser provocado por un error. Por lo tanto, Ping no tiene que emular una condición de error para obtener un mensaje ICMP de vuelta. Ping tiene dos opciones que permiten especificar una lista de direcciones para el camino que debe tomar la transmisión: "-j", que sugiere una ruta, y "-k", que dicta la ruta.
                .col-md-7
                  figure
                    img(src='@/assets/curso/tema2/img05.svg', alt='Texto que describa la imagen')
              .row.justifiy-content-evenly
                .col-md-5
                  h4.mb-4 Barrido de Ping Sweep
                  p.m-0.mb-4.mb-md-0 Determina los <em>hosts</em> vivos de un rango de direcciones IP, mediante envío de peticiones de eco ICMP a múltiples <em>hosts</em>. Si un <em>host</em> está vivo, devolverá una respuesta de eco ICMP. Es una técnica usada para identificar si los anfitriones están activos en las redes usando sus direcciones IP. El método de barrido de Ping se utiliza para hacer Ping a muchos <em>hosts</em> a la vez. Por ejemplo, si hay una red con una identificación de red 192.10.0.0/24, entonces es muy simple identificar el número total de <em>hosts</em> allí mediante un Ping de barrido de esta red. 
                .col-md-7
                  figure
                    img(src='@/assets/curso/tema2/img06.svg', alt='Texto que describa la imagen')
              .row.justifiy-content-evenly
                .col-md-5
                  h4.mb-4 Three Way Handshake
                  p.m-0.mb-4.mb-md-0 También denominado TCP 3-<em>way handshake</em>, es un proceso utilizado en una red TCP/IP para hacer una conexión entre el servidor y el cliente, es un proceso de tres pasos que requiere que, tanto el cliente como el servidor, intercambien paquetes de sincronización y reconocimiento antes de que comience el verdadero proceso de comunicación de datos.
                .col-md-7
                  figure
                    img(src='@/assets/curso/tema2/img07.svg', alt='Texto que describa la imagen')

      .row.justifiy-content-center
        .col-12.col-md-4
          figure
            img(data-aos="fade-right")(src='@/assets/curso/tema2/img08.svg')
        .col-12.col-md-8
          .cajon.color-primario.p-3.mb-4(data-aos="fade-left")
            h5.ms-3.pt-2 Proceso de apretón de manos
            p.ms-3.pt-2 El proceso de apretón de manos de tres vías está diseñado de tal manera que ambos extremos ayudan a iniciar, negociar y separar las conexiones de sockets TCP al mismo tiempo. También permite transferir múltiples conexiones de sockets TCP, en ambas direcciones, al mismo tiempo. 

      p.m-0.mb-4 He aquí los tres pasos:

      TabsA.color-acento-botones.mb-5(data-aos="fade-right")
        .tarjeta.color-acento-botones--borde.p-4.border_radius1(titulo="PASO 1")
          .row.justify-content-center.align-items-center
            .col-12.col-md-7
              h4 PASO 1
              p En el primer paso el cliente establece una conexión con un servidor. Envía un segmento con SYN e informa al servidor acerca de que el cliente debe iniciar la comunicación, y con lo que debe ser su número de secuencia.
            .col-12.col-md-4
              figure
              img(src='@/assets/curso/tema2/img10.svg')
        
        .tarjeta.color-acento-botones--borde.p-4.border_radius1(titulo="PASO 2")
          .row.justify-content-center.align-items-center
            .col-12.col-md-7
              h4 PASO 2
              p En este paso el servidor responde a la solicitud del cliente con la señal SYN-ACK establecida. ACK le ayuda a significar la respuesta del segmento que se recibe y SYN significa qué número de secuencia debe ser capaz de comenzar con los segmentos.
            .col-12.col-md-4
              figure
              img(src='@/assets/curso/tema2/img09.svg')

        .tarjeta.color-acento-botones--borde.p-4.border_radius1(titulo="PASO 3")
          .row.justify-content-center.align-items-center
            .col-12.col-md-7
              h4 PASO 3
              p En este último paso el cliente reconoce la respuesta del servidor, y ambos crean una conexión estable que iniciará el proceso de transferencia real de datos.
            .col-12.col-md-4
              figure
              img(src='@/assets/curso/tema2/img11.svg')
      
      .row.justifiy-content-center.align-items-center
        .col-12.col-md-8
          .cajon.color-primario.p-3.mb-4(data-aos="fade-right")
            h5.ms-1.pt-2 Banderas de comunicación TCP
            p.ms-1.pt-2 Las banderas de TCP tienen la misma función de mostrar cambios, situaciones o condiciones de la información; podrían compararse con un semáforo, ya que alertan sobre cuándo se debe parar, seguir o tener precaución. Estas banderas informan el estado de la información, de extremo a extremo, para que los datos lleguen íntegros (tal cual como son).
        .col-12.col-md-4
          figure
            img(data-aos="fade-left")(src='@/assets/curso/tema2/img12.svg')

    ImagenInfografica.manito.color-secundario.mb-5(data-aos="fade-up")
      template(v-slot:imagen)
        figure
          img(src='@/assets/curso/tema2/imginfografica_t2.svg', alt='Texto que describa la imagen')
          figcaption Banderas de comunicación TCP

      .tarjeta.color-acento-contenido.p-3(x="12.7%" y="32.2%")
        .h5.mb-2 Sincronización (SYN) 
        p Se utiliza en el primer paso de la fase de establecimiento de la conexión o el proceso de apretón de manos de tres vías entre los dos anfitriones. Solo el primer paquete del remitente y del receptor debe tener esta bandera. Se utiliza para sincronizar el número de secuencia, es decir, para indicar al otro extremo el número de secuencia que debe exceptuar.

      .tarjeta.color-acento-contenido.p-3(x="12.7%" y="57.8%")
        .h5.mb-2 Acuse de recibo (ACK) 
        p Se utiliza para acusar recibo de los paquetes que son recibidos con éxito por el host. El indicador se establece si el campo de número de confirmación contiene un número de confirmación válido.

      .tarjeta.color-acento-contenido.p-3(x="12.7%" y="84%")
        .h5.mb-2 Finalizar (FIN) 
        p Se utiliza para solicitar la terminación de la conexión, es decir, cuando no hay más datos del remitente solicita la terminación de la conexión. Este es el último paquete enviado por el remitente. Libera los recursos reservados y termina la conexión con gracia.

      .tarjeta.color-acento-contenido.p-3(x="87.4%" y="32%")
        .h5.mb-2 Reset (RST) 
        p Se utiliza para terminar la conexión si el remitente RST siente que algo está mal con la conexión TCP o que la conversación no debería existir. Puede ser enviado desde el lado del receptor cuando el paquete es enviado a un host particular que no lo esperaba.

      .tarjeta.color-acento-contenido.p-3(x="87.4%" y="57.8%")
        .h5.mb-2 Push (PSH)
        p La capa de transporte por defecto espera durante algún tiempo a que la capa de aplicación envíe suficientes datos, iguales al tamaño máximo del segmento para que el número de paquetes transmitidos en la red se reduzca al mínimo, lo cual no es deseable por alguna aplicación, como las aplicaciones interactivas (chat). De manera similar, la capa de transporte en el extremo del receptor almacena los paquetes y los transmite a la capa de aplicación, si cumple ciertos criterios.

      .tarjeta.color-acento-contenido.p-3(x="87.4%" y="84%")
        .h5.mb-2 Urgente (URG)
        p Los datos dentro de un segmento con URG = 1 bandera se transmite a la capa de aplicación inmediatamente, aunque haya más datos que dar a la capa de aplicación. Se utiliza para notificar al receptor que procese los paquetes urgentes antes de procesar todos los demás paquetes. Se notificará al receptor cuando se hayan recibido todos los datos urgentes conocidos.
    
    Separador

    #t_2_2.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 2.2	Herramientas de escaneo

    .row.justify-content-center.mb-4
      .col-12.col-md-10
        .cajon.color-acento-contenido.p-2.mb-5.mb-md-0(data-aos="fade-left")
          .row.justify-content-around.align-items-center
            .col-md-10
              p.m-0.ms-4 Hablar de estas para identificar diferentes vulnerabilidades en un sistema, consiste tanto en permanecer en el anonimato como en falsificar la identidad de un dispositivo que era confiable por los sistemas defensivos; todo con el fin de realizar intrusiones y analizar qué fallas existen en las redes y solventarlas.
            .col-md-2
              figure
                img(src='@/assets/curso/tema2/img13.svg')
    
    p.m-0.mb-5 Entre las herramientas más comunes, se pueden mencionar:

    .row.mb-5
      .col-md-6.mb-5.mb-md-0(data-aos="fade-right")
        LineaTiempoD.color-secundario
          p(numero="1" titulo="Hping 2 Hping 3") Hping3 es una herramienta que se utiliza desde la consola o terminal en Linux, cuyo fin es el análisis y ensamblado de paquetes TCP/IP, similar al comando Ping. Esta herramienta, además de enviar paquetes ICMP, también puede enviar paquetes TCP, UDP y RAW-IP de una forma muy rápida.
          
          p(numero="2" titulo="Utilidad de Hping3") Esta aplicación puede ser muy útil a la hora de realizar testeos de seguridad sobre firewalls, escaneo avanzado de puertos o seguimiento de rutas, distintos tipos de pruebas sobre varios protocolos y también se puede verificar la capacidad de generar una denegación de servicio (DoS) mediante un flood de paquetes modificados.
          
          p(numero="3" titulo="Herramienta de Análisis Nmap") Nmap, abreviatura de Network Mapper, es una herramienta gratuita y de código abierto para la exploración de vulnerabilidades y el descubrimiento de redes. Los administradores de red utilizan Nmap para identificar qué dispositivos se están ejecutando en sus sistemas, descubriendo los hosts que están disponibles y los servicios que ofrecen, encontrando los puertos abiertos y detectando los riesgos de seguridad.

          p(numero="4" titulo="Usos de Nmap") Puede ser usado para monitorear tanto hosts individuales como vastas redes que abarcan cientos de miles de dispositivos y multitud de subredes. Aunque Nmap ha evolucionado a lo largo de los años y es extremadamente flexible, en el fondo es una herramienta de escaneo de puertos que recopila información enviando paquetes sin procesar a los puertos del sistema, escucha las respuestas y determina si los puertos están abiertos, cerrados o filtrados de alguna manera, por ejemplo, un cortafuego.

          p(numero="5" titulo="Zenmap") Zenmap es una interfaz gráfica de código abierto para Nmap. Está disponible en muchos sistemas operativos (Linux, Windows, Mac OS X, BSD, etc.) y hace que Nmap sea más fácil de usar para los principiantes. Zenmap suele estar empaquetado con el propio Nmap, pero si se desea descargarlo por separado, se  puede hacer en https://nmap.org/download.html.

      .col-md-6
        figure
          img(data-aos="fade-left")(src='@/assets/curso/tema2/img14.png')

    .row.justify-content-center.mb-4      
      .col-lg-5
        figure
          img.mb-5.mb-md-0(data-aos="fade-right")(src='@/assets/curso/tema2/img15.svg')
      .col-lg-7
        .cajon.color-acento-botones.p-4(data-aos="fade-left")
          .h5.mb-4 ¡Importante!
          p.m-0 Cuando los profesionales de la ciberseguridad utilizan herramientas de escaneo en las redes y dispositivos de las organizaciones, puede haber riesgos legales que deben ser manejados por los individuos y las empresas. A menudo, los instrumentos de exploración se utilizan para medir el cumplimiento de las políticas y leyes de ciberseguridad, por lo que deben utilizarse con el debido cuidado; hay protocolos que deben seguirse para garantizar el uso adecuado de los instrumentos de escaneo

    Separador

    #t_2_3.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 2.3	<em>Fingerprinting</em>, aparcamiento y OS

    .row.justify-content-center.align-items-center.mb-5(data-aos="fade-up")
      .col-12.col-md-4
        p.m-0 OS <em>fingerprinting</em> se refiere a la detección del sistema operativo de un host final, mediante el análisis de paquetes, que se originan en ese sistema. Es utilizada por los profesionales de la seguridad y los piratas informáticos para trazar mapas de redes remotas y determinar qué vulnerabilidades podrían estar presentes para ser explotadas.
        .tarjeta-color.bg_color7.p-2
          p.m-0 OS <em>fingerprinting</em> funciona solo para paquetes que contienen una conexión TCP completa; es decir, la conexión TCP debe tener una conexión SYN, SYN/ACK y ACK
      .col-12.col-md-4
        figure
          img(src='@/assets/curso/tema2/img16.png')
      .col-12.col-md-4
        .cajon.color-secundario.py-4.px-3
          .h5.mb-4.mt-3 ¡Tenga presente!
          p.m-0 Ciertos parámetros de la definición del protocolo TCP/IP se dejan a discreción de la aplicación del sistema operativo respectivo. Los diferentes sistemas operativos establecen diferentes valores, por defecto. Al recoger y examinar estos valores, se puede diferenciar entre varios sistemas operativos.

    .bg_fondo2_t2
      p.m-0.mb-4.text-center Algunas de las áreas que pueden ser examinadas para determinar el sistema operativo son:
      .row.justify-content-center.align-items-center(data-aos="fade-right")          
        .col-12.col-md-7
          .tarjeta-color.bg_color8.p-3
            ul
              li 
                i.fas.fa-check-circle
                |  TTL.
              li 
                i.fas.fa-check-circle
                |  El tamaño de la ventana.
              li 
                i.fas.fa-check-circle
                |  Tamaño del paquete.
              li 
                i.fas.fa-check-circle
                |  DF bitl.
              li 
                i.fas.fa-check-circle
                |  TOSl.
              hr.mb-0.mt-0
            ul
              li 
                i.fas.fa-check-circle
                |  <b><em>Fingerprinting</em> activo del sistema operativo</b>
                p.m-0 Implica determinar activamente el SO de un PC objetivo, enviando paquetes cuidadosamente elaborados y examinando el comportamiento TCP/IP de las respuestas recibidas.
            ul
              li 
                i.fas.fa-check-circle
                |  <b><em>Fingerprinting</em> pasivo del sistema operativo</b>
                p.m-0 La huella del sistema operativo pasivo es el examen de una muestra de paquetes recolectada pasivamente de un host. Se basa en rastros del sistema remoto. En lugar de consultar activamente el sistema remoto, puede capturar los paquetes enviados desde el sistema remoto.
        .col-12.col-md-5
          figure
            img(data-aos="fade-left")(src='@/assets/curso/tema2/img17.png')

    Separador

    #t_2_4.titulo-segundo.color-acento-contenido(data-aos="zoom-out-right")
      h2 2.4	Uso de	<em>proxy</em> y anonimizadores

    p.m-0.mb-4 Un servidor <em>proxy</em> actúa como una puerta de enlace entre un usuario e internet. Es un servidor intermediario que separa a los usuarios finales de los sitios web que navegan. Los servidores <em>proxy</em> proporcionan diferentes niveles de funcionalidad, seguridad y privacidad, dependiendo de su caso de uso, necesidades o política de la empresa.

    .row.justify-content-center.mb-4
      .col-12.col-md-10
        .cajon.color-acento-contenido.p-4.mb-5.mb-md-0(data-aos="fade-right")
          .row.justify-content-around.align-items-center
            .col-md-7
              p.m-0 Si se utiliza un servidor <em>proxy</em>, el tráfico de internet fluye a través del servidor <em>proxy</em> en su camino hacia la dirección que se solicitó; la solicitud vuelve, entonces, a través de ese mismo servidor <em>proxy</em> (hay excepciones a esta regla) y luego el servidor <em>proxy</em> reenvía los datos recibidos del sitio web al usuario. 
            .col-md-5
              figure
                img(data-aos="fade-left")(src='@/assets/curso/tema2/img18.svg')
    
    .row.justify-content-center.align-items-stretch.mb-4
      .col-12.col-md-4
        .tarjeta-color.bg_color5.p-3.height3
          .h5.mb-4 ¡Atención!
          p.m-0 Los servidores proxy modernos hacen mucho más que reenviar las solicitudes de la web, todo en nombre de la seguridad de los datos y el rendimiento de la red.
      .col-12.col-md-4
        figure
          img(src='@/assets/curso/tema2/img19.svg')
      .col-12.col-md-4
        .tarjeta-color.bg_color3.p-3
          .h5.mb-4 ¡Importante!
          p.m-0 Actúan como un cortafuego y un filtro web, proporcionan conexiones de red compartidas y almacenan datos en caché para acelerar las solicitudes comunes. Un buen servidor proxy mantiene a los usuarios y a la red interna protegidos de las cosas malas que viven en la internet salvaje. Pueden proporcionar un alto nivel de privacidad.

    p.m-0 En el siguiente recurso se puede conocer, profundizar y asimilar las razones técnicas, por las cuales se hace útil y necesario el uso de un servidor <em>proxy</em>:

    .row.justify-content-center.mb-5(data-aos="fade-up-right")
        .col-12.col-md-12.posit_relative2    
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/T3gJn19Q520" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

    .bg_fondo3_t2.mb-4.mt-5
      .row.justify-content-center.align-items-center
        .col-12.col-md-5
          figure.ms-4.ms-md-0
            img(data-aos="fade-right")(src='@/assets/curso/tema2/img20.png')
        .col-12.col-md-7(data-aos="fade-left").mt-5
          .h5.mb-4 Anonimizadores 
          p.m-o Los sitios anonimizadores acceden a Internet a su nombre, protegiendo la información personal del usuario; Un anonimizador protege toda la información de identificación de una computadora, mientras navega en lugar de la persona, permitiendo permanecer, al menos, un paso alejada de los sitios que visita. 

    p.m-0.mb-4 Estas son las particularidades de los tipos de anonimizadores:
    
    .row.mb-5(data-aos="fade-right")
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta.color-primario
          .p-4
            .row.justify-content-center
              .col-md-4.mb-5
                figure
                  img.img.mx-auto.d-block.img100.mt-5(src='@/assets/curso/tema2/img21.svg')
            .row.justify-content-center
              .col-md-6
                h4.text-center Anonimizador

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta.color-primario
          .p-4
            .row.justify-content-center
              .col-md-4.mb-5
                figure
                  img.img.mx-auto.d-block.img100.mt-5(src='@/assets/curso/tema2/img22.svg')
            .row.justify-content-center
              .col-md-10
                h4.text-center Anonimizadores en red

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta.color-primario
          .p-4
            .row.justify-content-center
              .col-md-4.mb-5
                figure
                  img.img.mx-auto.d-block.img100.mt-5(src='@/assets/curso/tema2/img23.svg')
            .row.justify-content-center
              .col-md-12
                h4.text-center Anonimizadores de un solo punto


</template>

<script>
export default {
  name: 'Tema2',
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
