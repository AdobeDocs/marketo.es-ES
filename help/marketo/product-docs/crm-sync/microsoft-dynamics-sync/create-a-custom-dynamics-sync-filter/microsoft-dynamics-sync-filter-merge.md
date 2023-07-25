---
unique-page-id: 10092969
description: Filtro de sincronización de Microsoft Dynamics - Combinar - Documentos de Marketo - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: combinar'
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtro de sincronización de Microsoft Dynamics: Combinar {#microsoft-dynamics-sync-filter-merge}

La combinación de posibles clientes en Microsoft Dynamics utiliza el tipo Dos opciones: Sincronizar filtro = Sí (TRUE) y Sincronizar filtro = No (FALSE). Cuando se combinan dos registros, el resultado varía en función del registro que sea True y del registro que sea False.

Los registros de posibles clientes pasan a ser true o false en función de las reglas de flujo de trabajo definidas por el administrador para determinar el ganador. El filtro de sincronización del registro ganador es lo que determina en última instancia si el registro de MS Dynamics se sincroniza con Marketo.

Cuando un registro es verdadero y uno es falso es cuando se vuelve complicado.

| Si el filtro de sincronización para el registro de pérdida es: | y el filtro de sincronización para el registro ganador es: | Este es el resultado en Marketo |
|---|---|---|
| Verdadero | Verdadero | El registro ganador continúa sincronizándose con Marketo |
| Falso | Falso | El récord ganador continúa **no** sincronizar con Marketo |
| Falso | Verdadero | El registro ganador se sincronizará con Marketo |
| Verdadero | Falso | El registro ganador no se sincronizará con Marketo |
