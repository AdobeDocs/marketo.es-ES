---
unique-page-id: 10092969
description: Filtro de sincronización de Microsoft Dynamics - Combinar - Documentos de marketing - Documentación del producto
title: Filtro de sincronización de Microsoft Dynamics - Combinar
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Filtro de sincronización de Microsoft Dynamics: Combinar {#microsoft-dynamics-sync-filter-merge}

La combinación de leads en Microsoft Dynamics utiliza el tipo Dos opciones: Filtro de sincronización = Sí (VERDADERO) y Filtro de sincronización = No (FALSO). Cuando combina dos registros, el resultado varía según el registro que sea Verdadero y el que sea Falso.

Los registros de posibles clientes pasan a ser verdaderos o falsos según las reglas de flujo de trabajo definidas por el administrador para determinar el ganador. El filtro de sincronización para el registro ganador es lo que determina en última instancia si el registro de MS Dynamics se sincroniza con Marketing.

Es cuando un registro es verdadero y uno es falso que se vuelve complicado.

| Si el filtro de sincronización para el registro perdedor es: | y el filtro de sincronización para el registro ganador es: | Este es el resultado de Marketing |
|---|---|---|
| True | True | El registro ganador continúa sincronizándose con Marketing |
| False | False | El registro ganador continúa **no** sincronizándose con Marketing |
| False | True | El registro ganador se sincronizará con Marketing |
| True | False | El registro ganador no se sincronizará con Marketing |

