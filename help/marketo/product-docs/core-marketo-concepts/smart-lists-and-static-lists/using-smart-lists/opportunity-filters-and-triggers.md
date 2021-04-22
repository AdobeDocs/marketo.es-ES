---
unique-page-id: 8159286
description: 'Filtros y Déclencheur de oportunidad: Documentos de Marketo: Documentación del producto'
title: Filtros y Déclencheur de oportunidad
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filtros y Déclencheur de oportunidad {#opportunity-filters-and-triggers}

Los filtros y déclencheur de oportunidad permiten rastrear eventos de oportunidad de Salesforce. Son un poco diferentes en comparación con otros filtros y déclencheur.

## Filtros de oportunidad {#opportunity-filters}

Los filtros de oportunidad le permiten explorar en profundidad los posibles clientes de Salesforce que tienen oportunidades. Puede encontrarlos en la carpeta Oportunidades de la paleta al editar una lista inteligente. Vienen con algunos sabores.

* Número de opciones
* Cantidad total de Opt
* Total de ingresos esperados de Opty
* Tiene oportunidad
* Se añadió la oportunidad
* Se ha eliminado la oportunidad
* Se actualizó la oportunidad

Si está buscando los campos de oportunidad (personalizados o estándar), utilice el filtro **Tiene oportunidad** o **La oportunidad era`[Added/Removed/Updated]`** filtros o déclencheur.

**Número de optys, cantidad total de opty, total de ingresos esperados de opty**

Con estos filtros, puede encontrar posibles clientes en función del número total, la cantidad o los ingresos esperados de todas sus oportunidades.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Tiene oportunidad, se agregó a la oportunidad, se eliminó de la oportunidad**

Si está buscando posibles clientes que tengan oportunidades basadas en una combinación de criterios, utilice el filtro **Tiene oportunidad**, **Se agregó a la oportunidad** o **Se eliminó del filtro de oportunidad**. Le dicen:

* **Tiene oportunidad**: Si este posible cliente tiene actualmente alguna oportunidad coincidente
* **Se agregó a la oportunidad**: Si este posible cliente alguna vez se agrega a una oportunidad coincidente
* **Se eliminó de la oportunidad**: Si este posible cliente se elimina de una oportunidad coincidente

Agregue los criterios de búsqueda como **Restrictions** en el filtro. Las restricciones incluyen los campos personalizados y estándar de oportunidad:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Por ejemplo, supongamos que desea encontrar posibles clientes que tengan oportunidades abiertas de al menos 5000 dólares. Arrastre el filtro **Tiene oportunidad** y utilice las restricciones **Está cerrado** y **Importe**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Cuando utiliza varios filtros de oportunidad, puede obtener respuestas incorrectas. Si creara el ejemplo anterior con dos filtros de oportunidad, obtendría una lista de posibles clientes que tengan cualquier oportunidad que sea de al menos $5,000 y cualquier oportunidad que se cierre, incluso si son oportunidades separadas.

**Se actualizó la oportunidad**

El filtro **Oportunidad actualizada** busca cualquier oportunidad cuando se actualizó un campo de oportunidad específico. Elija el campo que desea comprobar con el menú desplegable Atributo de Déclencheur y, a continuación, utilice las restricciones para reducir el conjunto de cambios.

Por ejemplo, este filtro muestra todos los posibles clientes que han cambiado su fecha de cierre en los últimos 30 días:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Déclencheur de oportunidad {#opportunity-triggers}

Los siguientes déclencheur de oportunidad están disponibles. Funcionan igual que los filtros correspondientes (descritos anteriormente), excepto que pueden almacenar en déclencheur las campañas justo cuando se produce el evento:

* Se ha actualizado la oportunidad
* Se ha agregado a Oportunidad
* Eliminada de oportunidad

Por ejemplo, puede utilizar esta lista inteligente para almacenar en déclencheur cuando se añada cualquier posible cliente a cualquier oportunidad. En el flujo, puede agregarlos a la lista de Marketing suspendido o enviarles un correo electrónico de destino.

![](assets/image2015-6-11-12-3a33-3a48.png)

Para obtener el déclencheur de los campos personalizados de oportunidad, utilice el déclencheur **Oportunidad actualizada** y seleccione el campo en la lista desplegable:

![](assets/image2015-6-11-12-3a33-3a34.png)
