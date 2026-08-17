---
description: 'Migración de AWS: Documentos de Marketo Engage: documentación del producto'
title: Migración de AWS
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: d5768261c9bb659ef96b73c46a9e078f953d8ed6
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 4%

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

>[!NOTE]
>
>Si usa [formularios externos](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} y desea evitar la pérdida de los datos de envío de formularios recopilados mientras Marketo Engage no está disponible durante la ventana de migración, póngase en contacto con el [Soporte técnico de Adobe](https://experienceleague.adobe.com/en/support){target="_blank"} **con al menos dos días hábiles** de antelación y proporcione el ID del formulario y el ID de Munchkin de su suscripción.

## Identificación del centro/pod de datos {#identify}

Antes de revisar las tablas siguientes, [aprenda a identificar](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) en qué centro de datos y pod/servidor se encuentra su suscripción.

## Programación {#schedule}

Las nuevas fechas y la información del centro de datos/pod se añaden o cambian periódicamente, por lo que debe supervisar esta programación para ver si hay actualizaciones.

+++Programación de julio
<table>
 <tbody>
  <tr>
   <th style="width:25%">Fecha</th>
   <th style="width:25%">Centro de datos/Pod</th>
   <th style="width:25%">Hora</th>
   <th style="width:25%">Estado</th>
  </tr>
  <tr>
   <td>8 de julio de 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Finalizaciones<br>
   Completado</td>
  </tr>
  <tr>
   <td>9 de julio de 2026</td>
   <td>AB70</td>
   <td>17:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
   <td>11 de julio de 2026</td>
   <td>AB46</td>
   <td>10:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
   <td>13 de julio de 2026</td>
   <td>NLD101</td>
   <td>10:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
   <td>15 de julio de 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
   <td>Finalizaciones<br>
   Completado</td>
  </tr>
  <tr>
   <td>17 de julio de 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
   <td>Finalizaciones<br>
   Completado</td>
  </tr>
  <tr>
   <td>21 de julio de 2026</td>
   <td>AB54</td>
   <td>17:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
   <td>23 de julio de 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
   <td>31 de julio de 2026</td>
   <td>AB43</td>
   <td>15:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">Fecha</th>
   <th style="width:25%">Centro de datos/Pod</th>
   <th style="width:25%">Hora</th>
   <th style="width:25%">Estado</th>
  </tr>
  <tr>
   <td>12 de agosto de 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Finalizaciones<br>
   Completado</td>
  </tr>
  <tr>
  <td>13 de agosto de 2026</td>
   <td>AB68</td>
   <td>16:00 PDT</td>
   <td>Finalizaciones</td>
  </tr>
  <tr>
  <td>18 de agosto de 2026</td>
   <td><i>AB39</i></td>
   <td><i>17:00 PDT</i></td>
   <td><i>Pospuesto (fecha por determinar)</i></td>
  </tr>
  <tr>
   <td>20 de agosto de 2026</td>
   <td>AB42<br>
   AB44</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
  </tr>
  <tr>
   <td>26 de agosto de 2026</td>
   <td>AB40<br>
   AB50</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
  </tr>
  <tr>
   <td>28 de agosto de 2026</td>
   <td>AB53<br>
   AB56</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
  </tr>
  <tr>
   <td>8 de septiembre de 2026</td>
   <td>AB01<br>
   AB02</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
  </tr>
  <tr>
   <td>10 de septiembre de 2026</td>
   <td>AB03<br>
   <i>AB04</i></td>
   <td>17:00 PDT<br>
   <i>6 p. m. PDT</i></td>
   <td>Según lo programado<br>
   <i>Pospuesto (fecha por determinar)</i></td>
  </tr>
  <tr>
   <td>15 de septiembre de 2026</td>
   <td>AB05<br>
   AB06</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
  </tr>
  <tr>
   <td>17 de septiembre de 2026</td>
   <td>AB07<br>
   AB08</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Según lo programado<br>
   Dentro del horario</td>
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

Para obtener las últimas actualizaciones, marque esta página como favorito. Si tiene alguna pregunta, póngase en contacto con el Soporte técnico de Adobe a través del portal de soporte técnico en Admin Console o [Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}.

## Preguntas frecuentes {#faq}

**¿Dónde se almacenan los datos?**
Todos los datos de usuario de Marketo se almacenan en Amazon Web Service (AWS). Marketo ha migrado su infraestructura de centros de datos físicos propios a la plataforma en la nube de nivel empresarial de AWS.

**¿Dónde se almacenan específicamente los datos personales?**
Los datos personales se almacenan en Amazon Aurora, el servicio de base de datos relacional totalmente gestionado de AWS. Aurora replica los datos de seis maneras en tres zonas de disponibilidad separadas dentro de la región de AWS para proteger los datos personales contra fallos de hardware, degradación del almacenamiento y eventos de infraestructura localizados.

**¿A quién pertenece el entorno de almacenamiento?**
La infraestructura de almacenamiento es propiedad de Amazon Web Service (AWS) y la gestiona. Adobe (Marketo) funciona como cliente de AWS bajo un modelo de responsabilidad compartida: AWS es responsable de la seguridad y disponibilidad de la infraestructura subyacente, mientras que Adobe es responsable de la seguridad de los datos y las aplicaciones que se ejecutan dentro de ella.

**¿Cuáles son los detalles completos sobre la producción, las ubicaciones de backup/recuperación ante desastres y la tecnología de almacenamiento?**
Marketo utiliza Amazon Aurora, un motor de base de datos relacional nativo de la nube totalmente administrado por AWS, como tecnología de base de datos principal. Aurora desvincula la computación y el almacenamiento, replicando automáticamente los datos de seis formas en tres zonas de disponibilidad dentro de la región de producción y requiriendo un quórum de cuatro copias para confirmar cualquier operación de escritura.

Aurora también realiza backups automáticos y continuos en Amazon S3 en tiempo real, lo que permite la recuperación en un momento dado (PITR) en cualquier segundo dentro de la ventana de retención configurada.

En este momento, la implementación Aurora de Marketo funciona dentro de una sola región de AWS, sin replicación entre regiones. Los datos de producción permanecen dentro de la infraestructura regional designada, y la recuperación ante desastres se proporciona a través de la redundancia del almacenamiento multi-AZ y los backups continuos de Aurora en lugar de la conmutación por error geográfica a una región secundaria. Esto puede evaluarse más a medida que la infraestructura de AWS de Marketo madure.
