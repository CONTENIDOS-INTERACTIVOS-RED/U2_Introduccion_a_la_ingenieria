<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:titulo="'Unidad 2. Introducción a la Revolución 4.0 en Ingeniería'" :subTitulo="'3. Digitalización: conceptos simples de IoT '")
  .container.tarjeta.tarjeta--blanca.px-4.pt-4.px-md-5.pt-md-5.pb-0.mb-5
    .row.mb-5
      .col-12.col-xl-7.col-xxl-8.d-flex.flex-column
        div.d-flex.align-items-start.bg-rosa.p-4.mb-4(data-aos="fade-right")
          img.me-3(style="width: 90px" src='@/assets/curso/unidad/img-62.svg', alt='Texto que describa la imagen')
          .d-flex.flex-column
            p.pe-xl-3.mb-0(data-aos="fade-up") La Internet de las Cosas, conocida como IoT, está transformando el entorno en formas que hace algunos años parecían sacadas de la ciencia ficción. Desde los hogares hasta las grandes fábricas, esta tecnología conecta dispositivos que interactúan entre sí y con las personas de manera inteligente, creando ecosistemas que optimizan tanto la vida cotidiana como los procesos industriales.
      .d-none.d-xl-block.col-xl-5.col-xxl-4.mx-auto.mt-4.mt-xl-0(data-aos="fade-left")
        img(src='@/assets/curso/unidad/img-63.png', alt='Texto que describa la imagen')  

    p.mb-4 Para profundizar en cómo funciona el IoT y sus implicaciones en distintos ámbitos, se invita a revisar este video, que explora los beneficios, desafíos y el inmenso potencial de esta tecnología innovadora. ¡Una oportunidad que no se puede perder!
    
    figure.mb-5
      .video
        <iframe width="1903" height="748" src="https://www.youtube.com/embed/c8o7X3X2Dd8" title="Internet de las Cosas" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  
    h2.mb-4 ¿Cómo funciona el IoT?
    .row.mb-5
      .d-none.d-xl-block.col-xl-5.col-xxl-4.mx-auto.mt-4.mt-xl-0(data-aos="fade-right")
        img(src='@/assets/curso/unidad/img-64.png', alt='Texto que describa la imagen')  
      .col-12.col-xl-7.col-xxl-8.d-flex.flex-column
        div.d-flex.align-items-start.bg-azul-claro.p-4.mb-4(data-aos="fade-left")
          img.me-3(style="width: 90px" src='@/assets/curso/unidad/img-67.svg', alt='Texto que describa la imagen')
          .d-flex.flex-column
            p.pe-xl-3.mb-0(data-aos="fade-up") El Internet de las Cosas (IoT) permite conectar dispositivos físicos a la nube para recopilar y analizar datos en tiempo real, transformando industrias y ciudades a través de tecnologías interconectadas. Imagina una fábrica moderna donde cada máquina —desde robots de soldadura hasta sistemas de control de calidad— está equipada con sensores que capturan información constantemente. Estos datos se envían a la nube, donde se analizan con herramientas de inteligencia artificial, permitiendo a los ingenieros optimizar el funcionamiento de cada máquina, anticipar fallas y ajustar procesos.

    p.mb-4 Esta misma tecnología se aplica en diversas áreas como la agricultura y las ciudades inteligentes, donde sensores monitorean condiciones y adaptan recursos para optimizar resultados y mejorar la calidad de vida. Para entender mejor el funcionamiento del IoT, podemos usar una analogía arquitectónica de capas, donde cada nivel desempeña una función específica e interconectada:
    p.mb-3 <strong>Tabla 1 </strong> Funcionamiento de IoT

    .tabla-a.mb-5
      table
        thead
          tr
            th.text-center Capa
            th.text-center.border-left-gris Descripción
            th.text-center.border-left-gris Ejemplo
        tbody
          tr
            td.d-flex.text-bold Capa de Dispositivos  
            td.border-left-gris.border-right-gris Compuesta por sensores y actuadores que recolectan datos del entorno y ejecutan acciones según las instrucciones recibidas. Incluye también microcontroladores que procesan datos y toman decisiones locales.
            td.d-flex Un sensor de movimiento detecta a una persona y envía una señal a un microcontrolador, que enciende una luz.
          tr
            td.d-flex.text-bold Dirección del razonamiento  
            td.border-left-gris.border-right-gris Esta capa conecta los dispositivos entre sí y con la red externa. Protocolos como Wi-Fi, Bluetooth y Zigbee facilitan la comunicación, mientras que los gateways actúan como puentes hacia internet.
            td.d-flex Un gateway IoT recoge datos de sensores y los envía a la nube a través de una conexión Wi-Fi.
          tr
            td.d-flex.text-bold Capa de Plataforma
            td.border-left-gris.border-right-gris En la nube, los datos son procesados y analizados utilizando herramientas de big data y aprendizaje automático. Plataformas como AWS IoT Core y Azure IoT Hub proporcionan infraestructura para gestionar los dispositivos IoT.
            td.d-flex Un algoritmo analiza el consumo energético de un hogar y ajusta automáticamente la temperatura para optimizar el uso de energía.
          tr
            td.d-flex.text-bold Capa de Aplicación
            td.border-left-gris.border-right-gris Es la interfaz visible para los usuarios, donde pueden controlar los dispositivos IoT y visualizar los datos. Incluye aplicaciones móviles y web con interfaces intuitivas.
            td.d-flex Una aplicación móvil permite al usuario ajustar el termostato y controlar la iluminación en su hogar.

    p.text-bold.mb-4 Ejemplo completo: Invernadero inteligente
    p.mb-4 Un invernadero equipado con sensores mide temperatura, humedad, luz y nutrientes en el suelo. Estos datos se envían a la nube, donde un algoritmo determina si es necesario ajustar la iluminación o el riego. Los actuadores ejecutan estos cambios y el agricultor puede monitorear y ajustar los parámetros a través de una aplicación móvil.

    .row.bg-azul-claro.bg-full-width.py-4.mb-5
      div.px-5.pb-md-3.py-4.d-flex
        .d-none.d-xl-block.col-xl-5.col-xxl-4.mx-auto.mt-4.mt-xl-0(data-aos="fade-right")
          img.h-100(src='@/assets/curso/unidad/img-65.png', alt='Texto que describa la imagen')
        .col-12.col-xl-7.col-xxl-8.d-flex.ps-4.align-items-center.flex-column(data-aos="fade-left")
          h2.mb-4.pb-2.me-auto Monitoreo de procesos industriales con IoT
          p.mb-4 ¿Sabía que el IoT está revolucionando la industria mediante el monitoreo en tiempo real?  Lo invitamos a leer el documento Monitoreo de procesos industriales con IoT,  descubrirá cómo el IoT optimiza procesos, reduce costos y mejora la eficiencia en sectores clave como la manufactura y la logística.

          p.mb-5  A través de ejemplos de éxito, explore cómo las empresas líderes aplican estas tecnologías para anticiparse a fallas y fortalecer su competitividad global.
          a.d-flex.me-auto.bg-white.box-shadow.cursor-pointer(data-aos="zoom-in" :href="obtenerLink('/downloads/Anexo_Monitoreo de procesos industriales con IoT.pdf')" target="_blank")
            img.h-100(style="width: 48px" src='@/assets/componentes/pdf-icon-square.svg', alt='Texto que describa la imagen')
            p.text-small.fs-14px.my-auto.px-2 <strong>Anexo.</strong>  ¿Sabía que el IoT está revolucionando la industria mediante el monitoreo en tiempo real?


    .bg-full-width.border-top-9-azul
      .px-4.px-md-5.pt-5.pb-0
        h2 Material complementario
        .row
          .col-12.col-md-6.col-lg-8
            p.d-flex.my-4
              img.me-3.mb-auto.mt-1(src='@/assets/componentes/book.svg' :style="{'max-width':'16px'}")
              a.text-small.text-primary(target="_blank", href="https://elibro.net/es/ereader/tecnologicadeloriente/275562") Pérez Calle, R. (2024). Economía, derecho y empresa ante una nueva era: digitalización, IA, y competitividad. Dykinson.
            p.d-flex.my-4
              img.me-3.mb-auto.mt-1(src='@/assets/componentes/youtube-icon.svg' :style="{'max-width':'16px'}")
              a.text-small.text-primary(target="_blank", href="https://youtu.be/lTd9wn3HywU") La ecuación digital (2023). Industria 4.0: La convergencia IT-OT como clave del éxito [Vídeo]
          .col-12.col-md-6.col-lg-3
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='Imagen de material complementario')

    .bg-full-width.border-top.actividad(style="background-color: #ebf1f5; border-top: 5px solid #f5c145 !important")
      .p-4.p-md-5
        #Actividad                
          <Actividad :cuestionario="cuestionario"/>

</template>

<script>
import BannerInterno from '../../components/plantilla/BannerInterno'
export default {
  name: 'Tema3',
  components: {
    BannerInterno,
  },

  data: () => ({
    cuestionario: {
      tema: 'Tecnologías Emergentes en la Industria',
      titulo: 'Ponte a prueba',
      introduccion:
        'Demuestra lo que aprendiste en esta unidad y pon a prueba tus conocimientos.',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto: 'El mantenimiento predictivo se basa en:',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La inspección visual de equipos',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'El análisis de datos recopilados por sensores',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'La experiencia del personal de mantenimiento',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'El reemplazo programado de componentes',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            '¿Cuál de las siguientes NO es una ventaja de la robótica colaborativa?',
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Aumenta la productividad', esCorrecta: false },
            {
              id: 'b',
              texto: 'Mejora la calidad de los productos',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reduce la necesidad de mano de obra humana',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Facilita la implementación de nuevas tecnologías',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto: 'La ciberseguridad es fundamental en la industria porque:',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Protege los sistemas de control industrial de ataques externos',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Permite la fabricación de piezas personalizadas',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Optimiza las rutas de entrega de productos',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Aumenta la precisión de los sensores',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            '¿Cuál de las siguientes tecnologías NO está directamente relacionada con la producción?',
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Fabricación aditiva', esCorrecta: false },
            { id: 'b', texto: 'Robótica colaborativa', esCorrecta: false },
            { id: 'c', texto: 'Mantenimiento predictivo', esCorrecta: false },
            {
              id: 'd',
              texto: 'Internet de las cosas industrial',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto: 'La impresión 3D se utiliza en la medicina para:',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Crear prótesis personalizadas',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Realizar cirugías a distancia',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Diagnosticar enfermedades', esCorrecta: false },
            {
              id: 'd',
              texto: 'Desarrollar nuevos medicamentos',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass"></style>
