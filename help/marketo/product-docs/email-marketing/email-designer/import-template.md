---
solution: Marketo Engage
product: marketo
title: Importación de plantilla
description: Obtenga información sobre cómo importar las plantillas de correo electrónico existentes del editor clásico al nuevo Designer de correo electrónico.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f5f5e256631b09937d97d7b70f9475f2c286676d
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Importación de plantilla {#template-import}

Importe sin problemas sus plantillas de correo electrónico existentes del editor clásico al nuevo Designer de correo electrónico, preservando sus diseños y acelerando la creación de plantillas con estructuras familiares y reutilizables.

1. Vaya a **Design Studio**.

   CAPTURA DE PANTALLA

1. Haga clic en **Plantillas de correo electrónico** y seleccione **Plantillas de correo electrónico (nuevas)**.

   CAPTURA DE PANTALLA

1. Haga clic en **Crear plantilla**.

   CAPTURA DE PANTALLA

1. Escriba un _Nombre_ y (opcional) _Descripción_.

   CAPTURA DE PANTALLA

1. Haga clic en **Plantillas Marketo** y elija las Plantillas existentes creadas en el editor de correo electrónico clásico.

   CAPTURA DE PANTALLA

   >[!NOTE]
   >
   >Solo se pueden importar las plantillas aprobadas y las que se han compartido con el espacio de trabajo actual.

1. Seleccione la plantilla que desee.

   CAPTURA DE PANTALLA

1. Haga clic en Use this template.

   CAPTURA DE PANTALLA

1. La plantilla importada se abre en el Designer de correo electrónico.

1. Revise los componentes para la conversión correcta y realice los ajustes necesarios con Designer. Cuando esté satisfecho con la plantilla, apruébela para usarla en correos electrónicos.

## Creación de fragmentos {#create-fragments}

Es aconsejable crear fragmentos de secciones repetibles para usarlos más adelante.

1. Haga clic en el botón **...Más** de la parte superior y seleccione **Guardar como fragmento**.

   CAPTURA DE PANTALLA

1. Seleccione un componente o una estructura y haga clic en **Crear**.

   CAPTURA DE PANTALLA

1. Escriba un nombre (y una descripción opcional) y haga clic en **Guardar**.

   CAPTURA DE PANTALLA

## Prácticas recomendadas {#best-practices}

* Dado que Freestyle HTML puede variar significativamente, es posible que el importador no siempre interprete todos los componentes a la perfección. Revise las plantillas importadas para asegurarse de que todas las secciones se puedan editar y asignar correctamente. Si un artículo no se puede seleccionar, simplemente vuelva a crear esa sección para obtener los mejores resultados.

* Después de la importación, puede guardar secciones reutilizables como fragmentos y aprobarlas para que las utilicen los autores de correo electrónico. Aplique temas de marca para mantener la coherencia y el cumplimiento.

* Puede seguir utilizando scripts de Velocity y considerar la posibilidad de volver a implementar fragmentos más antiguos mediante una combinación de fragmentos y contenido condicional para mejorar la flexibilidad y el control.

<table><thead>
  <tr>
    <th>Limitación</th>
    <th>Razón</th>
    <th>Solución</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Las variables definidas en el editor de correo electrónico clásico no están disponibles en el nivel de correo electrónico.</td>
    <td>Las variables se diseñaron originalmente para simplificar la edición por correo electrónico cuando el editor aún no ofrecía funciones de WYSIWYG. En Email Designer, los usuarios pueden lograr una flexibilidad similar a través de los controles disponibles. El importador mantiene la estructura y los componentes de la plantilla existente, lo que le ayuda a recrearla de forma eficaz en el Designer de correo electrónico.</td>
    <td>Los usuarios deben poder conseguirlo en Designer. <p>
    Para los módulos, puede guardar diferentes segmentos como fragmentos. Los fragmentos aprobados estarán disponibles para su uso en el nivel de correo electrónico.</td>
  </tr>
  <tr>
    <td>Si la HTML de origen contiene bloques anidados, las capas más profundas no se pueden dirigir en Designer.</td>
    <td>El Designer de correo electrónico no admite comentarios anidados.</td>
    <td>Aunque Designer no permite la edición de estructuras anidadas, debe procesarse con precisión. Asegúrese de probar primero la plantilla.<p>
    Vuelva a crear la estructura mediante Cuadrícula.</td>
  </tr>
  <tr>
    <td>A veces, los botones se importan como contenedores simples con texto dentro.</td>
    <td>Algunos de los estilos de implementación que utilizan HTML se pueden malinterpretar durante la importación.</td>
    <td>Vuelva a crear el botón en Designer.</td>
  </tr>
  <tr>
    <td>Los botones pueden ser a veces demasiado grandes.</td>
    <td>Conflicto entre el CSS del correo electrónico de Marketo con otros elementos de nivel inferior (<code>&lt;span&gt;</code>)</td>
    <td>Intente ajustar los márgenes y el relleno del botón en Designer.</td>
  </tr>
  <tr>
    <td>Los puntos de viñeta no se admiten de forma nativa.</td>
    <td>Email Designer no ofrece puntos de viñeta en este momento.</td>
    <td>Considere volver a implementar las viñetas mediante técnicas alternativas.</td>
  </tr>
  <tr>
    <td>La alineación vertical se distorsiona cuando el contenido del contenedor no respeta el valor del atributo valign.</td>
    <td><code>valign</code> no funciona dentro de los contenedores definidos en la plantilla.</td>
    <td>Intente ajustar los márgenes y el relleno del botón en el Designer de correo electrónico.</td>
  </tr>
  <tr>
    <td>Los tokens Personalization de nivel de programa (Mis tokens) en el nivel de plantilla pueden encontrar errores de validación.</td>
    <td>Las plantillas de correo electrónico no admiten tokens de nivel de programa.</td>
    <td>Sustitúyalos por otros tipos de token dentro de las plantillas y reemplácelos por Mis tokens dentro de los correos electrónicos individuales.</td>
  </tr>
  <tr>
    <td>Es posible que los componentes divisores no se puedan seleccionar.</td>
    <td>Los componentes divisores no se tratan en la versión.</td>
    <td>N/A</td>
  </tr>
  <tr>
    <td>Si el HTML original tiene estructuras mal formadas, es probable que se transfieran.</td>
    <td>Problemas con el HTML original.</td>
    <td>Los problemas deberían solucionarse antes de la importación.</td>
  </tr>
  <tr>
    <td>Para el contenido importado, el uso de la previsualización de contenido no es un indicador fiable.</td>
    <td>La función de vista previa de Designer no admite HTML personalizado.</td>
    <td>Se recomienda probar el correo electrónico con la opción <b>Enviar prueba</b> en la pantalla <i>Simular contenido</i>.</td>
  </tr>
  <tr>
    <td>Los fragmentos de la plantilla antigua no funcionarán en el Designer de correo electrónico.</td>
    <td>El Designer de correo electrónico no admite fragmentos.</td>
    <td>Vuelva a implementar los fragmentos como fragmentos asociados con contenido condicional.</td>
  </tr>
</tbody></table>
