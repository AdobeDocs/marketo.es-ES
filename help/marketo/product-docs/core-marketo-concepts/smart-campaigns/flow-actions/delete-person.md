---
unique-page-id: 1147082
description: Eliminar persona - Documentos de Marketo - Documentación del producto
title: Eliminar persona
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 4%

---

# Eliminar persona {#delete-person}

Las personas erróneas a veces entran en la base de datos. El paso de flujo Eliminar persona puede deshacerse de ellos.

## Información general {#overview}

Utilice el paso de flujo en una campaña inteligente.

![](assets/one-4.png)

>[!CAUTION]
>
>Al eliminar una persona, también se eliminarán todos sus datos RCE históricos. No se puede deshacer.

## Uso {#usage}

Al arrastrar el paso de flujo, también se establecerá automáticamente para eliminarlo de su CRM.

![](assets/two-4.png)

Puede eliminar de Marketo y no de su CRM, de esta manera:

![](assets/three-3.png)

>[!NOTE]
>
>Eliminación de la persona de su CRM **solo funciona con Salesforce**. Si elimina a una persona de Marketo y decide mantenerla en Salesforce, se volverá a crear en Marketo si en algún momento se actualiza su registro de Salesforce.
