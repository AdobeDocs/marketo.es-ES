---
unique-page-id: 1900554
description: Edición de la documentación del producto de HTML de un correo electrónico - Documentos de Marketo
title: Editar el HTML de un correo electrónico
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 4%

---

# Editar el HTML de un correo electrónico {#edit-an-emails-html}

A veces, es posible que tenga que modificar la HTML subyacente de un correo electrónico. A veces puede utilizar un sistema externo para diseñar y crear el código del correo electrónico. En cualquier caso, puede importar o editar fácilmente código desde el editor de correo electrónico.

## Editar HTML {#edit-html}

1. Seleccione su correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/teamspidey.jpg)

1. Haga clic en **[!UICONTROL Editar código]**.

   ![](assets/two-4.png)

1. Realice los cambios necesarios. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia lo que quieras. Puede reemplazar todo el HTML o realizar ajustes menores.

1. Haga clic en la lista desplegable **[!UICONTROL Acciones de código]** para descargar el código como archivo .html, integrar el CSS o validar el HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La práctica recomendada para los correos electrónicos es hacer que todos los estilos estén en línea. Varios clientes de correo electrónico no admiten CSS en la sección `<head>`.

## Separación de un Correo Electrónico de su Plantilla {#breaking-an-email-from-its-template}

Estos cambios de código **no** separarán un correo electrónico de su plantilla:

* Edición del contenido de cualquier módulo (incluida la adición de nuevos elementos dentro del módulo)
* Adición de un nuevo módulo al contenedor
* Eliminación de un módulo del contenedor

* Cambiar atributos específicos de mkto (por ejemplo, &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) de cualquier elemento fuera de un módulo
* Editar el contenido de cualquier elemento (texto enriquecido, imagen, vídeo, etc.) fuera de un módulo

Estas acciones que puede hacer en el editor de código **separarán** el correo electrónico de su plantilla:

* Cambiar cualquier elemento del código fuera de un elemento o módulo
* Añadir o cambiar atributos que no sean mkto (por ejemplo, &quot;id&quot; o &quot;style&quot;) de cualquier elemento fuera de un módulo
* Eliminación de un elemento que está fuera de un módulo

## Código de búsqueda {#search-code}

Utilice la funcionalidad Buscar código para buscar y reemplazar contenido de forma eficaz dentro del código HTML del correo electrónico.

1. En el código del correo electrónico, haga clic en **[!UICONTROL Código de búsqueda]**.

   ![](assets/five-2.png)

1. Escriba lo que quiera encontrar y haga clic en **[!UICONTROL Buscar siguiente]** para buscar hacia adelante o en **[!UICONTROL Buscar anterior]** para buscar hacia atrás. También tiene la opción de **[!UICONTROL Reemplazar]** y **[!UICONTROL Reemplazar todo]**.

   ![](assets/six-1.png)

1. Haga clic en **[!UICONTROL Cerrar]** cuando haya terminado.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >El código de búsqueda también está disponible en [Editor de plantillas de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Le recomendamos que continúe editando los correos electrónicos con la funcionalidad integrada de Marketo, pero este editor de código proporciona flexibilidad si lo necesita.
