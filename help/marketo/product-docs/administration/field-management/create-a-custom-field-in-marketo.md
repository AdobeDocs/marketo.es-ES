---
unique-page-id: 2360287
description: Pasos para crear un nuevo campo personalizado en Marketo Engage para almacenar y capturar datos de personas o empresas.
title: Creación de un campo personalizado en Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
TQID: https://experienceleague.adobe.com/xdG07VzIcNYcqCsR3wfXHTGE07nsLYAvbM8QZZJf0oo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 203
ht-degree: 9%

---

# Creación de un campo personalizado en Marketo {#create-a-custom-field-in-marketo}

Obtenga información sobre cómo crear un campo personalizado en Marketo Engage para almacenar y capturar datos.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. Haga clic en **[!UICONTROL Administración de campos]**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >Si desea que los campos se mantengan sincronizados con su CRM, créelos en el CRM y se crearán automáticamente en Marketo.

1. Haga clic en **[!UICONTROL Nuevo campo personalizado]**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. Elija _[!UICONTROL Objeto]_.

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >Aunque no puede seleccionar el objeto _Company_ usted mismo, puede solicitarlo poniéndose en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

1. Elija el campo _[!UICONTROL Type]_. Esto cambiará la forma en que se procesa en las listas inteligentes y en los formularios de Marketo.

   >[!TIP]
   >
   >Consulte el [Glosario de tipos de campos personalizados](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. Escriba _[!UICONTROL Name]_ tal como desea que aparezca en Marketo (el _[!UICONTROL Nombre de API]_ se genera automáticamente). Elija con cuidado, ya que no se puede cambiar el nombre después de guardar. Haga clic en **[!UICONTROL Crear]** cuando haya terminado.

>[!CAUTION]
>
>Los nombres de campo no pueden comenzar con los siguientes caracteres: **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>El nombre de la API lo utilizan la API de SOAP y otros procesos backend.

Ahora puede utilizar este campo personalizado en formularios, pasos de flujo y listas inteligentes.
