---
unique-page-id: 7515133
description: 'Sincronización de SFDC: combinación de un posible cliente/contacto/persona - Documentos de Marketo - Documentación del producto'
title: 'Sincronización de SFDC: combinación de un posible cliente/contacto/persona'
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

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
* Si el &quot;registro perdedor&quot; (el que está desapareciendo) tenía un valor y el registro ganador no tiene ninguno, mantendremos el registro perdedor. En otras palabras, &quot;Algún valor es mejor que ningún valor&quot;.
* Se combinan todos los elementos del registro de actividad.

>[!NOTE]
>
>Análisis profundo para obtener más información sobre [la combinación de personas en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
