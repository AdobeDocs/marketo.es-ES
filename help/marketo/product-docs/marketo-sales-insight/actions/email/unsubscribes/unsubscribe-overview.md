---
description: Información general sobre la cancelación de la suscripción - Documentos de Marketo - Documentación del producto
title: Información general de cancelación de suscripción
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Información general de cancelación de suscripción {#unsubscribe-overview}

Cada vez es más importante que las organizaciones cumplan con las leyes de privacidad de correo electrónico. Para ayudarle con esto, hemos realizado algunas mejoras en nuestra experiencia de cancelación de suscripción.

* Los vínculos de cancelación de suscripción se colocan en todos los correos electrónicos enviados desde Marketo Sales and Salesforce (esto no se aplica a los correos electrónicos personalizados enviados desde Outlook o Gmail)
* Los administradores pueden editar los mensajes de cancelación de suscripción para todo su equipo
* La información de cancelación de suscripción se almacena en PDV
* Las cancelaciones de suscripción se pueden realizar manualmente: vínculos en los que se hizo clic, sincronización de Salesforce y devoluciones
* Nueva página de aterrizaje de vínculo de cancelación de suscripción

## Cancelar suscripción a página de aterrizaje de vínculo {#unsubscribe-link-landing-page}

Cuando una persona hace clic en el vínculo de cancelación de suscripción, se le redirige a una página de aterrizaje de cancelación de suscripción en la que puede seleccionar desde qué desea cancelar la suscripción y por qué.

![](assets/unsubscribe-overview-1.png)

Esta información se guardará en la vista de detalles de la persona para su visualización posterior.

## Cancelar suscripción al grupo {#unsubscribe-group}

Ver y administrar todas las personas que cancelaron su suscripción en un solo lugar.

![](assets/unsubscribe-overview-2.png)

Utilice la barra de búsqueda para buscar cualquier persona que no esté suscrita.

![](assets/unsubscribe-overview-3.png)

Si es administrador, puede ir al grupo Cancelar suscripción para filtrar por Cancelaciones de suscripción de cuenta y ver todas las cancelaciones de suscripción que se han recopilado en su base de datos de personas.

![](assets/unsubscribe-overview-4.png)

## Tarjeta Historial de cancelación {#unsubscribe-history-card}

La tarjeta Historial de cancelación de suscripción ayuda a los administradores y usuarios a obtener información contextual sobre el historial de cancelación de suscripción de sus contactos. Vaya a la pestaña Personas y seleccione una persona. Se encuentra en la parte inferior de la pestaña Acerca de, en la vista de detalles de la persona.

>[!NOTE]
>
>Solo habrá una tarjeta Historial de cancelación de suscripción si la persona tiene _resuscrito_ en algún momento.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Fecha</strong></td> 
   <td><p>Muestra la fecha en la que se canceló la suscripción o se volvió a suscribir.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Detalles</strong></td> 
   <td><p>Volver a suscribir: un administrador de Sales Connect ha eliminado manualmente la cancelación de la suscripción del registro de contactos. También puede mostrar algunos detalles relacionados con el motivo por el que se canceló la suscripción al contacto.</p><p>Cancelar suscripción: se canceló la suscripción del contacto.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Origen</strong></td> 
   <td><p>Sincronización de Salesforce: Una sincronización de Salesforce capturó la cancelación de la suscripción.</p><p>Manual: el usuario ha hecho clic en el botón Cancelar la suscripción para darse de baja.</p><p>Vínculo en el que se hizo clic: el destinatario de un correo electrónico hizo clic en el vínculo para cancelar la suscripción.</p><p>"Nombre del administrador": Se mostrará un nombre de administrador cuando la acción fue volver a suscribir contactos. Esto permite a los usuarios saber quién eliminó la cancelación de la suscripción.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Personalizar mensaje de vínculo de cancelación de suscripción](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
