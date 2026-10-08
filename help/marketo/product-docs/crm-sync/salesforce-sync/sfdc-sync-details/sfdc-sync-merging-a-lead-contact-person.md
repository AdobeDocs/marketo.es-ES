---
unique-page-id: 7515133
description: Comprenda cómo funciona la combinación de posibles clientes, contactos y personas en Salesforce y Marketo. Conozca las reglas de combinación para puntuaciones, valores de campo y registros de actividad.
title: 'Sincronización de SFDC: combinación de un posible cliente/contacto/persona'
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 3%
---
# Sincronización de SFDC: combinación de un posible cliente/contacto/persona {#sfdc-sync-merging-a-lead-contact-person}

A veces es mejor simplemente enumerar las reglas. Aquí vamos:

* Cuando combina dos posibles clientes en **[!DNL Salesforce]**, la sincronización normal indica a Marketo y los posibles clientes se combinan automáticamente como personas en Marketo.
* Al combinar dos personas en **Marketo**, se invoca el mismo proceso que al combinarlas como posibles clientes en [!DNL Salesforce]. Sigue funcionando automáticamente.
* Combinar un **posible cliente (persona) en un contacto** funciona de la misma manera. Termina con un solo contacto en ambos lados.
* Al combinar, se suma la puntuación predeterminada.

>[!NOTE]
>
>La combinación de 3 posibles clientes (personas) con puntuaciones de 10 cada una dará como resultado 1 posible cliente (persona) con una puntuación de 30.

* Los valores de campo que entran en conflicto se toman del &quot;registro ganador&quot;. (Registro = el posible cliente o contacto resultante)
* Si el &quot;registro perdedor&quot; (el que está desapareciendo) tenía un valor y el registro ganador no tiene ninguno (o es nulo), mantendremos el registro perdedor. En otras palabras, &quot;Algún valor es mejor que ningún valor&quot;.
* Se combinan todos los elementos del registro de actividad.

>[!MORELIKETHIS]
>
>Análisis profundo para obtener más información sobre [la combinación de personas en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
