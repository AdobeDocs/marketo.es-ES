---
unique-page-id: 2953419
description: Uso del Editor de texto enriquecido - Marketo Docs - Documentación del producto
title: Uso del Editor de texto enriquecido
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---

# Uso del Editor de texto enriquecido {#using-the-rich-text-editor}

El Editor de texto enriquecido (RTE) aparece en todo Marketo y está disponible siempre que desee agregar o editar contenido. Verá una versión de este en páginas de aterrizaje, programas, correos electrónicos, formularios y fragmentos. Haga clic en **Editar borrador** y aparecerá para servirle.

## Configuración del editor {#editor-settings}

La configuración del elemento de bloque raíz define qué etiquetas ajustan el contenido. De forma predeterminada, el elemento de bloque raíz de correo electrónico utiliza `<p>` etiquetas. Tiene la opción de cambiarlo siguiendo los pasos a continuación.

>[!TIP]
>
>Aunque tiene la opción de elegir el elemento de bloque raíz, siempre recomendamos utilizar la configuración predeterminada para la mejor experiencia de usuario.

1. Haga clic en **Administrador**.

   ![](assets/one.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/two.png)

1. Haga clic en **Editar configuración del editor de texto**.

   ![](assets/three.png)

1. En el **Editor de correo electrónico/fragmento de código** desplegable, seleccione `<div>` o Ninguno y haga clic en **Guardar**. `<div>` en este ejemplo.

   ![](assets/four.png)

   Si tiene `<div class=“mktEditable”></div>` en una plantilla de correo electrónico, verá el siguiente comportamiento de origen de HTML al abrir la sección y escribir &quot;Texto va aquí&quot; en el editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Ninguno</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;El texto va aquí&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;El texto va aquí&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>El texto va aquí<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>También puede cambiar el elemento de bloque raíz del Editor de páginas de aterrizaje siguiendo los mismos pasos, pero haciendo clic en el botón **Editor de página de aterrizaje** en el paso 4 en lugar de Editor de correo electrónico/fragmento de código.

>[!NOTE]
>
>El elemento de bloque raíz siempre es `<p>` para tokens de programa de texto enriquecido.

## Funciones {#features}

Estas son las características que encontrará en un RTE.

| Icono | Nombre | Qué hace |
|---|---|---|
| ![--](assets/image2015-7-9-10-3a23-3a24.png) | Familia de fuentes | Elige tu estilo, ¡tenemos mucho! |
| ![--](assets/image2015-7-9-10-3a22-3a11.png) | Tamaño de fuente | ¿Qué tan grande quieres? 25 opciones, de 8 px a 90 px. |
| ![--](assets/image2015-7-9-10-3a59-3a4.png) | Estilos | Elija Párrafo o seis estilos de encabezado (para páginas de aterrizaje). |
| ![--](assets/image2015-7-9-10-3a20-3a1.png) | Interlineado | Elija la distancia entre las líneas. |
| ![--](assets/image2015-7-9-10-3a25-3a52.png) | Color del texto | Negro, rojo o lo que quieras. |
| ![--](assets/image2015-7-9-10-3a24-3a38.png) | Color de fondo | Resaltar para énfasis. |
| ![--](assets/image2015-7-9-10-3a28-3a4.png) | Negrita | **Más oscuro y más grueso**. |
| ![--](assets/image2015-7-9-10-3a29-3a1.png) | Cursiva | *Anclaje, para énfasis o presupuesto* s. |
| ![--](assets/image2015-7-9-10-3a30-3a56.png) | Subrayado | Coloca una línea debajo del texto. |
| ![--](assets/image2015-7-9-10-3a31-3a57.png) | Alineación | Utilice este menú desplegable para mostrar el texto y las imágenes. Centrarlos, elegir la alineación a la izquierda o a la derecha, o propagarlos de borde a borde con una justificación completa. |  | ![--](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Elija viñetas o números en la lista desplegable. Las viñetas son buenas con listas y números con pasos. |
| ![--](assets/image2015-7-9-10-3a38-3a0.png) | Sangría | Elija más o menos sangría. Se utiliza para párrafos o cualquier texto que desee destacar. |
| ![--](assets/image2015-7-9-10-3a38-3a58.png) | Insertar/Editar vínculo | Inserte un enlace a un sitio web u otro contenido; haga cambios en ella fácilmente. |
| ![--](assets/image2015-7-9-10-3a39-3a42.png) | Insertar/Editar imagen | Una imagen vale mil palabras. Suéltelo. Haga clic en el icono de la cámara para navegar por Design Studio. Puede colocar las imágenes una al lado de la otra. |
| ![--](assets/image2015-7-9-10-3a40-3a36.png) | Insertar token | Una herramienta potente, buena para la personalización de correo electrónico y el seguimiento de datos. Asegúrese de introducir un valor predeterminado. |
| ![--](assets/image2015-7-9-10-3a41-3a21.png) | Deshacer | ¡Vaya! Retrocedamos un paso y volvamos a intentarlo. |
| ![--](assets/image2015-7-9-10-3a42-3a13.png) | Rehacer | Si está bien, vuelva al original. |
| ![--](assets/image2015-7-9-10-3a43-3a29.png) | Tabla | Construye tu propio, como este. Un menú desplegable permite configurarlo. |
| ![--](assets/image2015-7-9-10-3a45-3a1.png) | Insertar anclaje | ¡Suelta el ancla! |
| ![--](assets/image2015-7-9-10-3a45-3a48.png) | Línea horizontal | Muchos usos: Bueno para dividir secciones. |
| ![--](assets/image2015-10-6-12-3a12-3a17.png) | Editar HTML | Abre el Editor de fuentes de HTML para que pueda modificar el código. |
| ![--](assets/image2015-7-9-10-3a47-3a36.png) | Subíndice | Letras de bajo uso (como en O)`<sub>2</sub>`). |
| ![--](assets/image2015-7-9-10-3a48-3a35.png) | Superíndice | ¡Tienes el poder! (2`<sup>6</sup>`). |
| ![--](assets/image2015-7-9-10-3a49-3a31.png) | Tachado | `<s>Put a line through text, like this</s>`. |
| ![--](assets/image2015-7-9-10-3a50-3a11.png) | Carácter especial | ¿Quieres hablar de euros? ¿Matemáticas? Tienes 243 opciones. |
| ![--](assets/image2015-7-9-10-3a52-3a26.png) | Buscar y reemplazar | Busque y cambie las cosas mucho más rápido que buscar cada instancia usted mismo. |
| ![--](assets/image2015-7-9-10-3a53-3a37.png) | Borrar formato | Devolver cosas a estándar. |
| ![--](assets/image2015-7-9-10-3a55-3a2.png) | Cancelar  | Presione el botón para decir: &quot;No importa&quot;. |
| ![--](assets/image2015-7-9-10-3a56-3a2.png) | Guardar | Presione el botón para decir, &quot;OK, me gusta&quot;. |

>[!TIP]
>
>El HTML y el texto se editan en pantallas independientes. Asegúrese de hacer clic en **Copiar desde el HTML** en el **Texto** pestaña y luego **Guardar** así que el texto coincide con su HTML.

>[!NOTE]
>
>No está limitado a las fuentes de la lista desplegable. Puede utilizar una que no aparezca en la lista si accede al código del HTML. Todas las fuentes web son compatibles con Marketo, pero las fuentes web no funcionan universalmente en todos los clientes de correo electrónico.

## Páginas de destino {#landing-pages}

La configuración del elemento de bloque raíz define qué etiquetas ajustan el contenido. De forma predeterminada, el elemento de bloque raíz de la página de aterrizaje utiliza `<div>` etiquetas. Tiene la opción de cambiarlo, siguiendo los pasos a continuación.

>[!TIP]
>
>Aunque tiene la opción de elegir el elemento de bloque raíz, siempre recomendamos utilizar la configuración predeterminada para la mejor experiencia de usuario.

1. Haga clic en **Administrador**.

   ![](assets/one.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/two.png)

1. Haga clic en **Editar configuración del editor de texto**.

   ![](assets/three.png)

1. En el **Editor de página de aterrizaje** desplegable, seleccione `<p>` o Ninguno y haga clic en **Guardar**. `<p>` en este ejemplo.

   ![](assets/five.png)

   ¡Y eso es todo!
