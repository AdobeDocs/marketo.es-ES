---
unique-page-id: 10092969
description: Filtro de sincronización de Microsoft Dynamics - Combinar - Documentos de Marketo - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: combinar'
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtro de sincronización de Microsoft Dynamics: Combinar {#microsoft-dynamics-sync-filter-merge}

La combinación de posibles clientes en Microsoft Dynamics utiliza el tipo Dos opciones: Filtro de sincronización = Sí (TRUE) y Filtro de sincronización = No (FALSE). Al combinar dos registros, el resultado varía según el registro que sea Verdadero y el que sea Falso.

Los registros de posibles clientes pasan a ser verdaderos o falsos, según las reglas de flujo de trabajo definidas por el administrador para determinar el ganador. El filtro de sincronización para el registro ganador es lo que determina finalmente si el registro de MS Dynamics se sincroniza con Marketo.

Es cuando un registro es verdadero y uno es falso que se vuelve complicado.

| Si el filtro de sincronización para el registro perdedor es: | y el filtro de sincronización para el registro ganador es: | Este es el resultado de Marketo |
|---|---|---|
| True | True | El registro ganador continúa sincronizándose con Marketo |
| False | False | El registro ganador continúa **not** sincronizar con Marketo |
| False | True | El registro ganador se sincronizará con Marketo |
| True | False | El registro ganador no se sincronizará con Marketo |
