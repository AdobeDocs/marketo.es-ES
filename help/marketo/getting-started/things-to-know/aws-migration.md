---
description: 'Migración de AWS: Documentos de Marketo Engage: documentación del producto'
title: Migración de AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 5a260c00311588c3a55f176e7a7977f422bcc8a4
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# Migración de AWS {#aws-migration}

En los próximos meses, todas las suscripciones de Marketo Engage se migrarán de un centro de datos privado a la nube pública de AWS para mejorar la fiabilidad, la escalabilidad y la velocidad.

Recibirá un correo electrónico y una notificación en la aplicación aproximadamente 30 días antes de la migración. Utilice esta guía para prepararse.

## Acciones recomendadas

Durante la ventana de migración, todos los servicios de Marketo Engage no estarán disponibles. Recomendamos realizar los siguientes pasos para mitigar cualquier impacto en su negocio.

* **Evite crear o actualizar posibles clientes o personas** o ejecutar procesos que modifiquen los registros de personas.

* **No almacene en déclencheur los procesos de seguimiento**, ya que las campañas programadas se pausarán.

* **Deshabilite temporalmente cualquier integración** que envíe o reciba datos desde o hacia Marketo Engage.

* **Evite ejecutar** importaciones o exportaciones de datos o cualquier campaña importante de generación de posibles clientes o personas.

* **Revise y actualice las listas de permitidos IP** para el inicio de sesión, el acceso a la API, el envío de correo electrónico, el seguimiento web y las integraciones.

* **Agregue las siguientes direcciones IP** y mantenga sus direcciones IP actuales tal cual:

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Impactos previstos en el servicio

Los impactos siguientes no requieren ninguna acción por su parte.

* **Las integraciones de CRM y los servicios de LaunchPoint** se deshabilitarán, pero se reanudarán automáticamente más tarde.
* **Las páginas de aterrizaje, los formularios y la recopilación de datos** no estarán disponibles, y en su lugar se mostrará un mensaje de mantenimiento.

## Programación {#schedule}

Periódicamente se añaden nuevas fechas e información de centros de datos/pod, así que asegúrese de volver aquí para obtener más detalles.

Antes de revisar la tabla siguiente, [aprenda a identificar](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) en qué centro de datos y pod/servidor se encuentra su suscripción.

<table>
 <tbody>
  <tr>
   <th style="width:75%">Fecha</th>
   <th style="width:25%">Pod</th>
  </tr>
  <tr>
   <td>5 de junio de 2026</td>
   <td>AB46</td>
  </tr>
  <tr>
   <td>8 de julio de 2026</td>
   <td>AB69<br>
   AB64</td>
  </tr>
  <tr>
   <td>9 de julio de 2026</td>
   <td>AB70<br>
   AB43</td>
  </tr>
  &lt;/body>
  </table>

## Actualizaciones y asistencia

Para obtener las últimas actualizaciones, marque esta página como favorito. Si tiene alguna pregunta, póngase en contacto con el Soporte técnico de Adobe a través del portal de soporte técnico en Admin Console o [Experience League](https://experienceleague.adobe.com/es/support).
