---
unique-page-id: 10092977
description: Filtro de sincronización de Microsoft Dynamics - Cualificar - Documentos de Marketo - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: calificar'
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Filtro de sincronización de Microsoft Dynamics: Calificar {#microsoft-dynamics-sync-filter-qualify}

Cuando desee convertir un posible cliente a un contacto en Microsoft Dynamics, asegúrese de utilizar este proceso de certificación predeterminado. A continuación, sincronícelo con Marketo.

## El proceso de conversión {#the-conversion-process}

A continuación se muestra cómo funcionan los filtros durante el proceso de conversión.

| Si el filtro de sincronización de posibles clientes es: | y el filtro de sincronización de contactos es: | Este es el resultado de Marketo |
|---|---|---|
| False | False | No hay nada sincronizado en Marketo |
| True | True | El contacto se sincroniza en Marketo |
| False | True | Se crea un nuevo registro de contacto en Marketo |
| True | False | MS Dynamics actualiza la información del posible cliente en Marketo, pero el registro de contacto no está sincronizado |

>[!CAUTION]
>
>Solo admitimos el proceso de conversión de Cualificación predeterminado.
