---
description: Agregar o eliminar personas de su campaña de Dynamics Campaign - Marketo Docs - Documentación del producto
title: Agregar o quitar personas de la campaña de Dynamics
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# Agregar o eliminar personas de su campaña de Dynamics {#add-or-remove-people-from-your-dynamics-campaign}

## Agregar a Dynamics Campaign {#add-to-dynamics-campaign}

Este paso de flujo se puede utilizar en Campañas inteligentes de Marketo para agregar personas como posibles clientes o contactos en una campaña de Microsoft. Si el posible cliente aún no existe en Dynamics, se sincronizará automáticamente y se agregará a la campaña.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para Campañas de activación.

En la campaña inteligente, busque y seleccione la campaña de Dynamics a la que desee agregar a sus usuarios.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si no puede ver una campaña de Dynamics en la lista de campañas:
>
>* Asegúrese de que la sincronización de campañas funcione
>* La campaña no está activa en Microsoft Dynamics


El sistema crea automáticamente una lista de marketing estática específica de la campaña, cada una para posibles clientes y contactos, a la que añadir a la persona. Se trata de una acción única y, una vez para las sincronizaciones posteriores a la campaña, se utiliza la misma lista de marketing. El estándar de nomenclatura adoptado para el nombre estático de la Lista de marketing es `Mkto-leads-<uniqueID>` para posibles clientes y `Mkto-contacts-<uniqueID>` para contactos.

La asociación de estas Listas de marketing generadas por Marketo a otras campañas podría llevar a un comportamiento confuso. Por ejemplo: agregar a una campaña también resultaría en agregar a la segunda campaña. Tampoco se recomienda disociar la lista de marketing generada por Marketo de la campaña en Dynamics.

## Eliminar de Dynamics Campaign {#remove-from-dynamics-campaign}

Este paso de flujo se puede utilizar en Campañas inteligentes de Marketo para eliminar personas de una campaña de Microsoft. Esto elimina únicamente los posibles clientes de una campaña que se hayan agregado anteriormente a la campaña a través de la acción de flujo &quot;Añadido a Microsoft Campaign&quot;.

>[!NOTE]
>
>Esta acción de flujo solo está disponible para Campañas de activación.

En la campaña inteligente, busque y seleccione la campaña de Dynamics de la que desee eliminar a las personas.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si no ve una campaña de Dynamics en la lista de campañas:
>
>* Asegúrese de que la sincronización de campañas funcione
>* La campaña no está activa en Microsoft Dynamics

