---
unique-page-id: 7504893
description: Integre varias  [!DNL Google AdWords] cuentas con Marketo mediante una cuenta de administrador en LaunchPoint.
title: Agregar  [!DNL Google AdWords] como [!DNL Launchpoint] servicio con una cuenta de gerente
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/fQYFZRLEULbnvJnYh1Yp9ziGIz1KPYwUPSqeo5Et63Y
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
source-wordcount: 309
ht-degree: 2%

---

# Agregar [!DNL Google AdWords] como servicio de [!DNL Launchpoint] con una cuenta de administrador {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], puede ver qué clics dieron como resultado posibles clientes calificados, oportunidades y nuevos clientes (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} en [!DNL AdWords]. Esta información no aparece en la interfaz de usuario de Marketo.

Si tiene varias cuentas de [!DNL Google Adwords], puede usar una cuenta de [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (anteriormente conocida como [!DNL My Client Center]) para integrarlas con Marketo.

Obtenga más información acerca de la característica de importación de conversión sin conexión de [Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>También puedes integrar una [cuenta independiente [!DNL Google AdWords] como [!DNL Launchpoint] servicio](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Seleccione **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Haga clic en el menú desplegable **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo servicio]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Escriba un **[!UICONTROL Nombre para mostrar]** y seleccione **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Seleccione **[!UICONTROL Autorizar Marketo]**.

   >[!NOTE]
   >
   >Asegúrese de cerrar la sesión de su cuenta personal de [!DNL Gmail] y habilitar las ventanas emergentes.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Seleccione la cuenta asociada con **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. El estado se muestra como **[!UICONTROL Correcto]**. Seleccione **[!UICONTROL Siguiente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Cargue sus conversiones sin conexión de Marketo a [!DNL Google AdWords] **[!UICONTROL Semanal]** o **[!UICONTROL Diario]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Conversión de atributos a **[!UICONTROL Primer clic]** o **[!UICONTROL Último clic]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Tipo | Definición |
   |---|---|
   | [!UICONTROL Primer clic] | Las conversiones sin conexión se atribuirán al primer anuncio de [!DNL AdWords] en el que hizo clic una persona en los últimos 90 días |
   | [!UICONTROL Último clic] | Las conversiones sin conexión se atribuirán a los últimos [!DNL AdWords] en los que hizo clic una persona |

   >[!NOTE]
   >
   >[Se debe seleccionar el etiquetado automático](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} para que esta característica funcione. Debe activarse dentro de [!DNL AdWords].

1. Haga clic en **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Anule la selección de las cuentas que no quiera actualizar. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Consulte el artículo relacionado siguiente para ver cómo asignar [!DNL AdWords] conversiones sin conexión en su modelo de ingresos.
