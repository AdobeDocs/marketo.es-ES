---
description: Configurar la sección Base de datos para una nueva instancia de Marketo Engage.
title: NUEVA BASE DE DATOS DE ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 3cb7e5ddef8ec05a7cf8d65dd9f3bafa5dcb7da1
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 13%

---

# NUEVA ÁREA: Lista de comprobación de base de datos {#new-area-database-checklist}

Obtenga información sobre cómo implementar los pasos necesarios para la sección Base de datos en la nueva instancia de Marketo Engage. Siga las guías de &quot;Implementación de una nueva instancia&quot; y realice un seguimiento de las tareas en curso para configurar la instancia y lograr una eficacia a largo plazo.

## Listas inteligentes del sistema {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Todas las personas</td>
    <td><li>Determine la implementación de una sincronización 1:1 con CRM o la aplicación de filtros para limitar quién se mueve de un sistema a otro y cuándo.</li> 
    <li>Revise la cantidad total de personas y personas comercializables en su <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank" rel="noopener noreferrer">database</a>.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Lista de bloqueados</td>
    <td><li>Defina los criterios de lista de bloqueados. Considere la posibilidad de agregar los dominios de la competencia a <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank" rel="noopener noreferrer">lista de bloqueados</a> para evitar que reciban correos electrónicos operativos y de marketing.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Marketing suspendido</td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank" rel="noopener noreferrer">Marketing suspendido</a> criterios.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Direcciones de emails rechazadas </td>
    <td><li>Defina los criterios para Direcciones de correo electrónico rechazadas.</li>
    <li>Revisar las personas en la categoría Correo electrónico no válido y si es necesario enviar sus correos electrónicos <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank" rel="noopener noreferrer">restablecer manualmente</a>.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Duplicados posibles</td>
    <td><li>Revise las personas en la lista de posibles duplicados.</li> 
    <li>Defina la estrategia de administración de duplicados para determinar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank" rel="noopener noreferrer">combinación manual de personas</a> o no.</li>  
    <li>Si tiene una integración de CRM, debe definir un proceso y una cuenta para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank" rel="noopener noreferrer">el efecto de combinar posibles clientes en CRM</a>.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Sin programa de adquisición</td>
    <td><li>Establezca campañas en las plantillas de programa que establecen el programa de adquisición, especialmente si utiliza formularios globales.</li></td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Personas que cancelaron su suscripción</td>
    <td><li>Revise los criterios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank" rel="noopener noreferrer">Personas sin suscribir</a>.</li></td>
    <td>Texto</td>
  </tr>
</tbody>
</table>

## Listas inteligentes de grupos {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listas inteligentes de grupos</td>
    <td><li>Tenga en cuenta la creación de Listas inteligentes de grupo para que no haya listas duplicadas.</li>
    <li>Realice un seguimiento de las listas maestras aquí en la base de datos.</li></td>
    <td>Texto</td>
  </tr>
</tbody>
</table>

## Segmentación {#segmentation}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentación</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank" rel="noopener noreferrer">Creación de segmentaciones</a> en función de sus necesidades empresariales. Cada suscripción está limitada a 20 segmentaciones y 100 segmentos dentro de cada segmentación.</li></td>
    <td>Texto</td>
  </tr>
</tbody>
</table>
