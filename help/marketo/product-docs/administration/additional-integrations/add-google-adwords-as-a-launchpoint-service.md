---
unique-page-id: 6095008
description: 'Añadir Google AdWords como un servicio de LaunchPoint: Documentos de Marketo: Documentación del producto'
title: Añadir Google AdWords como un servicio de LaunchPoint
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Agregar Google AdWords como un servicio de LaunchPoint {#add-google-adwords-as-a-launchpoint-service}

Vincule su cuenta de Google AdWords a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a Google AdWords. A continuación, desde la interfaz de usuario de AdWords, podrá ver fácilmente qué clics tuvieron como resultado posibles clientes calificados, oportunidades y nuevos clientes (o las etapas de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords. Esta información no aparece en la interfaz de usuario de Marketo.

Obtenga más información sobre la [función de importación de conversión sin conexión de Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>También puede integrar un [Google AdWords como servicio de punto de inicio con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Vaya a la sección **Admin**.

   ![](assets/login-admin.png)

1. Seleccione **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Seleccione **Nuevo** y **Nuevo servicio**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Introduzca un nombre para mostrar y seleccione **Google AdWords**.

   ![](assets/new-service-google.png)

1. Seleccione **Autorizar Marketo**.

   >[!NOTE]
   >
   >Asegúrese de cerrar la sesión de su cuenta personal de Gmail y activar ventanas emergentes.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Seleccione la cuenta asociada a Google AdWords.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Seleccione **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. El estado se mostrará como **Success**. Seleccione **Siguiente**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Cargue las conversiones sin conexión de Marketo a Google AdWords **Semanal** o **Diaria**.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Conversión de atributos al **Primer clic** o **Último clic**.

   | Tipo | Definición |
   |---|---|
   | Primer clic | Las conversiones sin conexión se atribuirán al primer anuncio de AdWords en el que hizo clic una persona en los últimos 90 días |
   | Último clic | Las conversiones sin conexión se atribuirán al último anuncio de AdWords en el que hizo clic una persona |

   >[!NOTE]
   >
   >El uso de un modelo de atribución coherente en Marketo y AdWords proporciona los datos más precisos.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Haga clic en **Crear**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Para que esta función funcione, debe ](https://support.google.com/adwords/answer/1752125?hl=en) estar seleccionada la etiqueta automática. La desactivación debe realizarse dentro de AdWords.

¡bueno! Ahora, vea el Artículo relacionado a continuación para aprender a asignar conversiones sin conexión de AdWords en su modelo de ingresos.

>[!MORELIKETHIS]
>
>[Configurar las conversiones de Google AdWords en el modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
