---
unique-page-id: 7504923
description: Configurar las conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador - Marketo Docs - Documentación del producto
title: Configurar conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Configurar conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule su cuenta de Google AdWords a Marketo para cargar automáticamente los datos de conversión sin conexión de Marketo a Google AdWords. A continuación, desde la interfaz de usuario de AdWords, podrá ver fácilmente qué clics tuvieron como resultado posibles clientes calificados, oportunidades y nuevos clientes (o las etapas de ingresos que desee rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords.

Si tiene varias cuentas de Google Adwords, puede usar una [Cuenta del Administrador de Google AdWords](https://www.google.com/adwords/manager-accounts/) (anteriormente My Client Center) para integrarlos con Marketo.

Puede asignar las conversiones sin conexión de AdWords a una o varias etapas en un modelo de ingresos. Hay dos maneras:

* Acción de fase
* Asignación de AdWords

>[!PREREQUISITES]
>
>[Añadir Google AdWords como servicio de punto de inicio con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar acción de etapa {#use-stage-action}

Asigne una conversión de AdWords en Acciones de etapa.

1. Seleccione el paso que desee asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En el **Acciones de fase** desplegable, seleccione **Establecer conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Establezca un **Conversión de AdWords**.

   >[!NOTE]
   >
   >Se puede seleccionar otra conversión de AdWords para cada cuenta secundaria.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Sugerencia: Si no tiene conversiones de AdWords, cree una haciendo clic en **+Nueva conversión**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Cuando haya terminado de asignar todas las conversiones de AdWords a etapas de ingresos, vuelva a la página de resumen. Select **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Consejo de Pro: Agregar una nueva conversión {#pro-tip-add-a-new-conversion}

Consejo a favor! Se puede crear una nueva conversión sin conexión de AdWords desde Marketo.

>[!CAUTION]
>
>Las nuevas conversiones creadas a partir de Marketo tienen habilitada la configuración de &quot;optimización&quot;. Esto significa que las estrategias de oferta de AdWords están permitidas para optimizar las ofertas para esas conversiones. Puede cambiar esta configuración desde la cuenta de AdWords.

1. En el **Acciones de fase** desplegable, seleccione **Establecer conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Select **Nueva conversión**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Escriba un **Nombre de conversión**. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de AdWords.

## Usar la asignación de AdWords {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con la conversión de AdWords en un solo lugar mediante asignaciones de AdWords.

1. Select **Editar asignaciones de AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione el **Cuenta de AdWords** y **Conversión de AdWords** para cada etapa que desee rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Una vez asignadas las etapas, haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Cuando haya terminado de asignar todas las conversiones de AdWords a etapas de ingresos, vuelva a la página de resumen. Select **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para ver los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de AdWords. Le recomendamos que use su [Función Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversiones para cada conversión sin conexión que importe desde Marketo.
