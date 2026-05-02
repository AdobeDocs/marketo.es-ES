---
unique-page-id: 2953188
description: Obtenga información sobre los filtros deducidos en las listas inteligentes. Comprender cómo Marketo infiere los filtros de los recursos vinculados.
title: Filtros inferidos
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

---

# Filtros inferidos {#inferred-filters}

Cuando alguien visita tu sitio web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} los cookies y los coloca en el sistema. El sistema busca su IP en una base de datos especial e infiere todo tipo de información.

>[!NOTE]
>
>Para garantizar que los valores de campo deducidos permanezcan actualizados, la base de datos utilizada para las búsquedas de direcciones IP se actualiza periódicamente. Las actualizaciones de la base de datos pueden introducir nuevos valores de campo deducidos que es posible que tenga que agregar a las definiciones de filtro de listas inteligentes.
>
>Las actualizaciones de la base de datos pueden producirse durante una [versión del producto Marketo Engage](/help/marketo/release-notes/release-schedule.md){target="_blank"}. Cuando se produce una actualización, las [notas de la versión de Marketo Engage](/help/marketo/release-notes/current.md){target="_blank"} contendrán una explicación de los cambios realizados en los valores de los campos deducidos.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

Cuando se utiliza cualquiera de estos filtros en una lista inteligente, los resultados muestran esta información deducida.

>[!TIP]
>
>Utilice estos filtros en un informe de actividad web. Utilice los territorios de los representantes de ventas y suscríbalos a un informe diario personalizado con los visitantes del sitio web en las últimas 24 horas. ¡Les encantará!
>
>* Página web visitada: últimas 24 horas
>* El estado deducido es [seleccione su territorio]

Estos visitantes anónimos se convierten automáticamente en personas cuando hacen clic en un vínculo de correo electrónico o rellenan un formulario. Sin embargo, conservan toda la información deducida.

>[!NOTE]
>
>Más información sobre [actividad anónima y posibles clientes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
