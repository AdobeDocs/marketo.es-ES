---
description: Configure la sección Base de datos para la nueva instancia de Marketo Engage.
title: 'Nuevas prácticas recomendadas para instancias: lista de comprobación de bases de datos'
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 9%

---

# Nuevas Prácticas Recomendadas Para Instancias: Lista De Comprobación De Bases De Datos {#new-instance-best-practices-database-checklist}

La sección Base de datos es donde encontrará los atributos clave de las personas de la instancia. Obtenga más información sobre los pasos necesarios para navegar por diferentes listas y segmentaciones de la base de datos, así como para administrar registros de personas.

Recuerde [descargar las listas de comprobación](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) y realizar un seguimiento de su progreso.

## Listas inteligentes del sistema {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Todas las personas</td>
    <td><li>Determine la implementación de una sincronización 1:1 con su CRM o la aplicación de filtros para limitar quién se mueve de un sistema a otro y cuándo.</li> 
    <li>Revise el número total de personas y personas comercializables en su <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=es" target="_blank">base de datos de Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Lista de bloqueos</td>
    <td><li>Defina los criterios de lista de bloqueados. Considere la posibilidad de agregar los dominios de la competencia a su <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=es" target="_blank">lista de bloqueados</a> para evitar que reciban cualquiera de sus correos electrónicos.</li></td>
  </tr>
  <tr>
    <td>Marketing suspendido</td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">criterios de marketing suspendido</a>.</li></td>
  </tr>
  <tr>
    <td>Direcciones de email rechazadas </td>
    <td><li>Defina los criterios para las direcciones de correo electrónico devueltas.</li>
    <li>Revise las personas en la categoría "Correo electrónico no válido" y determine si sus correos electrónicos deben <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=es" target="_blank">restablecerse manualmente</a>.</li></td>
  </tr>
  <tr>
    <td>Duplicados posibles</td>
    <td><li>Revise las personas en la lista de posibles duplicados.</li> 
    <li>Defina su estrategia de administración de duplicados para determinar si desea <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=es" target="_blank">combinar personas manualmente</a>.</li>  
    <li>Si tiene una integración de CRM, defina un proceso y una cuenta para <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">el efecto de combinar posibles clientes en su CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Sin programa de adquisición</td>
    <td><li>Establezca campañas en las plantillas de programa que establecen un programa de adquisición, especialmente si utiliza formularios globales.</li></td>
  </tr>
  <tr>
    <td>Personas que cancelaron su suscripción</td>
    <td><li>Revisa tus criterios para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=es" target="_blank">Personas que cancelaron la suscripción</a>.</li></td>
  </tr>
</tbody>
</table>

## Listas inteligentes de grupos {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listas inteligentes de grupos</td>
    <td><li>Tenga en cuenta la creación de Listas inteligentes de grupo para que no haya listas duplicadas.</li>
    <li>Realizar un seguimiento de las listas maestras de la base de datos.</li></td>
  </tr>
</tbody>
</table>

## Segmentación {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">Área</th>
    <th style="width:79%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentación</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=es" target="_blank">Cree segmentaciones</a> basadas en sus necesidades comerciales. Cada suscripción está limitada a 20 segmentaciones y 100 segmentos dentro de cada segmentación.</li></td>
  </tr>
</tbody>
</table>
