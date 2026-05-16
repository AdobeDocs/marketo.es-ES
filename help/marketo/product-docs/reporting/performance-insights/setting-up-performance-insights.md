---
unique-page-id: 12981145
description: Obtenga información sobre cómo configurar las perspectivas de rendimiento configurando la configuración de oportunidades, los costes de programas, el comportamiento de análisis y los criterios de éxito. Asegúrese de que la atribución y el flujo de datos sean los adecuados para generar informes precisos.
title: Configuración de perspectivas de rendimiento
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
TQID: https://experienceleague.adobe.com/xH9HG3hKoUFG3428IngBYFG6n4W3k1Bd-baVI7WTMrE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: b9f06cb0-cdf7-4b83-a9d1-a701d132779b
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 331
ht-degree: 2%

---

# Configurando [!UICONTROL Perspectivas de rendimiento] {#setting-up-performance-insights}

Siga los pasos a continuación para configurar MPI.

## Configuración de oportunidad {#opportunity-setup}

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/admin.png)

1. Haga clic en **[!UICONTROL Análisis del ciclo de ingresos]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Si no tiene RCA, tendrá que seleccionar **[!UICONTROL Análisis de programa]** para el paso 2.

1. En Atribución, haga clic en **[!UICONTROL Editar]**.

   ![](assets/three-1.png)

1. Se muestra Configuración de atribución.

   ![](assets/four-2.png)

   Si la Atribución es explícita, asegúrese de que la Función de contacto de oportunidad se haya rellenado (a través del punto de conexión de la Función de oportunidad o a través de la integración de CRM).

   Si la Atribución está implícita, asegúrese de que el campo de empresa del posible cliente/contacto sea el mismo que el Nombre de cuenta de la oportunidad.

   >[!NOTE]
   >
   >Asegúrese de que todas las oportunidades tengan los campos adecuados rellenados:
   >
   >* [!UICONTROL Importe de oportunidad]
   >* [!UICONTROL Está Cerrado]
   >* [!UICONTROL Ha Ganado]
   >* [!UICONTROL Fecha de creación] (no se puede establecer en su caso)
   >* [!UICONTROL Fecha de cierre] (puede que no se haya establecido en su caso)
   >* [!UICONTROL Tipo de oportunidad]

## Configuración del programa {#program-setup}

Actualice los costes del programa durante al menos 12 meses. Puede hacerlo manualmente o mediante la API del programa. En este ejemplo lo hacemos manualmente.

1. Haga clic en **[!UICONTROL Actividades de marketing]**.

   ![](assets/ma.png)

1. Busque y seleccione su programa.

   ![](assets/select-program.png)

1. Haga clic en la ficha **[!UICONTROL Configuración]**.

   ![](assets/setup-tab.png)

1. Arrastre **[!UICONTROL Costo de período]** al lienzo.

   ![](assets/period-cost.png)

1. Establezca el mes del programa como mínimo hace 12 meses y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/set-period.png)

1. Establezca el costo del período y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/set-cost.png)

A continuación, revise el comportamiento de Analytics para indicar si algún canal en particular debe incluirse en Analytics. Establezca el Comportamiento de Analytics (Normal, Inclusivo, Operativo).

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/admin.png)

1. Haga clic en **[!UICONTROL Etiquetas]**.

   ![](assets/tags.png)

1. Haga clic en **+** para expandir la lista de canales.

   ![](assets/channel.png)

1. Haga doble clic en el canal deseado.

   ![](assets/channel-click.png)

1. Haga clic en el menú desplegable **[!UICONTROL Comportamiento de Analytics]** y seleccione el comportamiento que desee.

   ![](assets/edit-channel.png)

1. Defina los criterios de éxito.

   ![](assets/success.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/save.png)

## Vinculación del programa a la persona {#tie-the-program-to-the-person}

1. Asegúrese de que el programa de adquisición y la fecha de adquisición se hayan establecido para cada persona de la base de datos para que funcione la Atribución de primer contacto.
1. Asegúrese de que los programas establezcan estados de éxito para sus recursos.

>[!NOTE]
>
>Los cambios realizados no son instantáneos. Se requiere un período de un día para que los cambios entren en vigor.
