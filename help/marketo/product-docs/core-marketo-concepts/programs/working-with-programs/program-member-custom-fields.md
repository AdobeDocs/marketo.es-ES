---
unique-page-id: 37355569
description: Campos personalizados de miembro del programa - Marketo Docs - Documentación del producto
title: Campos personalizados de miembro del programa
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Campos personalizados de miembro del programa {#program-member-custom-fields}

Los campos personalizados del miembro del programa le permiten recopilar datos específicos del programa para cada miembro. Pueden utilizarse en: Marketo forms, Smart List filters and déclencheur, y acciones de flujo de Smart Campaign. Los datos se pueden ver en la pestaña Miembros del programa.

>[!NOTE]
>
>Los campos personalizados de miembro del programa no tienen una integración con los campos de miembro de Salesforce Campaign en este momento.

## Crear un campo personalizado de miembro del programa {#create-a-program-member-custom-field}

1. En Marketo, haga clic en **Admin**.

   ![](assets/one.png)

1. Haga clic en **Administración de campos**.

   ![](assets/two.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/three.png)

1. Haga clic en la lista desplegable Objeto y seleccione el objeto deseado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Los campos personalizados Persona y Miembro del programa no pueden compartir el mismo nombre.

1. Complete los campos restantes y haga clic en **Create**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Los tipos compatibles con los campos personalizados de miembro del programa son: booleano, fecha, fecha, hora, flotante, entero, cadena, URL. [Obtenga más información sobre los tipos](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md) de campo.

## Descripciones de objetos {#object-descriptions}

| Objeto | Descripción |
|---|---|
| Empresa | Nombre de la empresa asociada a la persona. |
| Oportunidad | Una oportunidad puede asociarse con una persona o cuenta como una posible venta futura. Normalmente, entran en Marketo a través de un CRM o a través de una API. |
| Persona | Persona de la base de datos de Marketo con la que interactúa mediante campañas de marketing. |
| Miembro del programa | Persona que también es miembro de un programa |

## Déclencheur y filtros {#triggers-and-filters}

Puede aprovechar estos datos específicos del programa en listas inteligentes mediante [déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) o [filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## Aspectos importantes {#things-to-know}

* Los campos personalizados de miembro del programa solo están disponibles en los recursos locales. No son compatibles con Design Studio porque no hay forma de vincularlas a un programa específico.
* No se puede clonar ni mover a Design Studio un formulario (o una página de aterrizaje con un formulario) que contenga campos personalizados Miembros del programa.
* El objeto Miembro del programa puede tener hasta 20 campos personalizados. Estos campos están disponibles para cualquier programa.
* Cuando elimine un miembro de un programa, si tiene datos en el campo personalizado Miembro del programa, los datos se limpiarán de ese campo.
* Para ver los datos, haga clic en la ficha Miembros del programa y cree una vista personalizada que incluya dichos campos.
* Se admiten la importación y exportación a través de [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) y [API](https://developers.marketo.com/).
* Cuando combina dos personas, se utilizarán los datos de campo personalizados del miembro del programa del ganador. Pero si el ganador no tiene ninguno, se utilizará el valor del perdedor.

>[!MORELIKETHIS]
>
>[Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
