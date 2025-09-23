---
unique-page-id: 10092969
description: Filtro de sincronización de Microsoft Dynamics - Combinar - Documentos de Marketo - Documentación del producto
title: Filtro de sincronización de Microsoft Dynamics - Combinar
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Filtro de sincronización de Dynamics [!DNL Microsoft]: Combinar {#microsoft-dynamics-sync-filter-merge}

La combinación de posibles clientes en [!DNL Microsoft Dynamics] usa el tipo de dos opciones: Sincronizar filtro = Sí (TRUE) y Sincronizar filtro = No (FALSE). Cuando se combinan dos registros, el resultado varía en función del registro que sea True y del registro que sea False.

Los registros de posibles clientes pasan a ser true o false en función de las reglas de flujo de trabajo definidas por el administrador para determinar el ganador. El filtro de sincronización del registro ganador es el que determina en última instancia si el registro [!DNL MS Dynamics] se sincroniza con Marketo.

Cuando un registro es verdadero y uno es falso es cuando se vuelve complicado.

| Si el filtro de sincronización para el registro de pérdida es: | y el filtro de sincronización para el registro ganador es: | Este es el resultado en Marketo |
|---|---|---|
| [!UICONTROL Verdadero] | [!UICONTROL Verdadero] | El registro ganador continúa sincronizándose con Marketo |
| [!UICONTROL Falso] | [!UICONTROL Falso] | El registro ganador continúa sincronizándose **no** con Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadero] | El registro ganador se sincronizará con Marketo |
| [!UICONTROL Verdadero] | [!UICONTROL Falso] | El registro ganador no se sincronizará con Marketo |
