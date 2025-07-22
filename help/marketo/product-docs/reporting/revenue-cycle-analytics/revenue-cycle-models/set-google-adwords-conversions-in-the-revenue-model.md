---
unique-page-id: 6095029
description: Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos - Documentos de Marketo - Documentación del producto
title: Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Establecer conversiones de [!DNL Google AdWords] en el modelo de ingresos {#set-google-adwords-conversions-in-the-revenue-model}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], podrá ver fácilmente qué clics resultaron en posibles clientes, oportunidades y clientes nuevos calificados (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en [!DNL AdWords].

>[!NOTE]
>
>Se trata de una integración de inserción de Marketo a [!DNL Google AdWords]. Los datos de conversión aparecerán _solamente_ en el portal [!DNL Google AdWords], _no en la interfaz de usuario de Marketo_.

Más información sobre la [característica de importación de conversión sin conexión de Google](https://support.google.com/adwords/answer/2998031?hl=en). Asigne [!DNL AdWords] conversiones sin conexión a una o más etapas en un modelo de ingresos. Existen tres formas de realizar la asignación:

* Conversión de [!DNL AdWords]
* Fase de acción
* Asignación de [!DNL AdWords]

Puede crear una nueva conversión sin conexión de [!DNL AdWords] desde Marketo si usa la acción de ensayo.

>[!PREREQUISITES]
>
>[Agregar [!DNL Google AdWords] como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usar conversión [!DNL AdWords] {#use-adwords-conversion}

1. Vaya al área de **[!UICONTROL Analytics]**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Seleccione un modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Seleccione la etapa de ingresos que desee asignar a una conversión de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Seleccione la **[!UICONTROL conversión de AdWords]** que desee asignar a su fase de Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   ¡Bonito! Los datos de conversión de [!DNL AdWords] se cargarán en [!DNL Google AdWords] a la cadencia seleccionada.

## Usar acción de escenario {#use-stage-action}

También puede asignar una [!UICONTROL Conversión de AdWords] en **[!UICONTROL Acciones de ensayo]**.

1. Seleccione el paso que desea asignar a una conversión de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En el menú desplegable **[!UICONTROL Acciones de ensayo]**, seleccione **[!UICONTROL Definir conversión de AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione una **[!UICONTROL conversión de AdWords]**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Sugerencia**: Si no tiene ninguna conversión de [!DNL AdWords], cree una haciendo clic en **[!UICONTROL +Nueva conversión]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Cuando haya terminado de asignar todas las conversiones de [!DNL AdWords] a las fases de ingresos, vuelva a la página de resumen. Seleccione **[!UICONTROL Acciones de modelo]** y elija **[!UICONTROL Aprobar etapas]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Sugerencia profesional: Añada una nueva conversión {#pro-tip-add-a-new-conversion}

¡Consejo profesional! Se puede crear una nueva conversión sin conexión de [!DNL AdWords] desde Marketo.

>[!CAUTION]
>
>Las nuevas conversiones creadas desde Marketo tienen activada la configuración de &quot;optimización&quot;. Esto significa que se permite que [!DNL AdWords] estrategias de oferta optimicen sus ofertas para esas conversiones. Puede cambiar esta configuración desde su cuenta de [!DNL AdWords].

1. En el menú desplegable **[!UICONTROL Acciones de ensayo]**, seleccione **[!UICONTROL Definir conversión de AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione **[!UICONTROL Nueva conversión]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Escriba un **[!UICONTROL Nombre de conversión]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de [!DNL AdWords].

## Usar asignación [!DNL AdWords] {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con su [!UICONTROL conversión de AdWords] en un solo lugar mediante asignaciones de [!DNL AdWords].

1. Seleccione **[!UICONTROL Editar asignaciones de AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione la **[!UICONTROL Conversión de AdWords]** que desee para cada etapa que desee rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Una vez que haya asignado las fases, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Cuando haya terminado de asignar todas las conversiones de [!DNL AdWords] a las fases de ingresos, vuelva a la página de resumen. Seleccione **[!UICONTROL Acciones de modelo]** y elija **[!UICONTROL Aprobar etapas]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para ver los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de [!DNL AdWords]. Le recomendamos que use su [característica Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversión para cada conversión sin conexión que importe desde Marketo.
