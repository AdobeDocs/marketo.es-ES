---
unique-page-id: 7515133
description: 'Sincronización SFDC: fusión de un posible cliente/contacto/persona - Marketo Docs - Documentación del producto'
title: 'Sincronización SFDC: fusión de un posible cliente/contacto/persona'
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Sincronización SFDC: Combinación de un posible cliente/contacto/persona {#sfdc-sync-merging-a-lead-contact-person}

A veces es mejor enumerar las reglas. Aquí vamos:

* Cuando combina dos posibles clientes en **Salesforce**, la sincronización normal indica a Marketo y los posibles clientes se combinan automáticamente como personas en Marketo.
* La combinación de dos personas en **Marketo** realmente invoca el mismo proceso que la combinación de dos personas como posibles clientes en Salesforce. Sigue funcionando automáticamente.
* La combinación de un **posible cliente (persona) en un contacto** funciona de la misma manera. Acabas con un solo contacto en ambos lados.
* Al combinar, se suma la puntuación predeterminada.

>[!NOTE]
>
>La combinación de 3 posibles clientes (personas) con puntuaciones de 10 cada uno, dará como resultado 1 posible cliente (persona) con una puntuación de 30.

* Los valores de campo en conflicto se toman del &quot;registro ganador&quot;. (Registro = el posible cliente o contacto resultante)
* Si el &quot;registro perdedor&quot; (el que está desapareciendo) tenía un valor y el registro ganador no tiene ninguno, conservaremos el registro perdedor. En otras palabras, &quot;Un valor es mejor que ningún valor&quot;.
* Se combinan todos los elementos del registro de actividades.

>[!NOTE]
>
>Análisis en profundidad para obtener más información sobre la [combinación de personas en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
