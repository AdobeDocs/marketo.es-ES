---
description: 'Migración de AWS: Documentos de Marketo Engage: documentación del producto'
title: Migración de AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 94b7cd136325e2c6cb63b8bbf9ae2ee0aeb028b7
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 2%

---

# Migración de AWS {#aws-migration}

En los próximos meses, todas las suscripciones de Marketo Engage se migrarán de un centro de datos privado a la nube pública de AWS para mejorar la fiabilidad, la escalabilidad y la velocidad.

Recibirá un correo electrónico y una notificación en la aplicación aproximadamente 30 días antes de la migración. Utilice esta guía para prepararse.

## Acciones recomendadas {#actions}

Durante la ventana de migración, todos los servicios de Marketo Engage no estarán disponibles. Recomendamos realizar los siguientes pasos para mitigar cualquier impacto en su negocio.

* **Evite crear o actualizar posibles clientes o personas** o ejecutar procesos que modifiquen los registros de personas.

* **No almacene en déclencheur los procesos de seguimiento**, ya que las campañas programadas se pausarán.

* **Deshabilite temporalmente cualquier integración** que envíe o reciba datos desde o hacia Marketo Engage.

* **Evite ejecutar** importaciones o exportaciones de datos o cualquier campaña importante de generación de posibles clientes o personas.

* **Revise y actualice las listas de permitidos IP** para el inicio de sesión, el acceso a la API, el envío de correo electrónico, el seguimiento web y las integraciones.

* **Agregue nuevas direcciones IP** y mantenga sus direcciones IP actuales tal cual. Consulte las direcciones IP que desea agregar en la [tabla siguiente](#ip-addresses).

## Impactos previstos en el servicio {#impacts}

Los impactos siguientes no requieren ninguna acción por su parte.

* **Las integraciones de CRM y los servicios de LaunchPoint** se deshabilitarán, pero se reanudarán automáticamente más tarde.
* **Las páginas de aterrizaje, los formularios y la recopilación de datos** no estarán disponibles, y en su lugar se mostrará un mensaje de mantenimiento.

## Identificación del centro/pod de datos {#identify}

Antes de revisar las tablas siguientes, [aprenda a identificar](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) en qué centro de datos y pod/servidor se encuentra su suscripción.

## Programar {#schedule}

Periódicamente se añaden nuevas fechas e información del centro de datos/pod, así que asegúrese de volver aquí para obtener más detalles.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Fecha</th>
   <th style="width:20%">Centro de datos/Pod</th>
   <th style="width:30%">Hora</th>
  </tr>
  <tr>
   <td>8 de julio de 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>9 de julio de 2026</td>
   <td>AB70<br>
   AB43</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>11 de julio de 2026</td>
   <td>AB46</td>
   <td>10:00 PDT</td>
  </tr>
  <tr>
   <td>13 de julio de 2026</td>
   <td>NLD101</td>
   <td>10:00 PDT</td>
  </tr>
  <tr>
   <td>15 de julio de 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
  </tr>
  <tr>
   <td>17 de julio de 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
  </tr>
  <tr>
   <td>21 de julio de 2026</td>
   <td>AB54<br>
   AB56</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>23 de julio de 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
  </tr>
  <tr>
   <td>12 de agosto de 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
  </tr>
  <td>13 de agosto de 2026</td>
   <td>AB62<br>
   AB68</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
  </tr>
  </body>
</table>

## Direcciones IP que agregar {#ip-addresses}

En función de su centro de datos, colabore con su departamento de TI para añadir las direcciones IP correspondientes.

<table>
<tbody>
<tr>
  <th style="width:25%">Centro de datos</th>
  <th style="width:75%">Direcciones IP</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
</body>
</table>

## Actualizaciones y asistencia {#support}

Para obtener las últimas actualizaciones, marque esta página como favorito. Si tiene alguna pregunta, póngase en contacto con el Soporte técnico de Adobe a través del portal de soporte técnico en Admin Console o [Experience League](https://experienceleague.adobe.com/es/support){target="_blank"}.
