---
unique-page-id: 2953243
description: Tipos de notificaciones - Documentos de marketing - Documentación del producto
title: Tipos de notificaciones
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Tipos de notificaciones {#notification-types}

Existen varios tipos de notificaciones.

## Error de campaña  {#campaign-failure}

Los errores de campaña le notifican los errores de sus campañas inteligentes.

## Sincronización de CRM {#crm-sync}

Las notificaciones de sincronización de CRM le avisan de los problemas críticos que se han encontrado con la sincronización de CRM, como los permisos incorrectos o la falta de sincronización.

**Microsoft Dynamics**

Las notificaciones de Dynamics se envían una vez cada 24 horas y contienen leads que no se sincronizaron en ese período de tiempo. Los motivos típicos de error son posibles duplicados (como arriba) o errores de discordancia de longitud de campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Si usa Salesforce, las notificaciones de error de sincronización se parecen a la de abajo. Los errores típicos incluyen credenciales caducadas y límites de API excedidos.

![](assets/salesforcesyncerror.png)

Participación

Cuando los leads se agotan en un flujo, enviamos una notificación.  La notificación incluye el número de posibles clientes que se agotaron y otra información.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Si intenta enviar leads a Facebook sin aceptar los términos del servicio, o si intenta enviar leads a Facebook después de quitar la aplicación de marketing.

Limpieza de Campaña del activador inactivo

Desactivar Campañas inteligentes activadas que ya no reciben ninguna actividad. Obtenga más información sobre la limpieza [](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)automática de campañas desencadenadoras.

LinkedIn

Cuando Marketing no puede crear una nueva audiencia, iniciar sesión o insertar correos electrónicos en LinkedIn después de tres intentos.

![](assets/linkedin.png)

Servicios Web

Recibirá una notificación cuando alcance su cuota diaria. La cuota se restablece cada noche a medianoche, hora central.

>[!NOTE]
>
>Algunos de los códigos de error que puede recibir se describen en nuestra Documentación [](http://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)para desarrolladores.

