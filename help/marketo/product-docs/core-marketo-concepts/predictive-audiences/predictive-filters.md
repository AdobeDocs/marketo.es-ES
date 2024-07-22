---
description: 'Filtros predictivos: documentos de Marketo, documentación del producto'
title: Filtros predictivos
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 3%

---

# Filtros predictivos {#predictive-filters}

Como parte de Predictive Audiences, Marketo ofrece un grupo de filtros basados en IA/ML en listas inteligentes dentro de campañas inteligentes.

![Imagen uno](assets/predictive-filters-1.png)

>[!NOTE]
>
>Los filtros &quot;Probabilidad de asistencia&quot; y &quot;Probabilidad de registro&quot; solo se pueden usar en Programas de eventos. &quot;Probabilidad de cancelar la suscripción&quot;, &quot;Similitud de miembros del programa&quot; y &quot;Similitud de miembros de listas inteligentes&quot; se pueden utilizar en todos los tipos de programas.

## Probabilidad de asistir {#likelihood-to-attend}

Este filtro se utiliza para reducir la audiencia de forma eficaz. Esto le ayuda a dirigir e invitar a posibles clientes que tienen una mayor probabilidad de **asistir** a su seminario web o evento. Tenga en cuenta que su &quot;Probabilidad de asistir al programa&quot; será su programa de evento actual.

![Imagen dos](assets/predictive-filters-2.png)

## Probabilidad de registrarse {#likelihood-to-register}

De manera similar al filtro _Probabilidad de asistir_, usa este filtro para reducir tu audiencia y segmentar a los posibles clientes que tengan una mayor probabilidad de **registrarse** en tu seminario web o evento.

![Imagen tres](assets/predictive-filters-3.png)

## Probabilidad de cancelar la subscripción {#likelihood-to-unsubscribe}

Esto filtra la audiencia según si tienen una probabilidad alta o baja de cancelar la suscripción en las próximas dos semanas. Puede usar esto para dirigirse a los posibles clientes con alta fatiga de forma diferente y más eficaz. El umbral de cancelación de suscripción es dinámico y está impulsado por un modelo de IA que considera varios atributos, incluido el tiempo de espera en la base de datos y las actividades de posible cliente.

![Imagen Cuatro](assets/predictive-filters-4.png)

>[!NOTE]
>
>Los filtros Probabilidad de asistencia, registro y cancelación de suscripción deben utilizarse junto con otros filtros estándar.

## Similitud de miembros del programa/Similitud de miembros de listas inteligentes {#lookalike-of-members}

Estos dos filtros le ayudan a ampliar su audiencia actual al dirigirse a posibles clientes adicionales similares a los miembros de otro programa o lista inteligente. Los filtros de similitud tienen en cuenta más de 50 factores, incluidos los atributos de los posibles clientes, la actividad de correo electrónico, la actividad web y la participación.

Haga clic en **[!UICONTROL Agregar restricción]** para elegir criterios de éxito para los miembros de los programas seleccionados.

Haga clic en el icono **+** para agregar fácilmente varios programas o listas inteligentes a un filtro.

![Imagen Cinco](assets/predictive-filters-5.png)

## Cosas que hay que tener en cuenta {#things-to-note}

* Puede aplicar filtros predictivos a una campaña inteligente incluso si el programa principal se crea antes de habilitar los filtros predictivos.
* Los filtros predictivos no están disponibles para campañas de Déclencheur.
* No se admite la clonación o el traslado de campañas que contengan filtros predictivos.
* Puede usar hasta cinco filtros predictivos en una lista inteligente.
* Si el Marketo Engage encuentra un error en la evaluación de filtros predictivos, la ejecución de la campaña se interrumpirá automáticamente y recibirá una notificación en el centro de notificaciones de Marketo.
* Los filtros predictivos tienen actualmente un límite de entrada de 1 millón de personas cualificadas.
* Puede tener hasta 50 programas activos con filtros predictivos.
