---
unique-page-id: 1900554
description: 'Edición del HTML de un correo electrónico: documentos de Marketo, documentación del producto'
title: Editar el HTML de un correo electrónico
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Editar el HTML de un correo electrónico {#edit-an-emails-html}

A veces, es posible que tenga que modificar el HTML subyacente de un correo electrónico. A veces puede utilizar un sistema externo para diseñar y crear el código del correo electrónico. En cualquier caso, puede importar o editar fácilmente código desde el editor de correo electrónico.

## Editar HTML {#edit-html}

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/teamspidey.jpg)

1. Clic **Editar código**.

   ![](assets/two-4.png)

1. Realice los cambios necesarios. Clic **Guardar** cuando termine.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia lo que quieras. Puede reemplazar todo el HTML o realizar ajustes menores.

1. Haga clic en **Acciones de código** para descargar el código como archivo .html, integrar el CSS o validar el HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La práctica recomendada para los correos electrónicos es hacer que todos los estilos estén en línea. Varios clientes de correo electrónico no admiten CSS dentro de `<head>` sección.

## Separación de un Correo Electrónico de su Plantilla {#breaking-an-email-from-its-template}

Estos cambios de código **no** romper un correo electrónico de su plantilla:

* Edición del contenido de cualquier módulo (incluida la adición de nuevos elementos dentro del módulo)
* Adición de un nuevo módulo al contenedor
* Eliminación de un módulo del contenedor

* Cambiar atributos específicos de mkto (por ejemplo, &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) de cualquier elemento fuera de un módulo
* Edición del contenido de cualquier elemento (texto enriquecido, imagen, vídeo, etc.) fuera de un módulo

Estas cosas se pueden hacer en el editor de código **testamento** separe el correo electrónico de su plantilla:

* Cambiar cualquier elemento del código fuera de un elemento o módulo
* Añadir o cambiar atributos que no sean mkto (por ejemplo, &quot;id&quot; o &quot;style&quot;) de cualquier elemento fuera de un módulo
* Eliminación de un elemento que está fuera de un módulo

## Código de búsqueda {#search-code}

Utilice la funcionalidad Buscar código para buscar y reemplazar contenido de forma eficaz dentro del código de HTML del correo electrónico.

1. En el código del correo electrónico, haga clic en **Código de búsqueda**.

   ![](assets/five-2.png)

1. Introduzca lo que desee buscar y haga clic en **Buscar siguiente** para buscar hacia delante o **Buscar anterior** para buscar hacia atrás. También tiene la opción de **Reemplazar** y **Reemplazar todo**.

   ![](assets/six-1.png)

1. Clic **Cerrar** cuando termine.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >El código de búsqueda también está disponible en la [Editor de plantillas de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Le recomendamos que continúe editando los correos electrónicos con la funcionalidad integrada de Marketo, pero este editor de código proporciona flexibilidad si lo necesita.
