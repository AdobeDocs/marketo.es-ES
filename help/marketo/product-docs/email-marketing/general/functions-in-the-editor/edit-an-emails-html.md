---
unique-page-id: 1900554
description: Editar el HTML de un mensaje de correo electrónico - Documentos de marketing - Documentación del producto
title: Editar el HTML de un correo electrónico
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Editar el HTML {#edit-an-emails-html} de un mensaje de correo electrónico

A veces es posible que necesite modificar el HTML subyacente de un correo electrónico. A veces puede utilizar un sistema externo para diseñar y generar el código de su correo electrónico. De cualquier forma, puede importar y/o editar código fácilmente desde el editor de correo electrónico.

## Editar HTML {#edit-html}

1. Seleccione su correo electrónico y haga clic en **Editar borrador**.

   ![](assets/teamspidey.jpg)

1. Haga clic en **Editar código**.

   ![](assets/two-4.png)

1. Realice cualquier cambio. Haga clic en **Guardar** cuando termine.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia lo que quieras. Puede reemplazar todo el HTML o realizar ajustes menores.

1. Haga clic en la lista desplegable **Acciones de código** para descargar el código como archivo .html, en línea con su CSS o validar el HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La práctica recomendada para los correos electrónicos es poner todos los estilos en línea. Varios clientes de correo electrónico no admiten CSS en la sección `<head>`.

## Romper un correo electrónico de su plantilla {#breaking-an-email-from-its-template}

Estos cambios en el código **no harán** romper un correo electrónico de su plantilla:

* Edición del contenido de cualquier módulo (incluida la adición de nuevos elementos dentro del módulo)
* Añadir un nuevo módulo al Contenedor
* Eliminación de un módulo del Contenedor

* Cambiar atributos específicos de mkto (por ejemplo, &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) de cualquier elemento fuera de un módulo
* Edición del contenido de cualquier elemento (texto enriquecido, imagen, vídeo, etc.) fuera de un módulo

Estas cosas que puede hacer en el editor de código **provocarán** la interrupción del correo electrónico de su plantilla:

* Cambio de cualquier elemento del código fuera de un elemento o módulo
* Añadir o cambiar atributos que no sean mkto (por ejemplo, &quot;id&quot; o &quot;estilo&quot;) de cualquier elemento fuera de un módulo
* Eliminación de un elemento que está fuera de un módulo

## Código de búsqueda {#search-code}

Utilice la funcionalidad Código de búsqueda para buscar y reemplazar de forma eficaz el contenido del código HTML del correo electrónico.

1. En el código de su correo electrónico, haga clic en **Buscar código**.

   ![](assets/five-2.png)

1. Escriba lo que desee encontrar y haga clic en **Buscar siguiente** para buscar hacia adelante o **Buscar anterior** para buscar hacia atrás. También tiene la opción de **Reemplazar** y **Reemplazar todo**.

   ![](assets/six-1.png)

1. Haga clic en **Cerrar** cuando termine.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >El código de búsqueda también está disponible en el [editor de plantillas de correo electrónico](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template).

Le recomendamos que continúe editando sus correos electrónicos utilizando la funcionalidad integrada de Marketing, pero este editor de código proporciona flexibilidad si lo necesita.
