---
description: Lista de comprobación de base de datos de instancias heredadas - Documentos de Marketo - Documentación del producto
title: Lista de comprobación de base de datos de instancias heredadas
hide: true
hidefromtoc: true
source-git-commit: 8660e8a7afa239c51cfed9e6e90e35aeedf6884f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 7%

---

# Instancia heredada: Lista de comprobación de base de datos {#inherited-instance-database-checklist}

Comprenda la cantidad total de personas, las personas comercializables y las fuentes principales de adquisición de personas en su suscripción.

## Listas inteligentes del sistema {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Todas las personas</td> 
   <td><li>¿Cuántas personas existen en la <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">database</a>?</li>
<li>Si la base de datos está casi llena, ¿recomienda la directiva de su empresa que amplíe el tamaño de la base de datos o que limpie los datos históricos?</li>
<li>¿Su base de datos general es al menos un 85% comercializable? 
<br/>     Si el suyo está por debajo de este umbral, observe las otras listas inteligentes del sistema (Lista de bloqueados, Marketing suspendido, Duplicados, Cancelación de suscripción) con mayor escrutinio.</li></td>
  </tr>
  <tr> 
   <td>Personas que cancelaron su suscripción</td> 
   <td><li>¿Cuáles son sus criterios de? <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">personas sin suscribir</a>? ¿Hay demasiadas personas sin suscribirse?</li>
<li>¿Sus métodos de cancelación de suscripción se ajustan a los requisitos de privacidad de datos?</li>
<li>¿Está actualizada su preferencia de cancelación de suscripción? ¿Cuánto tiempo han permanecido los registros en su base de datos como no comercializables?</li></td>
  </tr>
  <tr> 
   <td>Marketing suspendido</td> 
   <td><li>¿Cuáles son sus criterios de? <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing suspendido</a>? ¿Hay demasiadas personas que están suspendidas de marketing?</li>
<li>¿Durante cuánto tiempo han permanecido los registros en el estado Suspendido de marketing?</li>
<p>Ejemplo de caso de uso suspendido de marketing: registros de personas que participan activamente en las ventas en las últimas fases para las que desea suprimir las comunicaciones de marketing.</td>
  </tr>
   <tr> 
   <td>Lista de bloqueados</td> 
   <td><li>¿Cuáles son sus criterios de? <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">registros de inclusión en la lista de bloqueados</a>? ¿Hay demasiada gente incluida en la lista de bloqueados?</li></td>
  </tr>
  <tr> 
   <td>Direcciones de emails rechazadas</td> 
   <td><li>¿Tienes un montón de <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">personas que rebotaron</a> en la base de datos?
   <br/>     En caso afirmativo, considere la posibilidad de investigar el motivo.</li></td></li></td>
  </tr>
  <tr> 
   <td>Duplicados posibles</td> 
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">registros potencialmente duplicados</a> ¿hay?
   <br/>     Considere la posibilidad de eliminarlos o combinarlos.</li></td>
  </tr>
   <tr> 
   <td>Sin programa de adquisición</td> 
   <td><li>¿Cuántas personas no tienen un <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programa de adquisición</a>?
   <br/>     Si hay mucho, considere investigar el por qué.</li></td>
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
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Listas inteligentes</a> ¿hay? ¿Cómo se utilizan en esta instancia?</li>
<li>¿Las listas están organizadas en una estructura de carpetas coherente? 
<br/>     Si tiene listas de huérfanos, considere la posibilidad de organizar el árbol para que los recursos sean fáciles de encontrar.</li>
<p><img src="assets/tip-icon.png" alt="icono de sugerencia">SUGERENCIA: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivando</a> Las listas inteligentes que ya no son necesarias ayudarán a la organización y al rendimiento.</td>
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
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Listas estáticas</a> ¿hay? ¿Cómo se utilizan en esta instancia?</li></td>
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
   <td><li>Que <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentaciones</a> ¿hay? ¿Cómo se utilizan?</li>
<li>Hay demasiada gente en <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segmentos predeterminados</a>?</li>
<li>¿Hay una segmentación para la audiencia comercializable? 
<br/>     Si no es así, considere la posibilidad de crear uno.</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[◄ una instancia heredada: Administración](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-1.md)

[Auditoría de una instancia heredada: ► de actividades de marketing](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-3.md)
