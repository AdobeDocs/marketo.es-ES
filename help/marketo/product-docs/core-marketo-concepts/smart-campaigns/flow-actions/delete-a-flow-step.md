---
unique-page-id: 1146987
description: 'Eliminación de un paso de flujo: documentos de Marketo, documentación del producto'
title: Eliminar un paso de flujo
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Eliminar un paso de flujo {#delete-a-flow-step}

>[!CAUTION]
>
>Si elimina los pasos del flujo, _especialmente los pasos de espera_ de las campañas inteligentes activas, puede dar resultados inesperados. Lea este artículo detenidamente.

Primero vamos a cubrir los conceptos básicos. Así se elimina un paso de flujo no deseado de una campaña inteligente.

1. En la campaña inteligente **[!UICONTROL Flujo]**, haga clic en el icono **X** para eliminar cualquier paso del flujo.

   ![](assets/delete-a-flow-step-1.png)

1. Haga clic en **[!UICONTROL Eliminar]**.

   ![](assets/delete-a-flow-step-2.png)

   >[!CAUTION]
   >
   >Eliminar, agregar y mover pasos dentro de una campaña _activa_ puede tener resultados inesperados. Considere la posibilidad de crear una nueva campaña, probarla y, a continuación, cambiar.

   Se pueden realizar cambios en una campaña activa, pero pueden tener consecuencias imprevistas. A continuación se muestran los detalles:

   **Campañas inteligentes por lotes**

   Si su campaña:

   1. **Nunca se ejecutó**. Realice todos los cambios que desee. No afectará a nadie hasta que ejecute esa campaña.
   1. **Es una campaña inteligente recurrente**. Los cambios afectarán a las personas en las ejecuciones futuras, no en las anteriores.
   1. **Ya se ejecutó SIN pasos de espera**. Ninguna persona se verá afectada porque la campaña está inactiva después de ejecutarse.
   1. **Se está ejecutando**. Los cambios pueden provocar un comportamiento inesperado según el momento y los detalles de la eliminación. Se recomienda NO editar una campaña por lotes que se esté ejecutando de forma activa. Para casos de emergencia, aprenda a [cancelar una campaña inteligente en ejecución](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}.

   1. **Ya se ejecutó CON pasos de espera.** Varios detalles sobre este.\
      Cuando una persona introduce un paso de espera, esta reduce la duración y el PASO NUMÉRICO al que desea volver. Consulte el ejemplo siguiente.

   **Campañas inteligentes de Déclencheur**

   1. **Sin pasos de espera**. Si elimina un paso normal, solo se verán afectadas las personas que realicen la campaña en el futuro.
   1. **Con pasos de espera**. Consulte el ejemplo siguiente para campañas por lotes. Se aplica la misma lógica.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >1. Una campaña inteligente tiene tres pasos.
   >    * PASO 1. Enviar #1 de correo electrónico
   >    * PASO 2. Esperar 1 semana
   >    * PASO 3. Enviar #2 de correo electrónico
   >
   >1. Las personas que toquen **Paso 2** esperarán 1 semana antes de pasar al **Paso 3**.
   >1. Usted elimina **Paso 2** durante la semana.
   >1. Las personas seguirán esperando la 1 semana (no vuelven a aparecer automáticamente en el flujo).
   >1. Cuando finalmente regresen, intentarán ir al **Paso 3**. No lo van a encontrar.
   >1. **IMPORTANTE:** Dado que ahora solo hay 2 pasos, las personas _no recibirán el correo electrónico #2_.
