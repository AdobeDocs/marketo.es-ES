---
unique-page-id: 7504923
description: Configurar las conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador - Documentos de marketing - Documentación del producto
title: Configurar las conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Configure las conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule su cuenta de Google AdWords a Marketing para cargar automáticamente datos de conversión sin conexión de Marketing a Google AdWords. Luego, desde la interfaz de usuario de AdWords, podrá ver fácilmente qué clics generaron posibles clientes calificados, oportunidades y nuevos clientes (o las etapas de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords.

Si tiene varias cuentas de Google Adwords, puede utilizar una [cuenta del administrador de Google AdWords](https://www.google.com/adwords/manager-accounts/) (anteriormente denominada My Client Center) para integrarlas con Marketing.

Puede asignar las conversiones sin conexión de AdWords a una o varias etapas en un modelo de ingresos. Existen dos maneras:

* Acción de etapa
* Asignación de AdWords

>[!PREREQUISITES]
>
>[Añadir Google AdWords como un servicio de punto de lanzamiento con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar acción de etapa {#use-stage-action}

Asigne una conversión de AdWords en Acciones de la etapa.

1. Seleccione el paso que desee asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En la lista desplegable **Acciones de etapa**, seleccione **Configurar conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Establezca una **Conversión de AdWords**.

   >[!NOTE]
   >
   >Se puede seleccionar otra conversión de AdWords para cada cuenta secundaria.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Sugerencia: Si no tiene ninguna conversión de AdWords, cree una haciendo clic en **+Nueva conversión**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Escriba un **Nombre de conversión**. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de AdWords.

## Usar la asignación de AdWords {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con la conversión de AdWords en un solo lugar mediante asignaciones de AdWords.

1. Seleccione **Editar asignaciones de AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione la **Cuenta de AdWords** deseada y **Conversión de AdWords** deseada para cada etapa que desee rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Una vez asignadas las etapas, haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las etapas de ingresos, vuelva a la página de resumen. Seleccione **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para realizar la vista de los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de AdWords. Le recomendamos que utilice la función [Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversiones para cada conversión sin conexión que importe desde Marketing.
