---
unique-page-id: 1146997
description: Usar un token de fecha en un paso de flujo de espera - Documentos de marketing - Documentación del producto
title: Usar un token de fecha en un paso de flujo de espera
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Usar un token de fecha en un paso de flujo de espera {#use-a-date-token-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el viaje de una persona a través de una campaña inteligente hasta una fecha concreta que utilice un token de fecha. También puede modificar la fecha de finalización en un número determinado de días.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Esto solo se aplica a campañas desencadenadoras. No puede utilizar esta función en campañas por lotes.

1. En la ficha **Flujo** de campaña inteligente, arrastre el ratón sobre el paso de flujo de **espera** .

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Haga clic en el icono de engranaje a la derecha.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. En la lista desplegable **Tipo** , seleccione Token **de fecha**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Elija un token de fecha para especificar cuándo debe finalizar el paso de espera:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Para esperar hasta el próximo aniversario de la fecha que se produzca en el año natural actual o siguiente, marque la casilla.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilice esta opción en los tokens de fecha que hacen referencia a fechas anteriores, como una fecha de inicio de cumpleaños o contrato.

1. Opcionalmente, puede modificar la fecha de finalización en un número específico de días.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >También puede especificar el número de días utilizando un token `{{lead.` o `{{company.` que represente un campo entero o un `{{my.` token de tipo numérico.

1. Haga clic en Guardar.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**Artículos relacionados**
   >
   >* [Usar una duración en un paso de flujo de espera](use-a-duration-in-a-wait-flow-step.md)
   >* [Usar una fecha específica en un paso de flujo de espera](use-a-specific-date-in-a-wait-flow-step.md)


