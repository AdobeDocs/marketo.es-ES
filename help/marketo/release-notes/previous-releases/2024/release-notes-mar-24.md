---
description: 'Notas de la versión, marzo de 2024: Documentos de Marketo: documentación del producto'
title: Notas de la versión, marzo de 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 30%

---

# Notas de la versión: marzo de 2024 {#release-notes-mar-24}

A continuación encontrará todas las funciones incluidas en la versión de marzo de 2024. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 08 de marzo de 2024**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Lógica de flujo de conversación avanzada</strong>: agregue campos adicionales para la evaluación en una sola opción para el seguimiento de flujo de conversación.</td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configuración del flujo conversacional para los formularios de Marketo Engage</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Reordenar lógica de flujo de conversación</strong>: en Marketo Engage Forms, ahora puede reordenar las opciones de flujo de conversación, en lugar de tener que eliminarlas y agregarlas de nuevo.</td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configuración del flujo conversacional para los formularios de Marketo Engage</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Metadatos de actividad de API</strong>:
   Ahora, los metadatos como agente de usuario, plataforma y dispositivo se incluyen en las actividades web y de correo electrónico, lo que ayuda a proporcionar una perspectiva coherente de estas actividades a través de la API de REST de Marketo.</td>
   <td>Publicado</td>
   <td>N/A</td>
  </tr>
 </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Obtener corrección de API de miembro del programa**: recientemente se realizó un cambio para corregir el comportamiento del extremo [Obtener miembros del programa](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Anteriormente, al utilizar el tipo de filtro `updatedAt` para especificar un intervalo de fechas, existía la posibilidad de que los registros de pertenencia a programas actualizados dentro de ese intervalo no se incluyeran en la respuesta. Además, existía la posibilidad de que los registros de pertenencia a programas actualizados fuera del intervalo de fechas especificado se incluyeran incorrectamente en la respuesta. Se han resuelto ambos problemas.

* **Desuso del complemento del explorador Insight de cuentas**: Adobe está eliminando el complemento del explorador Insight de cuentas [Administración de cuentas de Target](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} de la Tienda web de Chrome el 8 de abril de 2024. Usuarios existentes: puede seguir utilizando el complemento hasta que migre la instancia de Marketo Engage a Adobe Identity y Admin Console. Este cambio **no afectará** ninguna otra función o dato de TAM dentro de Marketo Engage o los complementos de correo electrónico de Chrome y Outlook que funcionan con Sales Insight. [Más información](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
