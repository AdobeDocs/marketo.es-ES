---
description: Lista de comprobación de base de datos de instancias heredadas - Documentos de Marketo - Documentación del producto
title: Lista de comprobación de base de datos de instancias heredadas
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
TQID: https://experienceleague.adobe.com/ssiWj0vQTwU1qBD5fyZ8VHz7RmFjaVxu1dj7J8G-P5U
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 423
ht-degree: 8%

---

# Instancia heredada: Lista de comprobación de la base de datos {#inherited-instance-database-checklist}

Comprenda la cantidad total de personas, las personas comercializables y las fuentes principales de adquisición de personas en su suscripción. Recuerde [descargar las listas de comprobación](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) y realizar un seguimiento de su progreso.

## Listas inteligentes del sistema {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr>
  <tr>
   <td>Todas las personas</td>
   <td><li>¿Cuántas personas existen en la <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">base de datos</a>?</li>
<li>Si la base de datos está casi llena, ¿recomienda la directiva de su empresa que amplíe el tamaño de la base de datos o que limpie los datos históricos?</li>
<li>¿Su base de datos general es al menos un 85% comercializable?
<br/> Si el suyo se encuentra por debajo de este umbral, observe las otras listas inteligentes del sistema (Lista de bloqueados, Marketing suspendido, Duplicados, Cancelar suscripción) con mayor escrutinio.</li></td>
  </tr>
  <tr>
   <td>Personas que cancelaron su suscripción</td>
   <td><li>¿Cuál es su criterio para <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">cancelar la suscripción</a>? ¿Hay demasiadas personas sin suscribirse?</li>
<li>¿Sus métodos de cancelación de suscripción se ajustan a los requisitos de privacidad de datos?</li>
<li>¿Está actualizada su preferencia de cancelación de suscripción? ¿Cuánto tiempo han permanecido los registros en su base de datos como no comercializables?</li></td>
  </tr>
  <tr>
   <td>Marketing suspendido</td>
   <td><li>¿Cuáles son sus criterios para <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing suspendido</a>? ¿Hay demasiadas personas que están suspendidas de marketing?</li>
<li>¿Durante cuánto tiempo han permanecido los registros en el estado Suspendido de marketing?</li>
<p>Ejemplo de caso de uso suspendido de marketing: registros de personas que participan activamente en las ventas en las últimas fases para las que desea suprimir las comunicaciones de marketing.</td>
  </tr>
   <tr>
   <td>Lista de bloqueados</td>
   <td><li>¿Cuáles son sus criterios para <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">registros de inclusión en la lista de bloqueados</a>? ¿Hay demasiada gente incluida en la lista de bloqueados?</li></td>
  </tr>
  <tr>
   <td>Direcciones de email rechazadas</td>
   <td><li>¿Tiene muchas <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">personas que rebotaron</a> en la base de datos?
   <br/> Si es así, considere la posibilidad de investigar el motivo.</li></td></li></td>
  </tr>
  <tr>
   <td>Duplicados posibles</td>
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">registros potencialmente duplicados</a> existen?
   <br/> Considere la posibilidad de eliminarlos o combinarlos.</li></td>
  </tr>
   <tr>
   <td>Sin programa de adquisición</td>
   <td><li>¿Cuántas personas no tienen un <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programa de adquisición</a>?
   <br/> Si hay muchas, considere la posibilidad de investigar el motivo.</li></td>
  </tr>
 </tbody>
</table>

## Listas inteligentes {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr>
  <tr>
   <td>Listas inteligentes</td>
   <td><li>¿Cuántas <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">listas inteligentes</a> hay? ¿Cómo se utilizan en esta instancia?</li>
   <p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: En la sección Base de Datos, las Listas Inteligentes de Grupo son listas generadas por el usuario y las Listas Inteligentes de Sistema son listas por defecto creadas por Marketo Engage.
<li>¿Las listas están organizadas en una estructura de carpetas coherente?
<br/> Si tiene listas de huérfanos, considere la posibilidad de organizar el árbol para que los recursos sean fáciles de encontrar.</li>
<p><img src="assets/tip-icon.png" alt="icono de sugerencia">SUGERENCIA: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivar</a> listas inteligentes que ya no se necesitan ayudará con la organización y el rendimiento.</td>
  </tr>
 </tbody>
</table>

## Listas estáticas {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr>
  <tr>
   <td>Listas estáticas</td>
   <td><li>¿Cuántas <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">listas estáticas</a> hay? ¿Cómo se utilizan en esta instancia?</li>
   <p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: En la sección Base de Datos, las Listas de Grupos son Listas Estáticas.</td>
  </tr>
 </tbody>
</table>

## Segmentación {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr>
  <tr>
   <td>Segmentación</td>
   <td><li>¿Qué <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentaciones</a> hay? ¿Cómo se utilizan?</li>
<li>¿Hay demasiadas personas en <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segmentos predeterminados</a>?</li>
<li>¿Hay una segmentación para la audiencia comercializable?
<br/> Si no es así, considere la posibilidad de crear uno.</li></td>
  </tr>
 </tbody>
</table>
