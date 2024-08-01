---
description: 'Notas de la versión, marzo de 2024: Documentos de Marketo: documentación del producto'
title: Notas de la versión, marzo de 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 1839ccb646e775b67efa8de7d2d2bf3dbbbefa72
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# Notas de la versión: marzo de 2024 {#release-notes-mar-24}

A continuación encontrará todas las funciones incluidas en la versión de marzo de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **8 de marzo de 2024**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr> 
   <td><strong>Lógica de flujo de conversación avanzada</strong>: agregue campos adicionales para la evaluación en una sola opción para el seguimiento de flujo de conversación.</td> 
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
   <td><strong>Reordenar lógica de flujo de conversación</strong>: en Marketo Engage Forms, ahora puede reordenar las opciones de flujo de conversación, en lugar de tener que eliminarlas y agregarlas de nuevo.</td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configuración de flujo de conversación para Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Metadatos de actividad de API</strong>: 
   Ahora, los metadatos como agente de usuario, plataforma y dispositivo se incluyen en las actividades web y de correo electrónico, lo que ayuda a proporcionar una perspectiva coherente de estas actividades a través de la API de REST de Marketo.</td> 
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Obtener corrección de API de miembro del programa**: recientemente se realizó un cambio para corregir el comportamiento del extremo [Obtener miembros del programa](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Anteriormente, al utilizar el tipo de filtro `updatedAt` para especificar un intervalo de fechas, existía la posibilidad de que los registros de pertenencia a programas actualizados dentro de ese intervalo no se incluyeran en la respuesta. Además, existía la posibilidad de que los registros de pertenencia a programas actualizados fuera del intervalo de fechas especificado se incluyeran incorrectamente en la respuesta. Se han resuelto ambos problemas.

* **Desuso del complemento del explorador de perspectiva de cuenta**: El Adobe está eliminando el complemento del explorador de perspectiva de cuenta [Administrador de cuentas de Target](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} de la Tienda web de Chrome el 8 de abril de 2024. Usuarios existentes: puede seguir utilizando el complemento hasta que migre la instancia de Marketo Engage a Identidad de Adobe y Admin Console. Este cambio **no afectará** a ninguna otra función o dato de TAM dentro de Marketo Engage ni a los complementos de correo electrónico de Chrome y Outlook que funcionan con Sales Insight. [Más información](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
