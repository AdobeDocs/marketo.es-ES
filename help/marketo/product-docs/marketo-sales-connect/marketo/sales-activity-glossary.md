---
description: Glosario de actividades de ventas - Documentos de Marketo - Documentación del producto
title: Glosario de actividades de ventas
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 13%

---

# Glosario de actividades de ventas {#sales-activity-glossary}

En Sales Connect, cuando un vendedor: añade un posible cliente a una cadencia de ventas, le envía un correo electrónico o realiza una llamada a una actividad; se registra en el historial de actividades de Marketo. Además, cuando el posible cliente interactúa con correos electrónicos, también se registran las aperturas, los clics y las respuestas.

Las actividades siguientes se registrarán en Marketo desde Sales Connect.

>[!NOTE]
>
>Estas actividades y atributos están disponibles para su consumo desde nuestra API de REST y Bulk.

## Actividades {#activities}

<table>
 <tr>
  <th>Actividad de ventas</th>
  <th>Atributo</th>
 </tr>
 <tr>
  <th rowspan="3">Enviar email de ventas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <td>Identificación de la plantilla</td>
 </tr>
 <tr>
  <th rowspan="3">Abrir email de ventas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <td>Identificación de la plantilla</td>
 </tr>
 <tr>
  <th rowspan="4">Correo electrónico de ventas en el que se hizo clic</th>
  <td>Vínculo</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <td>Identificación de la plantilla</td>
 </tr>
 <tr>
  <th rowspan="2">Correo electrónico de ventas recibido</th>
  <td>Recibido por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <th rowspan="4">Se rechazó el email de ventas</th>
  <td>Detalles</td>
 </tr>
 <tr>
  <td>Identificación de la plantilla</td>
 </tr>
 <tr>
  <td>Email</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <th rowspan="7">Llamada de ventas recibida</th>
  <td>Llamada de ventas realizada por</td>
 </tr>
 <tr>
  <td>Estado de la llamada de venta</td>
 </tr>
 <tr>
  <td>Asunto de la llamada de venta</td>
 </tr>
 <tr>
  <td>Nombre de campaña de ventas</td>
 </tr>
 <tr>
  <td>Dirección URL de la campaña de ventas</td>
 </tr>
 <tr>
  <td>Número de teléfono de ventas llamado</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <th rowspan="6">Agregar a la campaña de ventas</th>
  <td>Nombre de campaña de ventas</td>
 </tr>
 <tr>
  <td>Estado de la llamada de venta</td>
 </tr>
 <tr>
  <td>Dirección URL de la campaña de ventas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <td>ID de campaña de ventas</td>
 </tr>
 <tr>
  <th rowspan="6">Eliminar de la campaña de ventas</th>
  <td>Nombre de campaña de ventas</td>
 </tr>
 <tr>
  <td>Estado de la llamada de venta</td>
 </tr>
 <tr>
  <td>Dirección URL de la campaña de ventas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origen</td>
 </tr>
 <tr>
  <td>ID de campaña de ventas</td>
 </tr>
</table>

## Descripciones {#descriptions}

<table> 
 <tr>
  <th>Atributo</th>
  <th>Descripción</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>Enviado por</strong></td>
   <td>Dirección de correo electrónico de la persona que envió el correo electrónico.</td> 
  </tr> 
  <tr> 
   <td><strong>Origen</strong></td> 
   <td>Fuente de la actividad. Se establecerá como "Tout" para las actividades de Conexión de ventas.</td> 
  </tr> 
  <tr> 
   <td><strong>Identificación de la plantilla</strong></td> 
   <td>Cuando el origen sea Tout, el ID de plantilla será el ID de plantilla de Marketo Sales Connect. Utilice esto para dirigirse a una plantilla específica en lugar de a una línea de asunto, que podría existir en varias plantillas.
</td> 
  </tr> 
  <tr> 
   <td><strong>Recibido por</strong></td> 
   <td>Dirección de correo electrónico de la persona que envió el correo electrónico.</td> 
  </tr> 
  <tr> 
   <td><strong>Detalles</strong></td> 
   <td>Detalles del mensaje de error de rechazo.</td> 
  </tr> 
  <tr> 
   <td><strong>Correo electrónico</strong></td> 
   <td>Dirección de correo electrónico devuelta.</td> 
  </tr> 
 </tbody> 
</table>