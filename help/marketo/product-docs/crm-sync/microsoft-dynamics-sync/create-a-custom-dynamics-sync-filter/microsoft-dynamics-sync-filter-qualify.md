---
unique-page-id: 10092977
description: Filtro de sincronización de Microsoft Dynamics - Calificar - Documentos de Marketo - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: calificar'
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Filtro de sincronización de Microsoft Dynamics: Calificar {#microsoft-dynamics-sync-filter-qualify}

Si desea convertir un posible cliente en un contacto en Microsoft Dynamics, asegúrese de utilizar este proceso de calificación predeterminado. A continuación, sincronícelo con Marketo.

## El proceso de conversión {#the-conversion-process}

Así es como funcionan los filtros durante el proceso de conversión.

| Si el filtro de sincronización de posibles clientes es: | y el filtro de sincronización de contactos es: | Este es el resultado en Marketo |
|---|---|---|
| Falso | Falso | No hay nada sincronizado en Marketo |
| Verdadero | Verdadero | El contacto se sincroniza en Marketo |
| Falso | Verdadero | Se crea un nuevo registro de contacto en Marketo |
| Verdadero | Falso | MS Dynamics actualiza la información del posible cliente en Marketo, pero el registro de contacto no está sincronizado |

>[!CAUTION]
>
>Solo admitimos el proceso de conversión Qualify listo para usar.
