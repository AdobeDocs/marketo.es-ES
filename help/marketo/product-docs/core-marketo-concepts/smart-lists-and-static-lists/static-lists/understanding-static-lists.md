---
unique-page-id: 2949891
description: 'Explicación de las listas estáticas: documentos de Marketo: documentación del producto'
title: Explicación de las listas estáticas
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 2%

---

# Explicación de las listas estáticas {#understanding-static-lists}

Las listas estáticas son una de las funciones más sencillas y útiles de Marketo. Son simplemente una lista de nombres de la base de datos. Encontrará muchas razones para usarlas.

>[!NOTE]
>
>Una sola persona en la base de datos puede estar en muchas listas estáticas diferentes.

La diferencia entre una lista estática y una lista inteligente es crucial para comprender.

| Tipo | Lógica |
|---|---|
| Lista inteligente | Basado en **reglas definidas** |
| Lista estática | Basado en **adición/eliminación de cada persona** |

>[!CAUTION]
>
>Uno de los errores más comunes es pensar que se puede eliminar a una persona de una lista simplemente &quot;eliminando a la persona&quot;. **Esto es incorrecto**. Al eliminar la persona, esta se eliminará de **toda la base de datos**, no solo la lista.

## Formas de agregar o eliminar personas de una lista {#ways-to-add-remove-people-from-a-list}

1. Paso de flujo de campaña inteligente ([Agregar a lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md), [Quitar de la lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md))

1. [Paso de flujo de acción único](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md)
1. Arrastrar personas a una lista del árbol
1. [Importación de lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)

## Algunos usos de una lista estática {#some-uses-of-a-static-list}

* Lista que se ha preseleccionado para recibir un mensaje de marketing.
* Una lista de &quot;competidores&quot; que utiliza para enviar mensajes de contrainteligencia maliciosos.
* Una lista temporal de personas en un estado concreto que luego las campañas inteligentes eliminan al salir de ese estado.

¡Disfruten del poder de la LISTA!

>[!MORELIKETHIS]
>
>[Crear una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)
