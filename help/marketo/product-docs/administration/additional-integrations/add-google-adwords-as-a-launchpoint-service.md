---
unique-page-id: 6095008
description: Vincule  [!DNL Google AdWords] a Marketo a través de LaunchPoint para cargar datos de conversión sin conexión para la generación de informes en AdWords.
title: Agregar  [!DNL Google AdWords] como [!DNL LaunchPoint] servicio
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/gpw57sy3WitNAh6g4mkajXuuFlRFzunZmfedM4aCrCk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 284
ht-degree: 2%

---

# Agregar [!DNL Google AdWords] como servicio [!DNL LaunchPoint] {#add-google-adwords-as-a-launchpoint-service}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], puede ver qué clics dieron como resultado posibles clientes calificados, oportunidades y nuevos clientes (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} en [!DNL AdWords]. Esta información no aparece en la interfaz de usuario de Marketo.

Obtenga más información acerca de la característica de importación de conversión sin conexión de [Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>**Se requieren permisos de administrador**

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

1. El estado se muestra como **[!UICONTROL Correcto]**. Seleccione **[!UICONTROL Siguiente]**.

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

Consulte el artículo relacionado siguiente para obtener información sobre cómo asignar [!DNL AdWords] conversiones sin conexión en su modelo de ingresos.
