---
unique-page-id: 2949891
description: 'Explicación de las listas estáticas: documentos de Marketo, documentación del producto'
title: Descripción de listas estáticas
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Descripción de listas estáticas {#understanding-static-lists}

Las listas estáticas son una de las funciones más sencillas y útiles de Marketo. Simplemente son una lista de nombres de la base de datos. Encontrará un montón de razones para usarlos.

>[!NOTE]
>
>Una sola persona de la base de datos puede estar en muchas listas estáticas diferentes.

La diferencia entre una lista estática y una lista inteligente es crucial para comprender.

| Tipo | Lógica |
|---|---|
| Lista inteligente | Basado en **reglas definidas** |
| Lista estática | Basado en **agregar o quitar cada persona** |

>[!CAUTION]
>
>Uno de los errores más comunes es pensar que se puede eliminar a una persona de una lista simplemente &quot;eliminándola&quot;. **Esto está mal**. Si se elimina a la persona, se eliminará de **toda la base de datos**, no solo la lista.

## Formas de agregar o quitar personas de una lista {#ways-to-add-remove-people-from-a-list}

1. Paso de flujo de campaña inteligente ([Añadir a lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Remove from List](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Paso de flujo de acción única](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Arrastrar personas a una lista del árbol
1. [Importación de lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Algunos usos de una lista estática {#some-uses-of-a-static-list}

* Una lista que se ha preseleccionado para recibir un mensaje de marketing.
* Una lista de &quot;competidores&quot; que utiliza para enviar mensajes maliciosos de contrainteligencia.
* Una lista temporal de personas en un estado particular, que luego son eliminadas por Campañas inteligentes cuando salen de ese estado.

¡Disfruta del poder de la LISTA!

>[!MORELIKETHIS]
>
>[Crear una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
