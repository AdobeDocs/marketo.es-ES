---
description: Glosario de actividades de ventas - Documentos de Marketo - Documentación del producto
title: Glosario de actividades de ventas
source-git-commit: 9f8d6895e88250afc2799b2fb7fc73442018362f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 8%

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
   <td><strong>Detalles</strong></td> 
   <td>Detalles del mensaje de error de rechazo.</td> 
  </tr> 
  <tr> 
   <td><strong>Correo electrónico</strong></td> 
   <td>Dirección de correo electrónico devuelta.</td> 
  </tr> 
  <tr> 
   <td><strong>Vínculo</strong></td> 
   <td>Dirección URL donde se hizo clic.</td> 
  </tr> 
  <tr> 
   <td><strong>Recibido por</strong></td> 
   <td>Dirección de correo electrónico de la persona que envió el correo electrónico.</td> 
  </tr>
  <tr> 
   <td><strong>Llamada De Ventas Contestada Por</strong></td> 
   <td>Nombre de la persona que respondió a la llamada.</td> 
  </tr>
  <tr> 
   <td><strong>Duración de la llamada de venta</strong></td> 
   <td>Duración de la llamada en segundos.</td> 
  </tr>
  <tr> 
   <td><strong>Llamada de ventas realizada por</strong></td> 
   <td>Dirección de correo electrónico del vendedor que realizó la llamada.</td> 
  </tr>
  <tr> 
   <td><strong>URL de registro de llamada de venta</strong></td> 
   <td>URL de registro de llamada.</td> 
  </tr>
  <tr> 
   <td><strong>Estado de la llamada de venta</strong></td> 
   <td>Guardará el estado de llamada final de la llamada que incluye: completado, sin respuesta, cancelado, fallido.</td> 
  </tr>
  <tr> 
   <td><strong>Asunto de la llamada de venta</strong></td> 
   <td>Resultado de la llamada seleccionado por un usuario de ventas en el marcador .</td> 
  </tr>
  <tr> 
   <td><strong>ID de campaña de ventas</strong></td> 
   <td>ID único para el recurso de la campaña de ventas en Conexión de ventas.</td> 
  </tr>
  <tr> 
   <td><strong>Nombre de campaña de ventas</strong></td> 
   <td>Nombre de la campaña de ventas.</td> 
  </tr>
  <tr> 
   <td><strong>Dirección URL de la campaña de ventas</strong></td> 
   <td>Dirección URL de conexión de ventas para la campaña de ventas.</td> 
  </tr>
  <tr> 
   <td><strong>Asunto del correo electrónico de ventas</strong></td> 
   <td>Línea de correo electrónico del asunto.</td> 
  </tr>
  <tr> 
   <td><strong>Número de teléfono de ventas llamado</strong></td> 
   <td>Número de teléfono llamado por Ventas.</td> 
  </tr>
  <tr> 
   <td><strong>Nombre de plantilla de ventas</strong></td> 
   <td>Nombre de la plantilla de correo electrónico en Conexión de ventas.</td> 
  </tr>
  <tr> 
   <td><strong>URL de plantilla de ventas</strong></td> 
   <td>Dirección URL de conexión de ventas para la plantilla de correo electrónico.</td> 
  </tr>
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
 </tbody> 
</table>