---
unique-page-id: 2953243
description: Tipos de notificaciones - Documentos de Marketo - Documentación del producto
title: Tipos de notificación
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Tipos de notificación {#notification-types}

Existen varios tipos de notificaciones.

## Error de campaña {#campaign-failure}

Los errores de campaña le notifican de los errores de sus campañas inteligentes.

## Sincronización de CRM {#crm-sync}

Las notificaciones de sincronización de CRM le advierten de problemas críticos que se han encontrado con la sincronización de CRM, como permisos incorrectos o la sincronización que se está realizando.

**Microsoft Dynamics**

Las notificaciones de Dynamics se envían una vez cada 24 horas y contienen posibles clientes que no se pudieron sincronizar en ese período de tiempo. Los motivos típicos del error son posibles clientes duplicados (como se indica más arriba) o errores de coincidencia de longitud de campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Si utiliza Salesforce, las notificaciones de error de sincronización se parecen a la que se muestra a continuación. Los errores típicos incluyen credenciales caducadas y límites de API excedidos.

![](assets/salesforcesyncerror.png)

Participación

Cuando los posibles clientes se agotan en una secuencia, se envía una notificación.  La notificación incluye el número de posibles clientes que se agotaron y alguna otra información.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Si intenta enviar posibles clientes a Facebook sin aceptar los términos del servicio o si intenta enviar posibles clientes a Facebook después de eliminar la aplicación de Marketo.

Limpieza de campaña de Déclencheur inactivo

Desactivar activó las campañas inteligentes que ya no obtienen ninguna actividad. Obtenga más información sobre [limpieza automática de campañas de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

linkedIn

Cuando Marketo no puede crear una nueva audiencia, iniciar sesión o enviar correos electrónicos a LinkedIn después de tres intentos.

![](assets/linkedin.png)

Servicios Web

Recibirá una notificación cuando alcance su cuota diaria. La cuota se restablece cada noche a medianoche, hora central.

>[!NOTE]
>
>Algunos de los códigos de error que puede recibir se describen en nuestra [Documentación para desarrolladores](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
