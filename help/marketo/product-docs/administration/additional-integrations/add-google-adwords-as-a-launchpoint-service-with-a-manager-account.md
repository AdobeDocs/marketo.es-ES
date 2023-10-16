---
unique-page-id: 7504893
description: "Agregar [!DNL Google AdWords] as a [!DNL Launchpoint] Servicio con una cuenta de responsable - Documentos de Marketo - Documentación del producto"
title: "Agregar [!DNL Google AdWords] as a [!DNL Launchpoint] Servicio con una cuenta de responsable"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Añadir [!DNL Google AdWords] as a [!DNL Launchpoint] Servicio con una cuenta de responsable {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Vincule su [!DNL Google AdWords] a Marketo para cargar automáticamente datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde el [!DNL AdWords] IU, podrá ver fácilmente qué clics resultaron en posibles clientes cualificados, oportunidades y nuevos clientes (o las fases de ingresos que desee rastrear) después de usted  [añadir columnas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Esta información no aparece en la interfaz de usuario de Marketo.

Si tiene varias [!DNL Google Adwords] cuentas, puede utilizar un [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (anteriormente conocido como [!DNL My Client Center]) para integrarlos con Marketo.

Más información sobre [Función de importación de conversión sin conexión de Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!NOTE]
>
>También puede integrar un [independiente [!DNL Google AdWords] cuenta como [!DNL Launchpoint] servicio](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Seleccionar **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione. **[!UICONTROL Nuevo servicio]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Introduzca una **[!UICONTROL Nombre para mostrar]** y seleccione **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Seleccionar **[!UICONTROL Autorizar Marketo]**.

   >[!NOTE]
   >
   >Asegúrese de cerrar la sesión de su [!DNL Gmail] y habilitar ventanas emergentes.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Seleccione la cuenta asociada a **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Clic **[!UICONTROL Aceptar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. El estado se mostrará como **[!UICONTROL Correcto]**. Seleccionar **[!UICONTROL Siguiente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Cargar las conversiones sin conexión de Marketo a [!DNL Google AdWords] **[!UICONTROL Semanalmente]** o **[!UICONTROL Diario]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Conversión de atributos a **[!UICONTROL Primer clic]** o **[!UICONTROL Último clic]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Tipo | Definición |
   |---|---|
   | [!UICONTROL Primer clic] | Las conversiones sin conexión se atribuirán a la primera [!DNL AdWords] anuncio en el que una persona ha hecho clic en los últimos 90 días |
   | [!UICONTROL Último clic] | Las conversiones sin conexión se atribuirán a la última [!DNL AdWords] y en el que una persona hizo clic |

   >[!NOTE]
   >
   >[Etiquetado automático](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} debe estar seleccionado para que esta función funcione. Debe activarse en el interior [!DNL AdWords].

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Anule la selección de las cuentas que no quiera actualizar. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Ahora consulte el artículo relacionado siguiente para ver cómo asignar [!DNL AdWords] conversiones sin conexión en el modelo de ingresos.

   >[!MORELIKETHIS]
   >
   >[Establecer [!DNL Google AdWords] Conversiones en el modelo de ingresos con una cuenta de responsable](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
