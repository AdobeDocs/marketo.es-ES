---
description: Agregar o eliminar personas de su campaña de Dynamics Campaign - Documentos de Marketo - Documentación del producto
title: Agregar o quitar personas de la campaña de Dynamics
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Agregar o eliminar personas de su campaña de Dynamics {#add-or-remove-people-from-your-dynamics-campaign}

## Agregar a Dynamics Campaign {#add-to-dynamics-campaign}

Este paso de flujo se puede utilizar en Marketo Smart Campaigns para añadir personas como posibles clientes o contactos en una campaña de Microsoft. Si el posible cliente aún no existe en Dynamics, se sincronizará automáticamente y se agregará a la campaña.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para Campañas de Déclencheur.

En la campaña inteligente, busque y seleccione la campaña de Dynamics a la que desee agregar a sus usuarios.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si no puede ver una campaña de Dynamics en la lista de campañas:
>
>* Asegúrese de que la sincronización de campañas funcione
>* La campaña no está activa en Microsoft Dynamics


El sistema crea automáticamente una lista de marketing estática específica de la campaña, cada una para posibles clientes y contactos, a la que añadir a la persona. Se trata de una acción única y, una vez para las sincronizaciones posteriores a la campaña, se utiliza la misma lista de marketing. El estándar de nomenclatura adoptado para el nombre estático de la Lista de marketing es `Mkto-leads-<uniqueID>` para posibles clientes y `Mkto-contacts-<uniqueID>` para contactos.

La asociación de estas Listas de marketing generadas por Marketo a otras campañas podría dar lugar a comportamientos confusos. Por ejemplo: agregar a una campaña también resultaría en agregar a la segunda campaña. Tampoco se recomienda desvincular la lista de marketing generada por Marketo de la campaña en Dynamics.

## Eliminar de Dynamics Campaign {#remove-from-dynamics-campaign}

Este paso de flujo se puede utilizar en Marketo Smart Campaigns para eliminar personas de una campaña de Microsoft. Esto elimina únicamente los posibles clientes de una campaña que se hayan agregado anteriormente a la campaña a través de la acción de flujo &quot;Añadido a Microsoft Campaign&quot;.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para Campañas de Déclencheur.

En la campaña inteligente, busque y seleccione la campaña de Dynamics de la que desee eliminar a las personas.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si no ve una campaña de Dynamics en la lista de campañas:
>
>* Asegúrese de que la sincronización de campañas funcione
>* La campaña no está activa en Microsoft Dynamics

