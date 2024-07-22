---
unique-page-id: 6095008
description: "Agregar  [!DNL Google AdWords] servicio as a [!DNL LaunchPoint] Service - Documentos de Marketo - Documentación del producto"
title: "Agregar [!DNL Google AdWords] como [!DNL LaunchPoint] servicio"
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Agregar [!DNL Google AdWords] como servicio [!DNL LaunchPoint] {#add-google-adwords-as-a-launchpoint-service}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], podrá ver fácilmente qué clics resultaron en posibles clientes, oportunidades y clientes nuevos calificados (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} en [!DNL AdWords]. Esta información no aparece en la interfaz de usuario de Marketo.

Obtenga más información acerca de la característica de importación de conversión sin conexión de [Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>También puede integrar un servicio [[!DNL Google AdWords] as a [!DNL Launchpoint] con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Seleccione **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Seleccione **[!UICONTROL Nuevo]** y **[!UICONTROL Nuevo servicio]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Escriba un [!UICONTROL nombre para mostrar] y seleccione **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Seleccione **[!UICONTROL Autorizar Marketo]**.

   >[!NOTE]
   >
   >Asegúrese de cerrar la sesión de su cuenta personal de [!DNL Gmail] y habilitar las ventanas emergentes.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Seleccione la cuenta asociada con [!DNL Google AdWords].

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Seleccione **[!UICONTROL Aceptar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. El estado se mostrará como **[!UICONTROL Correcto]**. Seleccione **[!UICONTROL Siguiente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Cargue sus conversiones sin conexión de Marketo a [!DNL Google AdWords] **[!UICONTROL Semanal]** o **[!UICONTROL Diario]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Conversión de atributos a **[!UICONTROL Primer clic]** o **[!UICONTROL Último clic]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Tipo | Definición |
   |---|---|
   | [!UICONTROL Primer clic] | Las conversiones sin conexión se atribuirán al primer anuncio de [!DNL AdWords] en el que hizo clic una persona en los últimos 90 días |
   | [!UICONTROL Último clic] | Las conversiones sin conexión se atribuirán a los últimos [!DNL AdWords] en los que hizo clic una persona |

   >[!NOTE]
   >
   >El uso de un modelo de atribución coherente en Marketo y [!DNL AdWords] proporciona los datos más precisos.

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Se debe seleccionar el etiquetado automático](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} para que esta característica funcione. La desactivación debe realizarse dentro de [!DNL AdWords].

¡Excelente! Ahora consulte el artículo relacionado siguiente para obtener información sobre cómo asignar [!DNL AdWords] conversiones sin conexión en su modelo de ingresos.

>[!MORELIKETHIS]
>
>[Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
