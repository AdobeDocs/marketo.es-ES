---
description: Agregar o quitar personas de su  [!DNL Dynamics] campaña - Documentos de Marketo - Documentación del producto
title: Agregar o quitar personas de su campaña  [!DNL Dynamics] Campaign
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Agregar o quitar personas de su campaña [!DNL Dynamics] {#add-or-remove-people-from-your-dynamics-campaign}

## Añadir a Dynamics Campaign {#add-to-dynamics-campaign}

Este paso de flujo se puede utilizar en Marketo Engage Smart Campaigns para agregar personas como posibles clientes o contactos en una campaña de Microsoft. Si el posible cliente aún no existe en Dynamics, se sincronizará automáticamente y se agregará a la campaña.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para campañas de Déclencheur.

En su campaña inteligente, busque y seleccione la campaña de Dynamics a la que desee agregar a sus recursos.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si no puede ver una campaña de Dynamics en la lista de campañas:
>
>* Asegúrese de que la sincronización de Campaign funcione
>* La campaña no está activa en [!DNL Microsoft Dynamics]

El sistema crea automáticamente una lista de marketing estática específica de la campaña, cada una para posibles clientes y contactos, a la que se agregará la persona. Es una acción única y, una vez para las sincronizaciones posteriores a la campaña, se utiliza la misma lista de marketing. El estándar de nomenclatura adoptado para el nombre estático de la lista de marketing es `Mkto-leads-<uniqueID>` para los posibles clientes y `Mkto-contacts-<uniqueID>` para los contactos.

La asociación de estas listas de marketing generadas por Marketo con otras campañas podría generar comportamientos confusos. Por ejemplo: añadir a una campaña también resultaría en añadir a la segunda campaña. Del mismo modo, tampoco se recomienda disociar la lista de marketing generada por Marketo de la campaña en [!DNL Dynamics].

## Eliminar de Dynamics Campaign {#remove-from-dynamics-campaign}

Este paso de flujo se puede utilizar en Marketo Smart Campaigns para eliminar personas de una campaña de Microsoft. Esto elimina solo los posibles clientes de una campaña que se han añadido previamente a la campaña mediante la acción de flujo &quot;Añadido a la campaña de Microsoft&quot;.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para campañas de Déclencheur.

En la campaña inteligente, busque y seleccione la campaña de Dynamics de la que desee eliminar a sus recursos.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si no ve una campaña [!DNL Dynamics] en la lista de campañas:
>
>* Asegúrese de que la sincronización de Campaign funcione
>* La campaña no está activa en [!DNL Microsoft Dynamics]
