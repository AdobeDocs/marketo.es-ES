---
description: 'Notas de la versión actuales, Documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cfbf9206bcb0e54abdbd962e52844bba11b07197
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 5%

---

# Notas de la versión: marzo de 2024 {#release-notes-mar-24}

A continuación encontrará todas las funciones incluidas en la versión de marzo de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes funciones entran dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **8 de marzo de 2024**, con un despliegue gradual de las funciones restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr> 
   <td><strong>Lógica avanzada de flujo de conversación</strong>: Añada campos adicionales para la evaluación en una sola opción para el seguimiento del flujo de conversación.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configuración de flujo de conversación para Marketo Engage Forms</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Reordenar lógica de flujo de conversación</strong>: en Marketo Engage Forms, ahora puede reordenar las opciones de Flujo de conversación, en lugar de tener que eliminarlas y agregarlas de nuevo.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configuración de flujo de conversación para Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Metadatos de actividad de API</strong>: los metadatos, como agente de usuario, plataforma y dispositivo, ahora se incluyen en las actividades web y de correo electrónico, lo que ayuda a proporcionar una perspectiva coherente de estas actividades a través de la API de REST de Marketo.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Obtener corrección de API de miembro del programa**: Se ha realizado un cambio recientemente para corregir el comportamiento de [Obtener miembros del programa](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} punto final. Anteriormente, al utilizar el `updatedAt` tipo de filtro para especificar un intervalo de fechas, existía la posibilidad de que los registros de pertenencia a programas actualizados dentro de ese intervalo no se incluyeran en la respuesta. Además, existía la posibilidad de que los registros de pertenencia a programas actualizados fuera del intervalo de fechas especificado se incluyeran incorrectamente en la respuesta. Se han resuelto ambos problemas.

* **Degradación del complemento del explorador de Account Insight**: el Adobe elimina la administración de cuentas de Target [Complemento del explorador de Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on March 18, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
