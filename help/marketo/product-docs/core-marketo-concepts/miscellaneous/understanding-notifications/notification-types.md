---
unique-page-id: 2953243
description: 'Tipos de notificación: documentos de Marketo, documentación del producto'
title: Tipos de notificación
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 7%

---

# Tipos de notificación {#notification-types}

Existen varios tipos de notificación.

## Error en la campaña  {#campaign-failure}

Los errores de Campaign le notifican de los errores que se producen en sus campañas inteligentes.

## Sincronización de CRM {#crm-sync}

Las notificaciones de sincronización de CRM le avisan de problemas críticos que se encuentran con la sincronización de CRM, como permisos incorrectos o la sincronización no está activa.

**[!DNL Microsoft Dynamics]**

Las notificaciones de [!DNL Dynamics] se envían una vez cada 24 horas y contienen posibles clientes que no se sincronizaron durante ese período de tiempo. Los motivos habituales del error son los errores de coincidencia de longitud de campo o posibles clientes duplicados (como se ha indicado anteriormente).

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Si usa [!DNL Salesforce], las notificaciones de error de sincronización se parecerán a las que se muestran a continuación. Los errores habituales incluyen credenciales caducadas y límites de API excedidos.

![](assets/salesforcesyncerror.png)

## Participación {#engagement}

Cuando las personas se agotan en un flujo, enviamos una notificación. La notificación incluye el número de personas que se agotaron y alguna otra información.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Si intenta enviar personas a Facebook sin aceptar los Términos de servicio, o si intenta enviar personas a Facebook después de eliminar la aplicación de Marketo.

## Limpieza de campañas desencadenadoras sin actividad {#idle-trigger-campaign-cleanup}

Desactive las campañas inteligentes activadas que ya no obtengan ninguna actividad. Más información sobre [limpieza automática de campañas de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

Cuando Marketo no puede crear una nueva audiencia, inicia sesión o envía correos electrónicos a LinkedIn después de tres intentos.

![](assets/linkedin.png)

## Servicios web {#web-services}

Se le notificará cuando alcance su cuota diaria. La cuota se restablece cada noche a medianoche, hora central.

>[!NOTE]
>
>Algunos de los códigos de error que puede recibir se describen en [Documentación para desarrolladores](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/error-codes).
