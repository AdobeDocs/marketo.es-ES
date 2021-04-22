---
unique-page-id: 1146987
description: 'Eliminación de un paso de flujo: documentos de Marketo: documentación del producto'
title: Eliminación de un paso de flujo
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Eliminar un paso de flujo {#delete-a-flow-step}

>[!CAUTION]
>
>La eliminación de los pasos de flujo, _especialmente los pasos de espera_ de las campañas inteligentes activas, puede tener resultados inesperados. **Lea este artículo detenidamente.**

Primero hagamos lo básico. Así se elimina un paso de flujo no deseado de una campaña inteligente. 1. En Flujo de campaña inteligente, haga clic en el icono X para eliminar cualquier paso de flujo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Haga clic en **Eliminar**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple y fácil, ¿verdad? Bueno, la mayoría de las veces...

   >[!CAUTION]
   >
   >La eliminación, adición y desplazamiento de pasos dentro de una campaña **activa** definitivamente pueden tener resultados inesperados. Considere la posibilidad de crear una nueva campaña, probarla y, a continuación, cambiar.

   Se pueden realizar cambios en una campaña activa, pero pueden tener consecuencias imprevistas. Aquí están los detalles:

   **Lotes de campañas inteligentes**

   Si la campaña:

   1. **Nunca corrió.** Realice todos los cambios que desee. No afectará a nadie hasta que ejecute esa campaña.
   1. **Es una campaña inteligente recurrente.** Los cambios afectarán a las personas en las ejecuciones futuras, no a las anteriores.
   1. **Ya se ha ejecutado sin pasos de espera.** Ninguna persona se verá afectada porque la campaña está inactiva después de ejecutarse.
   1. **Se está ejecutando ahora mismo.** Los cambios pueden provocar un comportamiento inesperado en función de la hora y los detalles de la eliminación. Se recomienda NO editar una campaña por lotes que se esté ejecutando activamente. Para casos de emergencia, aprenda a [cancelar una campaña inteligente en ejecución](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Ya ejecutó CON pasos de espera.** Varios detalles sobre esto.\
      Cuando una persona introduce un paso de espera, la persona reduce la duración y a qué paso NUMBER regresar. Consulte el ejemplo siguiente.

   **Campañas inteligentes de déclencheur**

   1. **Sin pasos de espera.** Si elimina un paso normal, solo se verán afectadas las personas que ejecuten la campaña en el futuro.
   1. **Con los pasos de espera.** Consulte el ejemplo siguiente para ver las campañas por lotes. Se aplica la misma lógica.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >1. Una campaña inteligente tiene 3 pasos.
      >    * PASO 1. Enviar correo electrónico n.º 1
      >    * PASO 2. Espera 1 semana
      >    * PASO 3. Enviar correo electrónico n.º 2
   >
   >1. Las personas que hayan llegado al **paso 2** esperarán una semana antes de pasar al **paso 3**.
   >1. El **paso 2** se elimina durante la semana.
   >1. La gente seguirá esperando la semana 1. (No vuelven a aparecer automáticamente en el flujo).
   >1. Cuando finalmente regresen, intentarán ir al **paso 3**. No lo encontrarán.
   >1. **IMPORTANTE:** Dado que ahora solo hay 2 pasos, las  *personas no recibirán el correo electrónico n.º 2.*


Realización de cambios en una campaña activa

Comprenda esta función y dominará las campañas inteligentes.
