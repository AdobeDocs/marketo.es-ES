---
unique-page-id: 11378814
description: Obtenga información acerca de las Listas de cuentas y cómo agrupan cuentas con nombre para la segmentación. Cree listas estáticas o dinámicas desde las vistas de cuentas de CRM.
title: '[!UICONTROL Listas de cuentas]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
TQID: https://experienceleague.adobe.com/fNIkaF84ELk9RJAxA9PK9rFlaEkNwia9sbgqsHOBOMI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 364
ht-degree: 2%

---

# [!UICONTROL Listas de cuentas] {#account-lists}

Una lista de cuentas es una colección de cuentas con nombre que se pueden agrupar como destino. Las listas de cuentas le permiten segmentar cuentas con nombre por sector, ubicación o tamaño de la compañía.

Además de las listas de cuentas, también puede crear listas de cuentas dinámicas que se generan a partir de vistas de cuentas de CRM públicas. Una vista de cuenta de CRM es un conjunto de reglas que actúa como filtro al mostrar cuentas. Por ejemplo, puede usarlo para buscar cuentas en las que el sector es atención médica *y* los ingresos superan los 100 millones de dólares.

![](assets/one.png)

>[!NOTE]
>
>Las listas de cuentas creadas en Marketo [!UICONTROL Administración de cuentas de Target] están disponibles automáticamente al crear listas inteligentes y campañas web en [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Crear una nueva lista de cuentas {#create-a-new-account-list}

1. Haga clic en el menú desplegable **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Crear nueva lista de cuentas]**.

   ![](assets/1a.png)

1. Asigne un nombre a la lista y haga clic en **[!UICONTROL Crear]**.

   ![](assets/three-0.png)

1. Después de crear su lista de cuentas, comience a [agregarle cuentas con nombre](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md).

   >[!NOTE]
   >
   >Marketo solo mostrará perspectivas para listas de cuentas con 2000 cuentas con nombre o menos.

## Crear una nueva lista de cuentas dinámicas {#create-a-new-dynamic-account-list}

1. Haga clic en el menú desplegable **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Crear nueva lista dinámica]**.

   ![](assets/1.png)

1. En el cuadro de diálogo, seleccione una **Vista de cuenta de CRM** de la lista desplegable o escriba el nombre para buscarla.

   ![](assets/image2017-7-18-9-48-23.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >En Salesforce, asegúrese de proporcionar permisos de objeto de vista de lista al usuario de sincronización.

## Cambiar nombre de lista de cuentas {#rename-an-account-list}

>[!NOTE]
>
>Estos pasos solo se aplican a listas de cuentas. Las listas de cuentas *dinámicas* utilizan el nombre de sus vistas de cuentas de CRM asociadas.

1. Seleccione la cuenta cuyo nombre desea cambiar, haga clic en la lista desplegable **[!UICONTROL Acciones de lista de cuentas]** y seleccione **[!UICONTROL Cambiar nombre de lista de cuentas]**.

   ![](assets/three.png)

1. Escriba el nuevo nombre y haga clic en **[!UICONTROL Cambiar nombre]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La vista de cuenta de CRM se sincroniza con la lista de cuentas dinámicas cada 8 horas. Si aún no están sincronizados, Marketo los sincronizará durante el siguiente ciclo.

## Eliminar una lista de cuentas {#delete-an-account-list}

>[!NOTE]
>
>Estos pasos son los mismos para las listas de cuentas y las listas de cuentas dinámicas.

1. Seleccione la cuenta que desee eliminar, haga clic en la lista desplegable **[!UICONTROL Acciones de lista de cuentas]** y seleccione **[!UICONTROL Eliminar lista de cuentas]**.

   ![](assets/five.png)

1. Haga clic en **[!UICONTROL Eliminar]**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Agregar una [!UICONTROL cuenta con nombre] existente a una lista de cuentas](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Información de la lista de cuentas](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
