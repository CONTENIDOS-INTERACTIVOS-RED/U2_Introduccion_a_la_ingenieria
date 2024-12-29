<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from '@/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Tecnologías Emergentes en la Industria',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> Evaluar el conocimiento sobre las tecnologías emergentes y su aplicación en la industria moderna.',
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
}
</script>
