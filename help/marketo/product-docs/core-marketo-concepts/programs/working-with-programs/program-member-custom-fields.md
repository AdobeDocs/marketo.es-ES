---
unique-page-id: 37355569
description: Campos personalizados de miembro del programa - Documentos de Marketo - Documentación del producto
title: Campos personalizados de miembro del programa
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 56f429dabf19c4425c68b0dcd745621681a038ae
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 1%

---

# Campos personalizados de miembro del programa {#program-member-custom-fields}

Los campos personalizados del miembro del programa le permiten recopilar datos específicos del programa para cada miembro. Pueden utilizarse en: Marketo forms, déclencheur y filtros de listas inteligentes y acciones de flujo de campañas inteligentes. Los datos se pueden ver en la pestaña Miembros del programa.

>[!NOTE]
>
>Los campos personalizados de miembro del programa no tienen una integración con los campos de miembro de Salesforce Campaign en este momento.

## Crear un campo personalizado de miembro del programa {#create-a-program-member-custom-field}

1. En Marketo, haga clic en **Administrador**.

   ![](assets/one.png)

1. Haga clic en **Gestión de las actividades sobre el terreno**.

   ![](assets/two.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/three.png)

1. Haga clic en la lista desplegable Objeto y seleccione el objeto deseado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Los campos personalizados Persona y Miembro del programa no pueden compartir el mismo nombre.

1. Complete los campos restantes y haga clic en **Crear**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Los tipos compatibles con los campos personalizados de miembro del programa son: booleano, fecha, fecha, hora, flotante, entero, cadena, URL. [Más información sobre los tipos de campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target=&quot;_blank&quot;}.

## Descripciones de objetos {#object-descriptions}

| Objeto | Descripción |
|---|---|
| Compañía | Nombre de la empresa asociada a la persona. |
| Oportunidad | Una oportunidad puede asociarse con una persona o cuenta como una posible venta futura. Normalmente entran en Marketo a través de un CRM o mediante una API. |
| Persona | Persona de la base de datos de Marketo con la que interactúa mediante campañas de marketing. |
| Miembro del programa | Persona que también es miembro de un programa |

## Déclencheur y filtros {#triggers-and-filters}

Puede aprovechar estos datos específicos del programa en listas inteligentes mediante [déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target=&quot;_blank&quot;} y/o [filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target=&quot;_blank&quot;}.

![](assets/six.png)

## Aspectos importantes {#things-to-know}

* Los campos personalizados de miembro del programa solo están disponibles en los recursos locales. No son compatibles con Design Studio porque no hay forma de vincularlas a un programa específico.
* No se puede clonar ni mover a Design Studio un formulario (o una página de aterrizaje con un formulario) que contenga campos personalizados Miembros del programa.
* El objeto Miembro del programa puede tener hasta 20 campos personalizados. Estos campos están disponibles para cualquier programa.
* Cuando elimine un miembro de un programa, si tiene datos en el campo personalizado Miembro del programa, los datos se limpiarán de ese campo.
* Para ver los datos, haga clic en la ficha Miembros del programa y cree una vista personalizada que incluya dichos campos.
* Importar y exportar mediante [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target=&quot;_blank&quot;} y [API](https://developers.marketo.com/)Se admiten {target=&quot;_blank&quot;}. Las exportaciones solo funcionan en listas de miembros del programa, no en listas estáticas.
* Cuando combina dos personas, se utilizarán los datos de campo personalizados del miembro del programa del ganador. Pero si el ganador no tiene ninguno, se utilizará el valor del perdedor.
* El tipo de cambio no está permitido en los campos Información de miembro del programa .
* La restricción &quot;contiene&quot; lista inteligente no es compatible con los campos personalizados de miembro del programa.

>[!MORELIKETHIS]
>
>[Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;}
