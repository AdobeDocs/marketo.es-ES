---
unique-page-id: 37355569
description: Obtenga información sobre los campos personalizados de miembros del programa. Almacene y utilice datos personalizados de cada persona en un programa.
title: Campos personalizados del miembro del programa
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
TQID: https://experienceleague.adobe.com/77kJb3iO-IaaAQwYcAcXvzBCe1Y18qSEeJ9GXd-Fw38
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 436
ht-degree: 5%

---

# Campos personalizados del miembro del programa {#program-member-custom-fields}

Los campos personalizados de miembro de programa permiten recopilar datos específicos del programa para cada miembro. Se pueden utilizar en: formularios Marketo Forms, déclencheur y filtros de listas inteligentes y acciones de flujo de campañas inteligentes. Los datos se pueden ver en la pestaña Miembros del programa.

## Crear un campo personalizado de miembro de programa {#create-a-program-member-custom-field}

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Administración de campos]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Nuevo campo personalizado]**.

   ![](assets/three.png)

1. Haga clic en el menú desplegable **[!UICONTROL Objeto]** y seleccione el objeto que desee.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Los campos personalizados [!UICONTROL Persona] y [!UICONTROL Miembro del programa] no pueden compartir el mismo nombre.

1. Rellene los campos restantes y haga clic en **[!UICONTROL Crear]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Los tipos compatibles con los campos personalizados [!UICONTROL Miembro de programa] son: booleano, fecha, fecha y hora, flotante, entero, cadena y dirección URL. [Más información sobre los tipos de campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Descripciones de objetos {#object-descriptions}

| Objeto | Descripción |
|---|---|
| Compañía | El nombre de la compañía asociada con la persona. |
| Oportunidad | Una oportunidad se puede asociar a una persona o cuenta como una venta futura potencial. Normalmente, entran en Marketo a través de un CRM o de una API. |
| Persona | Persona de la base de datos de Marketo con la que participa mediante campañas de marketing. |
| Miembro del programa | Persona que también es miembro de un programa |

## Déclencheur y filtros {#triggers-and-filters}

Puede aprovechar estos datos específicos del programa en listas inteligentes mediante [déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} o [filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}.

![](assets/six.png)

## Cosas que debe saber {#things-to-know}

* Los campos personalizados de miembro de programa solo están disponibles en los recursos locales. No son compatibles con Design Studio porque no hay forma de vincularlos a un programa específico.
* No se puede clonar ni mover a Design Studio un formulario (o una página de aterrizaje con un formulario) que contenga campos personalizados de miembro de programa.
* [Puede sincronizar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} los campos personalizados del miembro del programa con los campos personalizados del miembro de la campaña.
* El objeto Miembro de programa puede tener hasta 20 campos personalizados. Estos campos están disponibles para cualquier programa.
* Cuando se quita un miembro de un programa, si tiene datos en el campo personalizado Miembro del programa, los datos se eliminan de ese campo.
* Para ver los datos, haga clic en la pestaña Miembros del programa y cree una vista personalizada que incluya dichos campos.
* Se admiten la importación y exportación mediante [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} y [API](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/home){target="_blank"}. Las exportaciones solo funcionan en listas de miembros de programa, no en listas estáticas.
* Cuando combina dos personas, se utilizan los datos del campo personalizado Miembro del programa del ganador. Pero si el ganador no tiene ninguno, se utilizará el valor del perdedor.
* No se permite cambiar el tipo en los campos Información de miembro del programa.
* La restricción &quot;contiene&quot; de la lista inteligente no es compatible con los campos personalizados de miembro de programa.

>[!MORELIKETHIS]
>
>* [Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Sincronización de campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
