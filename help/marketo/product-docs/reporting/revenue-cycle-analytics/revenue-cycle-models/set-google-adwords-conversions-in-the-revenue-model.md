---
unique-page-id: 6095029
description: Conversiones de Google AdWords en el modelo de ingresos - Documentos de Marketo - Documentación del producto
title: Establecer conversiones de Google AdWords en el modelo de ingresos
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Establecer conversiones de Google AdWords en el modelo de ingresos {#set-google-adwords-conversions-in-the-revenue-model}

Vincule su cuenta de Google AdWords a Marketo para cargar automáticamente datos de conversión sin conexión de Marketo a Google AdWords. A continuación, desde la interfaz de usuario de AdWords, podrá ver fácilmente qué clics resultaron en posibles clientes calificados, oportunidades y nuevos clientes (o las etapas de ingresos que desee rastrear) después de usted [añadir columnas personalizadas](https://support.google.com/adwords/answer/3073556) en AdWords.

>[!NOTE]
>
>Se trata de una integración push de Marketo a Google AdWords. Aparecerán los datos de conversión _solamente_ en su portal de Google AdWords, _no está en la IU de Marketo_.

Más información sobre [Función de importación de conversión sin conexión de Google](https://support.google.com/adwords/answer/2998031?hl=en). Asigne conversiones sin conexión de AdWords a una o más etapas en un modelo de ingresos. Existen tres formas de realizar la asignación:

* Conversión de AdWords
* Fase de acción
* Asignación de AdWords

Puede crear una nueva conversión sin conexión de AdWords desde Marketo si utiliza la acción de fase.

>[!PREREQUISITES]
>
>[Añadir Google AdWords como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Utilizar la conversión de AdWords {#use-adwords-conversion}

1. Vaya a la **Analytics** área.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Seleccione un modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Clic **Editar borrador**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Seleccione la etapa de ingresos que desee asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Seleccione el **Conversión de AdWords** desea asignar a su fase de Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   ¡Bonito! Los datos de conversión de AdWords se cargarán en Google AdWords en la cadencia seleccionada.

## Usar acción de escenario {#use-stage-action}

También puede asignar una Conversión de AdWords en Acciones de ensayo.

1. Seleccione el paso que desea asignar a una conversión de AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. En el **Acciones de fase** menú desplegable, seleccione **Establecer conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccione un **Conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Sugerencia**: Si no tiene ninguna conversión de AdWords, cree una haciendo clic en **+Nueva conversión**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Clic **Guardar**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las fases de ingresos, vuelva a la página de resumen. Seleccionar **Acciones de modelo** y elija **Aprobar fases**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Sugerencia profesional: Añada una nueva conversión {#pro-tip-add-a-new-conversion}

¡Consejo profesional! Se puede crear una nueva conversión sin conexión de AdWords desde Marketo.

>[!CAUTION]
>
>Las nuevas conversiones creadas desde Marketo tienen activada la configuración de &quot;optimización&quot;. Esto significa que las estrategias de oferta de AdWords pueden optimizar sus ofertas para esas conversiones. Puede cambiar esta configuración desde su cuenta de AdWords.

1. En el **Acciones de fase** menú desplegable, seleccione **Establecer conversión de AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleccionar **Nueva conversión**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Introduzca una **Nombre de conversión**. Clic **Guardar**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   ¡Excelente! Esta nueva conversión aparecerá en su cuenta de AdWords.

## Usar asignación de AdWords {#use-adwords-mapping}

Puede asociar todas las etapas del modelo con su Conversión de AdWords en un solo lugar usando Asignaciones de AdWords.

1. Seleccionar **Editar asignaciones de AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleccione el **Conversión de AdWords** para cada fase que desee rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Una vez que haya asignado las fases, haga clic en **Guardar**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Una vez que haya terminado de asignar todas las conversiones de AdWords a las fases de ingresos, vuelva a la página de resumen. Seleccionar **Acciones de modelo** y elija **Aprobar fases**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para ver los datos de conversión sin conexión, deberá iniciar sesión en su cuenta de AdWords. Le recomendamos que utilice su [Función Columnas personalizadas](https://support.google.com/adwords/answer/3073556) para crear columnas de recuento de conversión para cada conversión sin conexión que importe desde Marketo.
