---
unique-page-id: 8159286
description: 'Filtros y Déclencheur de oportunidad: documentos de Marketo, documentación del producto'
title: Filtros y Déclencheur de oportunidad
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 5%

---

# Filtros y Déclencheur de oportunidad {#opportunity-filters-and-triggers}

Los filtros y déclencheur de oportunidad le permiten rastrear eventos de oportunidad de Salesforce. Son un poco diferentes en comparación con otros filtros y déclencheur.

## Filtros de oportunidad {#opportunity-filters}

Los filtros de oportunidad le permiten explorar en profundidad los posibles clientes de Salesforce que tienen oportunidades. Puede encontrarlas en la carpeta Oportunidades de la paleta al editar una lista inteligente. Vienen en algunos sabores.

* Cantidad de oportunidades
* Monto total de la oportunidad
* Ingreso esperado total de la oportunidad
* Tiene oportunidad
* Se ha añadido la oportunidad
* Se ha eliminado la oportunidad
* Se actualizó la oportunidad

Si estás buscando tus campos de oportunidad (personalizados o estándar), usa el filtro **Tiene oportunidad** o **La oportunidad era`[Added/Removed/Updated]`** filtros o déclencheur.

**Número de opciones, Importe total de la opción, Ingresos totales esperados de la opción**

Con estos filtros, puede encontrar posibles clientes en función del número total, la cantidad o los ingresos esperados de todas sus oportunidades.

![](assets/opportunity-filters-and-triggers-1.png)

**Tiene oportunidad, Se agregó a la oportunidad, Se eliminó de la oportunidad**

Si está buscando posibles clientes que tienen oportunidades basadas en una combinación de criterios, use el filtro **Tiene oportunidad**, **Se agregó a la oportunidad** o **Se eliminó de la oportunidad**. Ellos te dicen:

* **Tiene oportunidad**: Si este posible cliente tiene actualmente alguna oportunidad coincidente
* **Se agregó a la oportunidad**: Si este posible cliente se agregó alguna vez a una oportunidad coincidente
* **Se eliminó de la oportunidad**: Si este posible cliente se eliminó alguna vez de una oportunidad coincidente

Agregue los criterios de búsqueda como **Restricciones** en el filtro. Las restricciones incluyen los campos estándar y personalizados de la oportunidad:

![](assets/opportunity-filters-and-triggers-2.png)

![](assets/opportunity-filters-and-triggers-3.png)

Por ejemplo, supongamos que desea encontrar posibles clientes que tengan oportunidades abiertas de al menos 5000 dólares. Arrastre el filtro **Tiene oportunidad** y use las restricciones **Está cerrado** y **Cantidad**:

![](assets/opportunity-filters-and-triggers-4.png)

>[!NOTE]
>
>Cuando utiliza varios filtros de oportunidad, puede obtener respuestas incorrectas. Si crea el ejemplo anterior con dos filtros de oportunidad, obtendrá una lista de posibles clientes que tengan cualquier oportunidad que sea de al menos 5000 $ y cualquier oportunidad que se cierre, incluso si se trata de oportunidades independientes.

**Se actualizó la oportunidad**

El filtro **Se actualizó la oportunidad** busca cualquier oportunidad cuando se actualizó un campo de oportunidad específico. Seleccione el campo que desea comprobar con el menú desplegable Atributo de Déclencheur y, a continuación, utilice las restricciones para reducir el conjunto de cambios.

Por ejemplo, este filtro le mostrará todos los posibles clientes a los que se les ha cambiado la fecha de cierre en los últimos 30 días:

![](assets/opportunity-filters-and-triggers-5.png)

## Déclencheur de oportunidad {#opportunity-triggers}

Están disponibles los siguientes déclencheur de oportunidad. Funcionan igual que sus filtros correspondientes (descritos anteriormente), excepto que pueden almacenar en déclencheur las campañas justo cuando se produce el evento:

* La oportunidad está actualizada
* Se agregó a Oportunidad
* Se quitó de Oportunidad

Por ejemplo, puede utilizar esta lista inteligente para generar déclencheur cuando se agregue un posible cliente a una oportunidad. En el flujo, puede añadirlos a la lista de suspendidos de marketing o enviarles un correo electrónico de destino.

![](assets/opportunity-filters-and-triggers-6.png)

Déclencheur Para desactivar los campos personalizados de oportunidad, usa el déclencheur **Se ha actualizado la oportunidad** y elige el campo en el menú desplegable:

![](assets/opportunity-filters-and-triggers-7.png)
