---
unique-page-id: 7513680
description: 'Automatizar una alerta para posibles personas duplicadas: Documentos de Marketo: Documentación del producto'
title: Automatizar una alerta para posibles personas duplicadas
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 50fc46312d2c7c25556994fad4e118c01cf92fc0
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Automatizar una alerta para posibles personas duplicadas {#automate-an-alert-for-possible-duplicate-people}

¿Desea crear una alerta cada vez que se cree una persona duplicada? A continuación se muestra cómo configurar una campaña inteligente para hacerlo.

1. [Crear una nueva campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Defina la siguiente lista inteligente:

* Déclencheur: **Se crea la persona**
* Filtro: **Duplicar campos.** Nombre del campo **es Nombre completo**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >Sé creativo. Experimente con diferentes campos para obtener mejores resultados de filtrado.

1. En el paso de flujo, seleccione [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)Acción de flujo {target=&quot;_blank&quot;}.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Al usar la variable [Enviar token de información de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} para incluir un vínculo a la persona en su CRM.

   >[!CAUTION]
   >
   >Si importa una lista grande, puede obtener un montón de estas alertas a la vez.
   >
   >Además, dos personas con el mismo nombre no significa automáticamente que sean la misma persona.

1. Active la campaña en la **Programación** pestaña .

   ![](assets/automate-an-alert-3.png)

¡Eso es todo! Esta campaña inteligente se déclencheur cada vez que se cree una nueva persona con un nombre completo existente en Marketo.

>[!MORELIKETHIS]
>
>[Buscar y combinar personas duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
