---
unique-page-id: 10092977
description: Filtro de sincronización de Microsoft Dynamics - Calificar - Documentos de Marketo - Documentación del producto
title: 'Filtro de sincronización de Microsoft Dynamics: calificar'
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 0%

---

# Filtro de sincronización de [!DNL Microsoft Dynamics]: calificar {#microsoft-dynamics-sync-filter-qualify}

Si desea convertir un posible cliente en un contacto de [!DNL Microsoft Dynamics], asegúrese de utilizar este proceso de calificación predeterminado. A continuación, sincronícelo con Marketo.

## El proceso de conversión {#the-conversion-process}

Así es como funcionan los filtros durante el proceso de conversión.

| Si el filtro de sincronización de posibles clientes es: | y el filtro de sincronización de contactos es: | Este es el resultado en Marketo |
|---|---|---|
| [!UICONTROL Falso] | [!UICONTROL Falso] | No hay nada sincronizado en Marketo |
| [!UICONTROL Verdadero] | [!UICONTROL Verdadero] | El contacto se sincroniza en Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadero] | Se crea un nuevo registro de contacto en Marketo |
| [!UICONTROL Verdadero] | [!UICONTROL Falso] | [!DNL MS Dynamics] actualiza la información de posibles clientes en Marketo, pero el registro de contacto no está sincronizado |

>[!CAUTION]
>
>Solo admitimos el proceso de conversión Qualify listo para usar.
