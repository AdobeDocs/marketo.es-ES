---
description: 'Notas de la versión actuales, Documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8921f2e7608dd1ec1240d39cfeae845f79ae5db2
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 7%

---

# Notas de la versión: enero de 2024 {#release-notes-jan-24}

A continuación encontrará todas las funciones incluidas en la versión de enero de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes funciones entran dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **12 de enero de 2024**, con un despliegue gradual de las funciones restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Seminarios web a petición para seminarios web interactivos</strong>: los seminarios web bajo demanda le permiten publicar la grabación del seminario web, así como rastrear sus visitas/relojes. Esto le ayudará a obtener más posibles clientes a través de los inscritos que no asistieron al seminario web (no se presentaron), pero que siguen interesados en conocer más detalles y ver la grabación.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">Seminarios web bajo demanda</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
  </tr>
    <tr> 
   <td><strong>Páginas de aterrizaje de conversación</strong>: incruste un flujo de conversación de Dynamic Chat directamente en una página de aterrizaje de Marketo Engage para que los visitantes puedan programar una reunión a través de Dynamic Chat sin tener que rellenar un formulario ni interactuar con un bot de chat.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   </tr>
    <tr> 
   <td><strong>Filtrado de actividad de bots de correo electrónico</strong>: mejora la captura de la actividad de bots para la participación por correo electrónico, lo que le permite elegir lo agresivo que desea que sea el filtrado de identificación de la actividad de bots.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtrado de actividad de bots de correo electrónico</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   </tr>
    <tr> 
   <td><strong>Actualización API de importación masiva de posibles clientes</strong>: Se ha realizado un ajuste menor en el comportamiento de la API de importación masiva de posibles clientes al <b>id</b> se especifica como <b>lookupField</b> durante la creación del trabajo. Si un registro de persona está vinculado al proporcionado <b>id</b> no se encuentra en la base de datos de Marketo Engage, no se producirá ninguna actualización de registro, ya que no se puede encontrar el registro. El comportamiento actualizado ahora incluye el aumento del recuento en <b>numOfRowsFailed</b> dentro de la respuesta, lo que indica que la operación ha fallado en estos casos.</td> 
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
 </tbody> 
</table>
<br/>

## Funciones de versión de Agile {#agile-release-features}

Todas las funciones a continuación siguen un formato Agile y se lanzan en varias fechas antes o después de la fecha de lanzamiento estándar. Compruebe el estado junto a cada función.

### Acciones de perspectiva de ventas {#sales-insight-actions}

![(estrella)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:15%">Estado</th>
   <th style="width:20%">Documentación</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Ventana de composición ampliable</strong>: la ventana de redacción de correo electrónico ahora comprime automáticamente el espacio no utilizado, lo que permite más espacio en el editor. Además, la ventana podrá salir y ampliarse aún más, lo que proporcionará a los usuarios todo el espacio que necesiten para editar sus correos electrónicos.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:15%">Estado</th>
   <th style="width:20%">Documentación</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Interfaz de usuario del bot de chat para Conversational Forms</strong>: Los visitantes del sitio web ahora pueden solicitar chat en vivo en un flujo de conversación.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Opciones de color de fuente de Chatbot</strong>: personalice los colores de las fuentes en una configuración de bot de chat.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Opción para repetir el cuadro de diálogo</strong>: Ahora puede reiniciar el cuadro de diálogo al principio después de que un visitante haya llegado al final.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Finalización manual del chat en vivo</strong>: Tanto los visitantes como los agentes ahora pueden finalizar manualmente una sesión de chat en vivo.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Bandeja de entrada del agente</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Actividades recientes del Marketo Engage en la bandeja de entrada del agente</strong>: las actividades recientes del Marketo Engage, como Correo electrónico abierto y Formulario rellenado, se mostrarán para los posibles clientes en la bandeja de entrada del agente.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Bifurcación condicional</strong>: ahora puede mostrar a los visitantes contenido de conversación diferente en función de condiciones predefinidas, como la ubicación del visitante o la disponibilidad del agente en directo.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Sincronizar actualización de API de posibles clientes**: La [API de posible cliente de sincronización](https://developers.marketo.com/rest-api/lead-database/leads/#create_and_update){target="_blank"}El comportamiento de se ha ajustado ligeramente en relación con las actualizaciones de `unsubscribed` field. Ahora, cuando pases `null` como valor, es igual a pasar un valor de `false`.

* **Marketo Engage Forms jQuery 1.x**: En nuestra versión de enero de 2024, actualizaremos jQuery para Marketo Engage Forms a jQuery 3.x. Esto puede afectar a la implementación de formularios personalizados que depende de versiones anteriores de jQuery. [Obtenga más información aquí](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **Verificación por correo electrónico para usuarios solo de SSO**: Solo los usuarios de SSO solían verificarse automáticamente, lo que les permitía utilizar una cuenta de correo electrónico inaccesible. A partir de mediados de enero, todos los usuarios de solo SSO existentes pasarán a estar sin verificar y se les pedirá que vuelvan a verificar su correo electrónico mediante un vínculo que enviemos a la cuenta de correo electrónico. Todos los usuarios nuevos de solo SSO deberán verificar sus direcciones de correo electrónico a partir de ahora.

* Vea la [Seminario web sobre la versión de Marketo Engage de enero de 2024](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}
