---
unique-page-id: 10092977
description: Filtro de sincronización de Microsoft Dynamics - Cualificar - Documentos de marketing - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: calificar'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Filtro de sincronización de Microsoft Dynamics: Calificar {#microsoft-dynamics-sync-filter-qualify}

Cuando desee convertir un posible cliente en un contacto en Microsoft Dynamics, asegúrese de utilizar este proceso de cualificación predeterminado. A continuación, sincronícelo con Marketing.

## El proceso de conversión {#the-conversion-process}

A continuación se muestra cómo funcionan los filtros durante el proceso de conversión.

| Si el filtro de sincronización de posibles clientes es: | y el filtro de sincronización de contactos es: | Este es el resultado de Marketing |
|---|---|---|
| False | False | No se ha sincronizado nada en Marketing |
| True | True | El contacto se sincroniza en Marketing |
| False | True | Se crea un nuevo registro de contacto en Marketing |
| True | False | MS Dynamics actualiza la información de posibles clientes en Marketing, pero el registro de contactos no está sincronizado |

>[!CAUTION]
>
>Solo se admite el proceso de conversión de Cualificación lista para usar.

