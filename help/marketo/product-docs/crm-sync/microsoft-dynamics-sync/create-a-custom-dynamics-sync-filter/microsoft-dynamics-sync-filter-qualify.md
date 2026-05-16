---
unique-page-id: 10092977
description: Obtenga información acerca del proceso de calificación del filtro de sincronización de Dynamics al convertir un posible cliente en un contacto. Comprenda cómo los valores del filtro de sincronización de contactos y posibles clientes afectan a la sincronización de Marketo.
title: 'Filtro de sincronización de Microsoft Dynamics: calificar'
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 124
ht-degree: 0%

---

# Filtro de sincronización de [!DNL Microsoft Dynamics]: calificar {#microsoft-dynamics-sync-filter-qualify}

Si desea convertir un posible cliente en un contacto de [!DNL Microsoft Dynamics], utilice este proceso de calificación predeterminado. A continuación, sincronícelo con Marketo.

## El proceso de conversión {#the-conversion-process}

| Si el filtro de sincronización de posibles clientes es: | y el filtro de sincronización de contactos es: | Este es el resultado en Marketo |
|---|---|---|
| [!UICONTROL Falso] | [!UICONTROL Falso] | No hay nada sincronizado en Marketo |
| [!UICONTROL Verdadero] | [!UICONTROL Verdadero] | El contacto se sincroniza en Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadero] | Se crea un nuevo registro de contacto en Marketo |
| [!UICONTROL Verdadero] | [!UICONTROL Falso] | [!DNL MS Dynamics] actualiza la información de posibles clientes en Marketo, pero el registro de contacto no está sincronizado |

>[!CAUTION]
>
>Solo admitimos el proceso de conversión Qualify listo para usar.
