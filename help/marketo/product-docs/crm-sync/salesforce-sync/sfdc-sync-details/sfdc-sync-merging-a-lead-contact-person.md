---
unique-page-id: 7515133
description: Sincronización de SFDC - Combinación de un posible cliente/contacto/persona - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: combinación de un posible cliente, contacto o persona'
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincronización SFDC: Combinación de un posible cliente/contacto/persona {#sfdc-sync-merging-a-lead-contact-person}

A veces es mejor sólo lista las reglas. Aquí vamos:

* Cuando combina dos leads en **Salesforce**, la sincronización normal indica a Marketing y los leads se combinan automáticamente como personas en Marketing.
* La combinación de dos personas en **Marketing** realmente invoca el mismo proceso que la combinación de dos personas como posibles clientes en Salesforce. Todavía funciona automáticamente.
* La combinación de un **lead (persona) en un contacto** funciona de la misma manera. Uno termina con un solo contacto en ambos lados.
* Al combinar, se suma la puntuación predeterminada.

>[!NOTE]
>
>La combinación de 3 posibles clientes (personas) con puntuaciones de 10 cada uno, dará como resultado 1 posible (persona) con una puntuación de 30.

* Los valores de campo en conflicto se toman del &quot;registro ganador&quot;. (Registro = el posible cliente o contacto resultante)
* Si el &quot;registro perdedor&quot; (el que está desapareciendo) tuviera un valor y el registro ganador no tuviera ninguno, mantendremos el registro perdedor. En otras palabras, &quot;Algún valor es mejor que ningún valor&quot;.
* Todos los elementos del registro de actividades se combinan.

>[!NOTE]
>
>Bucear profundo para obtener más información sobre [la combinación de personas en Marketing](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
