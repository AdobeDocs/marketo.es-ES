---
unique-page-id: 2953419
description: Uso del editor de texto enriquecido - Documentos de Marketo - Documentación del producto
title: Uso del editor de texto enriquecido
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 2%

---

# Uso del editor de texto enriquecido {#using-the-rich-text-editor}

El Editor de texto enriquecido (RTE) aparece en Marketo y está disponible siempre que desee agregar o editar contenido. Verá una versión en páginas de aterrizaje, programas, correos electrónicos, formularios y fragmentos de código. Simplemente haz clic en **[!UICONTROL Editar borrador]** y aparecerá para servirte.

## Configuración de editor {#editor-settings}

La configuración del elemento de bloque raíz define qué etiquetas ajustan el contenido. De manera predeterminada, el elemento de bloque raíz del correo electrónico utiliza etiquetas `<p>`. Tiene la opción de cambiar esto siguiendo los pasos a continuación.

>[!TIP]
>
>Aunque tiene la opción de elegir el elemento de bloque raíz, siempre recomendamos utilizar la configuración predeterminada para mejorar la experiencia del usuario.

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Editar configuración del editor de texto]**.

   ![](assets/three.png)

1. En el menú desplegable **[!UICONTROL Correo electrónico] / [!UICONTROL Editor de fragmentos]**, seleccione `<div>` o [!UICONTROL Ninguno] y haga clic en **[!UICONTROL Guardar]**. `<div>` se usa en este ejemplo.

   ![](assets/four.png)

   Si tiene `<div class=“mktEditable”></div>` en una plantilla de correo electrónico, verá el siguiente comportamiento de HTML Source al abrir la sección y escribir &quot;El texto va aquí&quot; en el editor:

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>Ninguna</th>
  </tr>
  <tr>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;El texto está aquí&lt;/p&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;El texto está aquí&lt;/div&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>El texto va aquí<br>&lt;/div&gt;</p></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>También puede cambiar el elemento de bloque raíz del Editor de la página de aterrizaje si sigue los mismos pasos, pero hace clic en la lista desplegable **[!UICONTROL Editor de página de aterrizaje]** en el paso 4 en lugar de [!UICONTROL Correo electrónico] / [!UICONTROL Editor de fragmentos].

>[!NOTE]
>
>El elemento de bloque raíz siempre es `<p>` para tokens de programa de texto enriquecido.

## Funciones {#features}

Estas son las funciones que encontrará en un RTE.

| Ícono | Nombre | Qué hace |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Familia de fuentes] | Elige tu estilo, ¡tenemos mucho! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Tamaño de fuente] | ¿Qué tan grande lo quieres? 25 opciones, de 8 px a 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Estilos] | Elija Párrafo o seis estilos de encabezado (para páginas de aterrizaje). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Interlineado] | Elige la distancia entre las líneas. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Color de texto] | Negro, rojo o lo que quieras. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Color de fondo] | Resaltar para dar énfasis. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Negrita] | **Más oscuro y grueso**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Cursiva] | *En ángulo, para énfasis o presupuesto* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Subrayado] | Pone una línea debajo del texto. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alineación] | Utilice este menú desplegable para diseñar el texto y las imágenes. Centrarlos, elegir la alineación a la izquierda o a la derecha, o extenderlos de borde a borde con justificación completa. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Elija viñetas o números en la lista desplegable. Las viñetas son buenas con las listas y los números con pasos. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Sangría] | Elija más o menos sangría. Utilícelo para párrafos o cualquier texto que desee destacar. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Insertar/Editar vínculo] | Coloque un vínculo a un sitio web u otro contenido; realice fácilmente cambios en él. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Insertar/Editar imagen] | Una imagen vale más que mil palabras. Coloca uno. Haga clic en el icono de la cámara para explorar Design Studio. Puede colocar imágenes en paralelo. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Insertar token] | Una herramienta potente, ideal para la personalización del correo electrónico y el seguimiento de datos. Asegúrese de introducir un valor predeterminado. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Deshacer] | ¡Uy! Vamos a retroceder un paso y volver a intentarlo. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Rehacer] | Si realmente funciona correctamente, vuelva al original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Tabla] | Construye tu propio, como éste. Un menú desplegable le permite configurarlo. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Insertar anclaje] | ¡Suelta el ancla! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Línea horizontal] | Muchos usos: ideal para dividir secciones. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Editar HTML] | Abre el Editor de Source de HTML para que puedas modificar tu código. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Subíndice] | Letras de cuelgue bajo (como en O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Superíndice] | ¡Tienes el poder! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Tachado] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Carácter especial] | ¿Quieres hablar de euros? ¿Matemáticas? Tienes 243 opciones. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Buscar y reemplazar] | Busque y cambie cosas mucho más rápido que buscando cada instancia usted mismo. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Borrar formato] | Devuelva las cosas al estándar. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Cancelar] | Presione el botón para decir: &quot;No importa&quot;. |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Guardar] | Presione el botón para decir: &quot;OK, me gusta&quot;. |

>[!TIP]
>
>El HTML y el texto se editan en pantallas independientes. Asegúrate de hacer clic en **[!UICONTROL Copiar de HTML]** en la ficha **[!UICONTROL Texto]** y, a continuación, **[!UICONTROL Guardar]** para que el texto coincida con tu HTML.

>[!NOTE]
>
>No está limitado a las fuentes de la lista desplegable. Puede utilizar uno que no aparezca en la lista accediendo al código HTML. Todas las fuentes web son compatibles con Marketo, pero las fuentes web no funcionan de forma universal en todos los clientes de correo electrónico.

## Páginas de destino {#landing-pages}

La configuración del elemento de bloque raíz define qué etiquetas ajustan el contenido. De manera predeterminada, el elemento de bloque raíz de la página de aterrizaje utiliza etiquetas `<div>`. Tiene la opción de cambiar esto siguiendo los pasos a continuación.

>[!TIP]
>
>Aunque tiene la opción de elegir el elemento de bloque raíz, siempre recomendamos utilizar la configuración predeterminada para mejorar la experiencia del usuario.

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Editar configuración del editor de texto]**.

   ![](assets/three.png)

1. En la lista desplegable **[!UICONTROL Editor de página de aterrizaje]**, seleccione `<p>` o [!UICONTROL Ninguno] y haga clic en **[!UICONTROL Guardar]**. `<p>` se usa en este ejemplo.

   ![](assets/five.png)

   ¡Y eso es todo!
