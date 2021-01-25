---
unique-page-id: 37355569
description: Campos personalizados de miembros de programa - Documentos de marketing - Documentación del producto
title: Campos personalizados de miembros de programa
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Campos personalizados de miembros de programa {#program-member-custom-fields}

Los campos personalizados de miembros de programa permiten recopilar datos específicos de programa para cada miembro. Pueden utilizarse en: Formularios de marketing, filtros y déclencheur de Listas inteligentes y acciones de flujo de Campañas inteligentes. Los datos se pueden ver en la ficha Miembros del programa.

## Crear un campo personalizado de miembro de Programa {#create-a-program-member-custom-field}

1. En Marketing, haga clic en **Administración**.

   ![](assets/one.png)

1. Haga clic en **Administración de campos**.

   ![](assets/two.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/three.png)

1. Haga clic en la lista desplegable Objeto y seleccione el objeto deseado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Los campos personalizados Persona y Miembro de Programa no pueden compartir el mismo nombre.

1. Complete los campos restantes y haga clic en **Crear**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Los tipos admitidos para los campos personalizados de Miembros de Programa son: booleano, fecha, fecha y hora, flotante, entero, cadena, URL. [Obtenga más información sobre los tipos](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md) de campo.

## Descripciones de objetos {#object-descriptions}

| Objeto | Descripción |
|---|---|
| Compañía | Nombre de la compañía asociada a la persona. |
| Oportunidad | Una oportunidad puede asociarse con una persona o cuenta como una posible venta futura. Normalmente, entran en Marketing a través de una CRM o de una API. |
| Persona | Persona de la base de datos de Marketing con la que interactúa mediante campañas de marketing. |
| Miembro programa | Persona que también es miembro de un programa |

## Déclencheur y Filtros {#triggers-and-filters}

Puede aprovechar estos datos específicos del programa en listas inteligentes mediante [déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) y/o [filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## Cosas que hay que saber {#things-to-know}

* Los campos personalizados de miembros de programa solo están disponibles en los recursos locales. No son compatibles con Design Studio porque no hay forma de vincularlos a un programa específico.
* No se puede clonar ni mover a Design Studio un formulario (o una página de aterrizaje con un formulario) que contenga campos personalizados Miembros de Programa.
* Los campos personalizados de miembros de programa no se pueden usar como tokens.
* El objeto Miembro de Programa puede tener hasta 20 campos personalizados. Estos campos están disponibles para cualquier programa.
* Cuando elimina un miembro de un programa, si tiene datos en el campo personalizado Miembro del Programa, los datos se eliminarán de ese campo.
* Para vista de los datos, haga clic en la ficha Miembros del programa y cree una vista personalizada que incluya dichos campos.
* Se admiten la importación y exportación mediante [lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)y [API](https://developers.marketo.com/).
* Cuando combina dos personas, se utilizarán los datos de campo personalizados de miembro de Programa del ganador. Pero si el ganador no tiene ninguno, se utilizará el valor del perdedor.

>[!MORELIKETHIS]
>
>[Creación de un campo personalizado en Marketing](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
