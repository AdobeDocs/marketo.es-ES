---
unique-page-id: 8159286
description: Déclencheur y Filtros de oportunidad - Documentos de marketing - Documentación del producto
title: Filtros y Déclencheur de oportunidad
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Filtros y Déclencheur de oportunidad {#opportunity-filters-and-triggers}

Los filtros y déclencheur de oportunidad permiten rastrear los eventos de oportunidad de Salesforce. Son un poco diferentes en comparación con otros filtros y déclencheur.

## Filtros de oportunidad {#opportunity-filters}

Los filtros de oportunidad le permiten explorar en profundidad los posibles clientes de Salesforce que tienen oportunidades. Puede encontrarlos en la carpeta Oportunidades de la paleta al editar una lista inteligente. Vienen con algunos sabores.

* Número de opciones
* Importe total de la opción
* Total de ingresos esperados de opción
* Tiene oportunidad
* Se Añadió la oportunidad
* Se eliminó la oportunidad
* Se actualizó la oportunidad

Si está buscando los campos Oportunidad (personalizados o estándar), utilice el filtro **Tiene oportunidad** o **La oportunidad era`[Added/Removed/Updated]`** filtros o déclencheur.

**Número de opciones, cantidad total de la opción, total de ingresos esperados de la opción**

Con estos filtros, puede encontrar posibles clientes en función del número total, el importe o los ingresos esperados de todas sus oportunidades.

![](assets/image2015-6-11-12-3a29-3a34.png)

**La oportunidad, Añadida a la oportunidad, fue eliminada de la oportunidad**

Si busca posibles clientes que tengan oportunidades basadas en una combinación de criterios, utilice el filtro **Tiene oportunidad**, **Se Añadió a Oportunidad** o **Se eliminó del filtro de oportunidad**. Le dicen:

* **Tiene oportunidad**: Si este posible cliente tiene actualmente alguna oportunidad de coincidencia
* **Se Añadió a Oportunidad**: Si este lead alguna vez se agregó a una oportunidad de coincidencia
* **Se eliminó de la oportunidad**: Si este lead alguna vez se ha eliminado de una oportunidad de coincidencia

Añada los criterios de búsqueda como **Restricciones** en el filtro. Las restricciones incluyen los campos personalizados y estándar de oportunidad:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Por ejemplo: supongamos que desea encontrar posibles clientes que tengan oportunidades abiertas de al menos $5.000. Arrastre el filtro **Tiene oportunidad** y utilice las restricciones **Está cerrado** y **Importe**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Si utiliza varios filtros de oportunidad, puede obtener respuestas incorrectas. Si construyera el ejemplo anterior con dos filtros de oportunidad, obtendría una lista de posibles clientes que tengan cualquier oportunidad que sea de al menos $5,000 y cualquier oportunidad que esté cerrada, incluso si son oportunidades separadas.

**Se actualizó la oportunidad**

El filtro **Oportunidad actualizada** busca cualquier oportunidad cuando se actualizó un campo de oportunidad específico. Seleccione el campo que desea comprobar con el menú desplegable Atributo de Déclencheur y, a continuación, utilice las restricciones para reducir el conjunto de cambios.

Por ejemplo: este filtro le mostrará todos los leads que han tenido un cambio de fecha de cierre en los últimos 30 días:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Déclencheur de oportunidad {#opportunity-triggers}

Están disponibles los siguientes déclencheur de oportunidad. Funcionan igual que sus filtros correspondientes (descritos anteriormente), excepto que pueden déclencheur de campañas justo cuando se produce el evento:

* Se ha actualizado la oportunidad
* Añadido a oportunidad
* Eliminado de oportunidad

Por ejemplo, puede usar esta Lista inteligente para el déclencheur cuando se añada cualquier posible posible cliente a cualquier oportunidad. En el flujo, puede agregarlos a la lista Suspendido de marketing o enviarles un correo electrónico de destino.

![](assets/image2015-6-11-12-3a33-3a48.png)

Para déclencheur de los campos personalizados de oportunidad, utilice el déclencheur **Oportunidad actualizada** y seleccione el campo en el menú desplegable:

![](assets/image2015-6-11-12-3a33-3a34.png)
