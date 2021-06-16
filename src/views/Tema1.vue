<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-principal
      .titulo-principal__numero
        span 1
      h1 Escenario avanzado de interoperabilidad
    
    h2.mb-4 Actores

    .tabla-a.color-secundario.mb-5
      table
        thead
          tr
            th Actor
            th Nombre del sistema de informaci&oacute;n asociado
            th Responsabilidad
        tbody
          tr
            td Departamento de Tecnolog&iacute;a
            td tecnolog&iacute;a_si
            td Obtener y crear registros para otorgar una nueva licencia a un ciudadano, a trav&eacute;s de X-Road.
          tr
            td Departamento de Ciudadan&iacute;a
            td ciudadan&iacute;a_si
            td Almacenar los datos personales de los ciudadanos.
          tr
            td Departamento de Transporte
            td transporte_si
            td Almacenar la informaci&oacute;n sobre antecedentes de suspensiones y cancelaciones de licencias de conducci&oacute;n.
          tr
            td Departamento de Tr&aacute;nsito
            td tr&aacute;nsito_si
            td Almacenar y permitir la creaci&oacute;n de registros &uacute;nicos de ciudadanos.
          tr
            td Departamento de Ense&ntilde;anza
            td ense&ntilde;anza_si
            td Almacenar informaci&oacute;n sobre ex&aacute;menes de conducci&oacute;n aplicados a los ciudadanos.
          tr
            td Departamento de Movilidad
            td movilidad_si
            td Almacenar y permitir la creaci&oacute;n de registros de licencias de conducci&oacute;n.
          tr
            td X-Road
            td xroad
            td Establecer y permitir la interoperabilidad entre los diferentes sistemas de informaci&oacute;n involucrados.
    
    .row.justify-content-center.mb-5
      .col-lg-10
        .cajon.color-secundario.ColorTarjeta2.p-4.mb-4
          .h4 Descripción
          p
            | El sistema de información del 
            strong departamento de Tecnología 
            | debe interponer con sistemas de información de los 
            strong departamentos: 
            | Tránsito, Ciudadanía, Transporte, Enseñanza y Movilidad, con el propósito de generar una nueva licencia de conducción.
          p
            | Este proceso debe realizarse a través del ecosistema 
            strong X-Road.
    
    #t1_1.titulo-segundo
      h2 1.1 Descripción detallada del escenario
      
    .row.justify-content-center.mb-5
      .col-md-7.col-lg-5
        figure.mb-4
          img(src='@/assets/curso/img01.svg', alt='Descripción detallada del escenario')

        a.anexo.mb-4(:href="obtenerLink('/downloads/Anexo1.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p 
              strong Anexo1. 
              | Descripción Detallada del Escenario
    
    #t1_2.titulo-segundo
      h2 1.2 Guía de implementación del escenario
    
    .row.justify-content-center.mb-4
      .col-md-7.col-lg-5
        a.anexo.mb-4(:href="obtenerLink('/downloads/Anexo2.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p 
              strong Anexo2. 
              | Guía de Implementación del Escenario
      
    .row.justify-content-center
      .col-lg-10
        figure.mb-4
          img(src='@/assets/curso/img02.svg', alt='Descripción detallada del escenario')
  
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass" scoped></style>
