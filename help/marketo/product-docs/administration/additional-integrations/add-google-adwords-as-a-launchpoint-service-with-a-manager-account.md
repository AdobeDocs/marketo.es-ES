---
unique-page-id: 7504893
description: "Agregar  [!DNL Google AdWords] as a [!DNL Launchpoint] Servicio con una cuenta de administrador - Documentos de Marketo - Documentación del producto"
title: "Agregar  [!DNL Google AdWords] como [!DNL Launchpoint] servicio con una cuenta de administrador"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Agregar [!DNL Google AdWords] como servicio de [!DNL Launchpoint] con una cuenta de administrador {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], podrá ver fácilmente qué clics resultaron en posibles clientes, oportunidades y nuevos clientes calificados (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} en [!DNL AdWords]. Esta información no aparece en la interfaz de usuario de Marketo.

Si tiene varias cuentas de [!DNL Google Adwords], puede usar una cuenta de [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (anteriormente conocida como [!DNL My Client Center]) para integrarlas con Marketo.

Obtenga más información acerca de la característica de importación de conversión sin conexión de [Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>**Se requieren permisos de administración**

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

1. El estado se mostrará como **[!UICONTROL Correcto]**. Seleccione **[!UICONTROL Siguiente]**.

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

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Anule la selección de las cuentas que no quiera actualizar. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Ahora consulte el artículo relacionado siguiente para ver cómo asignar [!DNL AdWords] conversiones sin conexión en su modelo de ingresos.

   >[!MORELIKETHIS]
   >
   >[Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos con una cuenta de administrador](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
