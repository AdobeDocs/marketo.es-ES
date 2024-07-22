---
unique-page-id: 7504923
description: Conversiones de Google AdWords en el modelo de ingresos con una cuenta de responsable - Documentos de Marketo - Documentación del producto
title: Establecer conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Establecer conversiones de Google AdWords en el modelo de ingresos con una cuenta de administrador {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule su cuenta de Google AdWords a Marketo para cargar automáticamente datos de conversión sin conexión de Marketo a Google AdWords. Entonces, desde la interfaz de usuario de AdWords, podrás ver fácilmente qué clics resultaron en posibles clientes, oportunidades y nuevos clientes calificados (o las etapas de ingresos que quieras rastrear) después de [agregar columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords.

Si tiene varias cuentas de Google AdWords, puede usar una [cuenta de Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (anteriormente conocida como My Client Center) para integrarlas con Marketo.

Puede asignar conversiones sin conexión de AdWords a una o más etapas en un modelo de ingresos. Hay dos maneras:

* Fase de acción
* Asignación de AdWords

>[!PREREQUISITES]
>
>[Agregar Google AdWords como servicio de punto de inicio con una cuenta de administrador](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar acción de escenario {#use-stage-action}

Asigne una conversión de AdWords en Acciones de fase.

1. Seleccione el paso que desea asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En el menú desplegable **Acciones de ensayo**, seleccione **Definir conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Establecer una **conversión de AdWords**.

   >[!NOTE]
   >
   >Se puede seleccionar una conversión de AdWords diferente para cada cuenta secundaria.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Sugerencia: Si no tiene ninguna conversión de AdWords, cree una haciendo clic en **+Nueva conversión**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las fases de ingresos, vuelva a la página de resumen. Seleccione **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Sugerencia profesional: Añada una nueva conversión {#pro-tip-add-a-new-conversion}

¡Consejo profesional! Se puede crear una nueva conversión sin conexión de AdWords desde Marketo.

>[!CAUTION]
>
>Las nuevas conversiones creadas desde Marketo tienen activada la configuración de &quot;optimización&quot;. Esto significa que las estrategias de oferta de AdWords pueden optimizar sus ofertas para esas conversiones. Puede cambiar esta configuración desde su cuenta de AdWords.

1. En el menú desplegable **Acciones de ensayo**, seleccione **Definir conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione **Nueva conversión**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Escriba un **Nombre de conversión**. Haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de AdWords.

## Usar asignación de AdWords {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con su Conversión de AdWords en un solo lugar usando Asignaciones de AdWords.

1. Seleccione **Editar asignaciones de AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione la **cuenta de AdWords** y la **conversión de AdWords** que desee para cada etapa que desee rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Una vez que haya asignado las fases, haga clic en **Guardar**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las fases de ingresos, vuelva a la página de resumen. Seleccione **Acciones de modelo** y elija **Aprobar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para ver los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de AdWords. Le recomendamos que use su [característica Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversión para cada conversión sin conexión que importe desde Marketo.
