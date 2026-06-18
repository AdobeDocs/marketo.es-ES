---
unique-page-id: 7515133
description: Comprenda cómo funciona la combinación de posibles clientes, contactos y personas en Salesforce y Marketo. Conozca las reglas de combinación para puntuaciones, valores de campo y registros de actividad.
title: 'Sincronización de SFDC: combinación de un posible cliente/contacto/persona'
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 25bbf4409df3db38b849d936e2a90b48f859d089
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 2%

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

>[!NOTE]
>
>El comportamiento de los campos booleanos en una combinación de API cambió en la versión de marzo de 2026. Ahora, un valor False se trata correctamente como si tuviera un valor para ese campo. Solo un valor nulo se trata como &quot;vacío&quot; al evaluar campos en conflicto. Ver [esta publicación de la comunidad](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219){target="_blank"} más detalles.

>[!MORELIKETHIS]
>
>Análisis profundo para obtener más información sobre [la combinación de personas en Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
