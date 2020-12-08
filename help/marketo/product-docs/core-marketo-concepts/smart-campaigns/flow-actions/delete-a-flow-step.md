---
unique-page-id: 1146987
description: Eliminar un paso de flujo - Documentos de marketing - Documentación del producto
title: Eliminar un paso de flujo
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Eliminar un paso de flujo {#delete-a-flow-step}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!CAUTION]
>
>La eliminación de los pasos de flujo, *especialmente los pasos* de espera de las campañas inteligentes activas, puede tener resultados inesperados. **Lea este artículo detenidamente.**

Primero hagamos lo básico. A continuación se explica cómo eliminar un paso de flujo no deseado de una campaña inteligente. 1. En Flujo de campaña inteligente, haga clic en el icono X para eliminar cualquier paso de flujo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Haga clic en **Eliminar**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple y fácil, ¿verdad? Bueno, la mayoría de las veces...

   >[!CAUTION]
   >
   >La eliminación, adición y desplazamiento de pasos dentro de una campaña **activa** puede tener definitivamente resultados inesperados. Considere la posibilidad de crear una nueva campaña, probarla y, a continuación, cambiar.

   Se pueden realizar cambios en una campaña activa, pero pueden tener consecuencias imprevistas. A continuación se detallan los detalles:

   **Campañas inteligentes por lotes**

   Si su campaña:

   1. **Nunca huí.** Realice todos los cambios que desee. No afectará a nadie hasta que corras esa campaña.
   1. **Es una campaña inteligente recurrente.** Los cambios afectarán a las personas en las ejecuciones futuras, no en las anteriores.
   1. **Ya se ejecutó SIN pasos de espera.** Ninguna persona se verá afectada porque la campaña está inactiva después de correr.
   1. **Se está ejecutando ahora mismo.** Los cambios pueden provocar un comportamiento inesperado en función del tiempo y los detalles de la eliminación. Se recomienda NO editar una campaña por lotes que se esté ejecutando activamente. En casos de emergencia, aprenda a [cancelar una campaña](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)inteligente en ejecución.

   1. **Ya se ejecutó CON los pasos de espera.** Varios detalles sobre este.\
      Cuando una persona entra en un paso de espera, la persona baja la duración y a qué PASO NUMÉRICO volver. Consulte el ejemplo siguiente.

   **Activar Campañas inteligentes**

   1. **No hay pasos de espera.** Si elimina un paso normal, solo se verán afectadas las personas que pasen por la campaña en el futuro.
   1. **Con los pasos de espera.** Consulte el ejemplo siguiente para ver campañas por lotes. Se aplica la misma lógica.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >    
   >    
   >1. Una campaña inteligente tiene 3 pasos.
   >
   >   * PASO 1. Enviar correo electrónico n.º 1
   >   * PASO 2. Esperar 1 semana
   >   * PASO 3. Enviar correo electrónico n.º 2
   >
   >1. Las personas que hayan llegado al **paso 2** esperarán una semana antes de pasar al **paso 3**.
   >1. Se elimina el **paso 2** durante la semana.
   >1. La gente seguirá esperando la semana. (No vuelven a aparecer automáticamente en el flujo).
   >1. Cuando finalmente regresen, tratarán de ir al **Paso 3**. No lo encontrarán.
   >1. **IMPORTANTE:** Dado que ahora solo hay 2 pasos, las *personas no recibirán el correo electrónico 2.*


Realización de cambios en una Campaña activa

Comprenda esta función y dominará las campañas inteligentes. ¡Guau!
