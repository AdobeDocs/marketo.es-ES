---
unique-page-id: 1147082
description: Obtenga información sobre cómo eliminar una persona de la base de datos con un paso de flujo. Elimine las personas que cumplan los criterios de Marketo.
title: Eliminar persona
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 3%

---

# Eliminar persona {#delete-person}

Las personas erróneas a veces entran en la base de datos. El paso de flujo Eliminar persona puede deshacerse de ellos.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Al eliminar una persona, también se eliminarán todos sus datos RCE históricos. No se puede deshacer.

1. Al arrastrar el paso de flujo, también se establecerá automáticamente para eliminarlo de su CRM.

   ![](assets/delete-person-2.png)

1. Puede eliminar de Marketo Engage y no de su CRM, de esta manera:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Quitar a la persona de su CRM _solo funciona con[!DNL Salesforce]_. Si elimina a una persona de Marketo y decide mantenerla en [!DNL Salesforce], se volverá a crear en Marketo si se actualiza su registro [!DNL Salesforce].
