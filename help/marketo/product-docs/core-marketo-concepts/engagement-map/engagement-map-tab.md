---
description: 'Pestaña Mapa de participación: Documentos de Marketo: documentación del producto'
title: Pestaña Mapa de participación
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: d41324dbde32ee731b3ce9c3416888e8088a2daa
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 0%

---

# Pestaña Mapa de participación {#engagement-map-tab}

El mapa de participación se representa mediante una serie de tarjetas de déclencheur, filtro y flujo. Al hacer clic en cada tarjeta, se muestra información adicional.

Información general sobre el déclencheur: Esta tarjeta muestra la cantidad de déclencheur en la campaña. Al hacer clic en él, se mostrará una tarjeta para cada déclencheur, así como un panel deslizable con la siguiente información:

* Campaña a la que pertenece el déclencheur
* Lista de nombres de déclencheur
* Editar Déclencheur

  ![](assets/engagement-map-tab-1.png)

Detalles del déclencheur: esta tarjeta muestra el nombre del déclencheur. Al hacer clic en él, se muestra un panel deslizable con la siguiente información:

* Campaña a la que pertenece el déclencheur
* Lista de restricciones asociadas al déclencheur
* Editar Déclencheur

Filtro: al hacer clic en esta tarjeta, se muestra un panel deslizable con la siguiente información:

* Campaña a la que pertenece el filtro
* Número estimado de personas que cumplen los requisitos para el filtro
* Lista de filtros y sus restricciones respectivas
* Editar filtro

  ![](assets/engagement-map-tab-3.png)

Pasos de flujo: si un paso de flujo incluye opciones, esta tarjeta mostrará el nombre del paso de flujo. Al hacer clic en él, se muestra un panel deslizable con la siguiente información:

* Campaña a la que pertenece el paso de flujo
* Lista de condiciones de elección asociadas al paso de flujo
* Editar paso de flujo

Pasos de flujo: Si un paso de flujo sí lo hace _no_ Si incluye cualquier opción, esta tarjeta mostrará los atributos asociados al paso de flujo. Al hacer clic en él, se muestra un panel deslizable con la siguiente información:

* Campaña a la que pertenece el paso de flujo
* Lista de atributos asociados al paso de flujo
* Editar paso de flujo

  ![](assets/engagement-map-tab-5.png)

## Paso de flujo para ejecutar y solicitar campañas {#flow-step-for-execute-and-request-campaigns}

* Si el paso Ejecutar o Solicitar flujo de campaña no incluye ninguna opción, la tarjeta mostrará el nombre de la campaña. Al hacer clic en la tarjeta, se muestra un panel deslizable con la siguiente información:

   * Campaña a la que pertenece el paso de flujo
   * Editar paso de flujo
   * Lista de atributos asociados al paso de flujo
   * Botón &quot;Ver lista&quot;, que abre una lista de campañas que utilizan la solicitud o ejecución de campaña específica

>[!NOTE]
>
>Puede editar los pasos de flujo desde una campaña principal. Para editar campañas anidadas, debe navegar a la campaña a través del vínculo en el panel deslizable.

* Si el paso Ejecutar o Solicitar flujo de campaña incluye opciones, al hacer clic en la tarjeta se muestra un panel deslizable con la siguiente información:

   * Campaña a la que pertenece el paso de flujo
   * Lista de condiciones de elección asociadas al paso de flujo
   * Editar paso de flujo

* Si una campaña de ejecución o solicitud incluye opciones, al hacer clic en la tarjeta de flujo se expandirá para mostrar todas las opciones en tarjetas individuales. Haciendo clic en _elección_ expandirá la campaña asociada a la opción específica, así como mostrará un panel deslizable con la siguiente información:

   * Campaña a la que pertenece la opción
   * Editar elección
   * Lista de condiciones de elección asociadas al paso de flujo
   * Ver lista, que abre una lista de campañas que utilizan la solicitud o ejecución de campaña específica

  ![](assets/engagement-map-tab-10.png)

## Visualización de una campaña de ejecución anidada {#visualizing-a-nested-execute-campaign}

Ejecute campañas ejecutadas en serie con la campaña principal. Las personas que cumplen los requisitos para una campaña ejecutable completan todos los pasos de flujo de la campaña y vuelven a la campaña principal para continuar con los pasos de flujo de esta campaña.

A continuación se muestra un ejemplo de una campaña inteligente, &quot;Campaña A&quot;, que incluye un paso de flujo de ejecución de campaña. Piense en la &quot;Campaña A&quot; como su campaña principal.

![](assets/engagement-map-tab-11.png)

1. Al hacer clic en la tarjeta Ejecutar flujo de campaña, se expandirá para mostrar los detalles de la &quot;Campaña B&quot;.
1. La &quot;Campaña B&quot; incluye un filtro que divide la audiencia en dos grupos: cualificada y no cualificada.
1. La audiencia cualificada pasa por los pasos de flujo asociados a la &quot;Campaña B&quot;.
1. Toda la audiencia (cualificada y no cualificada) vuelve a la &quot;Campaña A&quot; y pasa al siguiente paso de flujo.

   ![](assets/engagement-map-tab-12.png)

Puede hacer clic en el paso Ejecutar flujo de campaña en la &quot;Campaña B&quot;, que se expandirá para mostrar las tarjetas de opción y la campaña asociada con cada opción.

![](assets/engagement-map-tab-13.png)

## Visualización de campañas de solicitudes {#visualizing-request-campaign}

Solicitar campañas ejecutadas en paralelo con la campaña principal. Las personas que cumplen los requisitos para una campaña de solicitud completan todos los pasos de flujo de la campaña y luego abandonan la campaña. Al mismo tiempo, el mismo conjunto de personas pasa por los pasos de flujo desde la campaña principal.

Este es un ejemplo de campaña inteligente, &quot;Campaña A&quot;, que incluye un paso de flujo de campaña de solicitud. Piense en la &quot;Campaña A&quot; como su campaña principal.

![](assets/engagement-map-tab-14.png)

1. Al hacer clic en la tarjeta de flujo de campaña de solicitud, se ampliará para mostrar los detalles de la &quot;Campaña B&quot;
1. La &quot;Campaña B&quot; incluye un filtro que divide la audiencia en dos grupos: cualificada y no cualificada.
1. La audiencia cualificada pasa por los pasos de flujo asociados a la &quot;Campaña B&quot;.
1. Al mismo tiempo, toda la audiencia pasa a los siguientes pasos de flujo en la &quot;Campaña A&quot;.

   ![](assets/engagement-map-tab-15.png)

Puede profundizar en sus campañas anidadas si alguno de los pasos de flujo incluye otra campaña de solicitud haciendo clic en la tarjeta de flujo para ver los detalles de la campaña.

![](assets/engagement-map-tab-16.png)

Este es un ejemplo de una campaña de solicitudes con opciones.

![](assets/engagement-map-tab-17.png)

## Control de errores {#error-handling}

Los errores en las listas inteligentes y los pasos de flujo se resaltarán mediante un icono de error en la tarjeta. Además, se mostrará el mensaje de error correspondiente en el panel deslizable.

A continuación se muestra un ejemplo de error en un déclencheur que se muestra en la tarjeta Información general de déclencheur, el panel deslizable y la tarjeta déclencheur de detalles.

**Los errores en las tarjetas de filtro pueden incluir:**

* Error en la lista inteligente que hará que no se muestre la audiencia cualificada

* Error en la lógica del filtro

* Error en restricciones (o falta de ellas) en uno o más filtros

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>Los errores dentro de una campaña anidada no serán visibles hasta que haya hecho clic para expandir la campaña anidada.
