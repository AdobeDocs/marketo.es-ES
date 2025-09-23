---
unique-page-id: 7504923
description: Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos con una cuenta de administrador - Documentos de Marketo - Documentación del producto
title: Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos con una cuenta de administrador
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Establecer [!DNL Google AdWords] conversiones en el modelo de ingresos con una cuenta de administrador {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule su cuenta de [!DNL Google AdWords] a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a [!DNL Google AdWords]. A continuación, desde la interfaz de usuario de [!DNL AdWords], podrá ver fácilmente qué clics resultaron en posibles clientes, oportunidades y clientes nuevos calificados (o las fases de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en [!DNL AdWords].

Si tiene varias cuentas de [!DNL Google Adwords], puede usar una [[!DNL Google AdWords] cuenta de administrador](https://www.google.com/adwords/manager-accounts/) (anteriormente conocida como Mi centro de cliente) para integrarlas con Marketo.

Puede asignar [!DNL AdWords] conversiones sin conexión a una o más etapas en un modelo de ingresos. Hay dos maneras:

* Fase de acción
* Asignación de [!DNL AdWords]

>[!PREREQUISITES]
>
>[Agregar [!DNL Google AdWords] como servicio de punto de inicio con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar acción de escenario {#use-stage-action}

Asignar una conversión [!DNL AdWords] en Acciones de ensayo.

1. Seleccione el paso que desea asignar a una conversión de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En el menú desplegable **[!UICONTROL Acciones de ensayo]**, seleccione **[!UICONTROL Definir conversión de AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Establecer una conversión de **[!DNL AdWords]**.

   >[!NOTE]
   >
   >Se puede seleccionar una conversión [!DNL AdWords] diferente para cada cuenta secundaria.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Sugerencia: Si no tiene ninguna conversión de [!DNL AdWords], cree una haciendo clic en **[!UICONTROL +Nueva conversión]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Escriba un **Nombre de conversión**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de [!DNL AdWords].

## Usar asignación [!DNL AdWords] {#use-adwords-mapping}

Puede asociar todas las fases del modelo con la conversión de [!DNL AdWords] en un solo lugar mediante asignaciones de [!DNL AdWords].

1. Seleccione **[!UICONTROL Editar asignaciones de AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione la cuenta **[!DNL AdWords]** y la conversión **[!DNL AdWords]** que desee para cada etapa que desee rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Una vez que haya asignado las fases, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Cuando haya terminado de asignar todas las conversiones de [!DNL AdWords] a las fases de ingresos, vuelva a la página de resumen. Seleccione **[!UICONTROL Acciones de modelo]** y elija **[!UICONTROL Aprobar etapas]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para ver los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de [!DNL AdWords]. Le recomendamos que use su [característica Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversión para cada conversión sin conexión que importe desde Marketo.
