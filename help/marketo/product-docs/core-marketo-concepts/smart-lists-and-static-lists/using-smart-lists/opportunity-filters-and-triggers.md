---
unique-page-id: 8159286
description: 'Filtros y Déclencheur de oportunidad: documentos de Marketo, documentación del producto'
title: Filtros y Déclencheur de oportunidad
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Filtros y Déclencheur de oportunidad {#opportunity-filters-and-triggers}

Los filtros y déclencheur de oportunidad le permiten rastrear eventos de oportunidad de Salesforce. Son un poco diferentes en comparación con otros filtros y déclencheur.

## Filtros de oportunidad {#opportunity-filters}

Los filtros de oportunidad le permiten explorar en profundidad los posibles clientes de Salesforce que tienen oportunidades. Puede encontrarlas en la carpeta Oportunidades de la paleta al editar una lista inteligente. Vienen en algunos sabores.

* Cantidad de oportunidades
* Monto total de la oportunidad
* Ingreso esperado total de la oportunidad
* Tiene una oportunidad
* Se ha añadido la oportunidad
* Se ha eliminado la oportunidad
* Se actualizó la oportunidad

Si está buscando los campos de oportunidad (personalizados o estándar), utilice el **Tiene oportunidad** filtrar o **La oportunidad era`[Added/Removed/Updated]`** filtros o déclencheur.

**Número de Optys, Importe de Opty Total, Ingresos esperados de Opty Total**

Con estos filtros, puede encontrar posibles clientes en función del número total, la cantidad o los ingresos esperados de todas sus oportunidades.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Tiene oportunidad, Se agregó a la oportunidad, Se eliminó de la oportunidad**

Si está buscando posibles clientes que tengan oportunidades basadas en una combinación de criterios, utilice el **Tiene oportunidad**, **Se agregó a la oportunidad**, o **Se eliminó de la oportunidad** filtro. Ellos te dicen:

* **Tiene oportunidad**: Si este posible cliente tiene actualmente cualquier oportunidad coincidente
* **Se agregó a la oportunidad**: Si este posible cliente se añadió alguna vez a una oportunidad coincidente
* **Se eliminó de la oportunidad**: si este posible cliente se ha eliminado de una oportunidad coincidente

Agregar los criterios de búsqueda como **Restricciones** en el filtro. Las restricciones incluyen los campos estándar y personalizados de la oportunidad:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Por ejemplo, supongamos que desea encontrar posibles clientes que tengan oportunidades abiertas de al menos 5000 dólares. Arrastre en el **Tiene oportunidad** filtre y utilice el **Está cerrado** y **Cantidad** restricciones:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Cuando utiliza varios filtros de oportunidad, puede obtener respuestas incorrectas. Si crea el ejemplo anterior con dos filtros de oportunidad, obtendrá una lista de posibles clientes que tengan cualquier oportunidad que sea de al menos 5000 $ y cualquier oportunidad que se cierre, incluso si se trata de oportunidades independientes.

**Se actualizó la oportunidad**

El **Se actualizó la oportunidad** El filtro busca cualquier oportunidad cuando se actualiza un campo de oportunidad específico. Seleccione el campo que desea comprobar con el menú desplegable Atributo de Déclencheur y, a continuación, utilice las restricciones para reducir el conjunto de cambios.

Por ejemplo, este filtro le mostrará todos los posibles clientes a los que se les ha cambiado la fecha de cierre en los últimos 30 días:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Déclencheur de oportunidad {#opportunity-triggers}

Están disponibles los siguientes déclencheur de oportunidad. Funcionan igual que sus filtros correspondientes (descritos anteriormente), excepto que pueden almacenar en déclencheur las campañas justo cuando se produce el evento:

* La oportunidad está actualizada
* Se agregó a Oportunidad
* Se quitó de Oportunidad

Por ejemplo, puede utilizar esta lista inteligente para generar déclencheur cuando se agregue un posible cliente a una oportunidad. En el flujo, puede añadirlos a la lista de suspendidos de marketing o enviarles un correo electrónico de destino.

![](assets/image2015-6-11-12-3a33-3a48.png)

Para eliminar el déclencheur de los campos personalizados de la oportunidad, utilice el **Se ha actualizado la oportunidad** Seleccione el déclencheur y el campo en el menú desplegable:

![](assets/image2015-6-11-12-3a33-3a34.png)
