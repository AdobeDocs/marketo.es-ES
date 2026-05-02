---
unique-page-id: 2949891
description: Obtenga información sobre las listas estáticas en Marketo para conjuntos fijos de personas. Utilice listas estáticas cuando la suscripción se administre manualmente.
title: Descripción de las listas estáticas
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 5%

---

# Descripción de las listas estáticas {#understanding-static-lists}

Las listas estáticas son una de las funciones más sencillas y útiles de Marketo. Son una lista de nombres de la base de datos. Encontrará un montón de razones para usarlos.

>[!NOTE]
>
>Una sola persona de la base de datos puede estar en muchas listas estáticas diferentes.

La diferencia entre una lista estática y una lista inteligente es crucial para comprender.

| Tipo | Lógica |
|---|---|
| Lista inteligente | Según **reglas definidas** |
| Lista estática | Basado en **agregar o quitar cada persona** |

>[!CAUTION]
>
>Uno de los errores más comunes es pensar que se puede eliminar a una persona de una lista &quot;eliminando a la persona&quot;. **Esto no es correcto**. Si se elimina a la persona, se eliminará de **toda la base de datos**, no solo de la lista.

## Formas de agregar o quitar personas de una lista {#ways-to-add-remove-people-from-a-list}

1. Paso de flujo de campaña inteligente ([Agregar a lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Quitar de lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Paso de flujo de acción única](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Arrastrar personas a una lista del árbol
1. [Importación de lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Algunos usos de una lista estática {#some-uses-of-a-static-list}

* Una lista que se ha preseleccionado para recibir un mensaje de marketing.
* Una lista de &quot;competidores&quot; que utiliza para enviar mensajes maliciosos de contrainteligencia.
* Una lista temporal de personas en un estado particular, que luego son eliminadas por Campañas inteligentes cuando salen de ese estado.

>[!MORELIKETHIS]
>
>[Crear una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
