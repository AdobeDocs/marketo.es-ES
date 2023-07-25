---
unique-page-id: 7515133
description: 'Sincronización de SFDC: fusión de un posible cliente/contacto/persona - Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: combinación de un posible cliente/contacto/persona'
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Sincronización de SFDC: combinación de un posible cliente/contacto/persona {#sfdc-sync-merging-a-lead-contact-person}

A veces es mejor simplemente enumerar las reglas. Aquí vamos:

* Cuando combina dos posibles clientes en **Salesforce**, la sincronización normal indica a Marketo y que los posibles clientes se combinan automáticamente como personas en Marketo.
* Combinación de dos personas en **Marketo** en realidad invoca el mismo proceso que combinarlos como posibles clientes en Salesforce. Sigue funcionando automáticamente.
* Combinación de un **dirigir (persona) a un contacto** funciona del mismo modo. Termina con un solo contacto en ambos lados.
* Al combinar, se suma la puntuación predeterminada.

>[!NOTE]
>
>La combinación de 3 posibles clientes (personas) con puntuaciones de 10 cada una dará como resultado 1 posible cliente (persona) con una puntuación de 30.

* Los valores de campo que entran en conflicto se toman del &quot;registro ganador&quot;. (Registro = el posible cliente o contacto resultante)
* Si el &quot;registro perdedor&quot; (el que está desapareciendo) tenía un valor y el registro ganador no tiene ninguno, mantendremos el registro perdedor. En otras palabras, &quot;Algún valor es mejor que ningún valor&quot;.
* Se combinan todos los elementos del registro de actividad.

>[!NOTE]
>
>Inmersión profunda para obtener más información sobre [combinación de personas en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
