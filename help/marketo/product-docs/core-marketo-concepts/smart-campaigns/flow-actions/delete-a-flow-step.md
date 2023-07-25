---
unique-page-id: 1146987
description: 'Eliminación de un paso de flujo: documentos de Marketo, documentación del producto'
title: Eliminar un paso de flujo
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Eliminar un paso de flujo {#delete-a-flow-step}

>[!CAUTION]
>
>Eliminación de pasos de flujo, _pasos de espera especialmente_ de campañas inteligentes activas, puede tener resultados inesperados. **Lea este artículo detenidamente.**

Primero vamos a hacer lo básico. Así se elimina un paso de flujo no deseado de una campaña inteligente. 1. En el flujo de campaña inteligente, haga clic en el icono X para eliminar cualquier paso del flujo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Clic **Eliminar**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple y fácil, ¿verdad? Bueno, la mayor parte del tiempo...

   >[!CAUTION]
   >
   >Eliminar, agregar y mover pasos dentro de un **activo** campaign puede tener resultados inesperados. Considere la posibilidad de crear una nueva campaña, probarla y, a continuación, cambiar.

   Se pueden realizar cambios en una campaña activa, pero pueden tener consecuencias imprevistas. A continuación se muestran los detalles:

   **Campañas inteligentes por lotes**

   Si su campaña:

   1. **Nunca corrí.** Realice todos los cambios que desee. No afectará a nadie hasta que ejecute esa campaña.
   1. **Es una campaña inteligente recurrente.** Los cambios afectarán a las personas en las ejecuciones futuras, no en las anteriores.
   1. **Ya se ejecutó SIN pasos de espera.** Ninguna persona se verá afectada porque la campaña está inactiva después de ejecutarse.
   1. **Está corriendo en este momento.** Los cambios pueden provocar un comportamiento inesperado según el momento y los detalles de la eliminación. Se recomienda NO editar una campaña por lotes que se esté ejecutando de forma activa. Para casos de emergencia, aprenda a [anulación de una campaña inteligente en ejecución](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Ya se ejecutó CON pasos de espera.** Varios detalles sobre este.\
      Cuando una persona introduce un paso de espera, esta reduce la duración y el PASO NUMÉRICO al que desea volver. Consulte el ejemplo siguiente.

   **Déclencheur de campañas inteligentes**

   1. **Sin pasos de espera.** Si elimina un paso normal, solo se verán afectadas las personas que realicen la campaña en el futuro.
   1. **Con pasos de espera.** Consulte el ejemplo siguiente para campañas por lotes. Se aplica la misma lógica.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >1. Una campaña inteligente tiene tres pasos.
   >    * PASO 1. Enviar #1 de correo electrónico
   >    * PASO 2. Esperar 1 semana
   >    * PASO 3. Enviar #2 de correo electrónico
   >
   >1. Personas que golpean **Paso 2** esperará 1 semana antes de pasar a **Paso 3**.
   >1. Usted elimina **Paso 2** durante la semana.
   >1. La gente seguirá esperando la semana 1. (No vuelven a aparecer automáticamente en el flujo).
   >1. Cuando finalmente regresen, intentarán ir a... **Paso 3**. No lo van a encontrar.
   >1. **IMPORTANTE:** Dado que ahora solo hay 2 pasos, la variable *Las personas afectadas no recibirán #2 de correo electrónico.*

Realización de cambios en una campaña activa

Comprenda esta función y dominará las campañas inteligentes.
