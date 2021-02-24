---
unique-page-id: 6095029
description: Configurar las conversiones de Google AdWords en el modelo de ingresos - Documentos de marketing - Documentación del producto
title: Configurar las conversiones de Google AdWords en el modelo de ingresos
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Establecer las conversiones de Google AdWords en el modelo de ingresos {#set-google-adwords-conversions-in-the-revenue-model}

Vincule su cuenta de Google AdWords a Marketing para cargar automáticamente datos de conversión sin conexión de Marketing a Google AdWords. Luego, desde la interfaz de usuario de AdWords, podrá ver fácilmente qué clics generaron posibles clientes calificados, oportunidades y nuevos clientes (o las etapas de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords.

>[!NOTE]
>
>Esta es una integración push de Marketing a Google AdWords. Los datos de conversión aparecerán _sólo_ en el portal Google AdWords, _no en la interfaz de usuario de Marketing_.

Obtenga más información sobre la [función de importación de conversión sin conexión de Google](https://support.google.com/adwords/answer/2998031?hl=en). Asigne las conversiones sin conexión de AdWords a una o más etapas de un modelo de ingresos. Existen tres formas de realizar la asignación:

* Conversión de AdWords
* Acción de etapa
* Asignación de AdWords

Puede crear una nueva conversión sin conexión de AdWords desde Marketing a si utiliza Acción de etapa.

>[!PREREQUISITES]
>
>[Añadir Google AdWords como un servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usar conversión de AdWords {#use-adwords-conversion}

1. Vaya al área **Analytics**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Seleccione un modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Haga clic en **Editar borrador**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Seleccione la etapa de ingresos que desee asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Seleccione la **Conversión de AdWords** que desea asignar a la etapa de marketing.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   ¡Bonito! Los datos de conversión de AdWords se cargarán en Google AdWords en la cadencia seleccionada.

## Usar acción de etapa {#use-stage-action}

También puede asignar una conversión de AdWords en Acciones de la etapa.

1. Seleccione el paso que desee asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En la lista desplegable **Acciones de etapa**, seleccione **Configurar conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione una **Conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Sugerencia**: Si no tiene ninguna conversión de AdWords, cree una haciendo clic en  **+Nueva conversión**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las etapas de ingresos, vuelva a la página de resumen. Seleccione **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Sugerencia de Pro: Añadir una nueva conversión {#pro-tip-add-a-new-conversion}

¡Sugerencia profesional! Se puede crear una nueva conversión sin conexión de AdWords desde Marketing.

>[!CAUTION]
>
>Las nuevas conversiones creadas a partir de Marketing tienen habilitada la configuración de &quot;optimización&quot;. Esto significa que las estrategias de oferta de AdWords pueden optimizar las ofertas para esas conversiones. Puede cambiar esta configuración desde la cuenta de AdWords.

1. En la lista desplegable **Acciones de etapa**, seleccione **Configurar conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione **Nueva conversión**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Escriba un **Nombre de conversión**. Haga clic en **Guardar**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de AdWords.

## Usar la asignación de AdWords {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con la conversión de AdWords en un solo lugar mediante asignaciones de AdWords.

1. Seleccione **Editar asignaciones de AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione la **Conversión de AdWords** deseada para cada etapa que desee rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Una vez asignadas las etapas, haga clic en **Guardar**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las etapas de ingresos, vuelva a la página de resumen. Seleccione **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para realizar la vista de los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de AdWords. Le recomendamos que utilice la función [Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversiones para cada conversión sin conexión que importe desde Marketing.
