---
unique-page-id: 1146999
description: 'Tokens para momentos interesantes: Marketo Docs: documentación del producto'
title: Tokens para momentos interesantes
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Tokens para momentos interesantes {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Aprenda a utilizar el paso [Flujo de momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Tokens disponibles {#available-tokens}

Consulte [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para ver todos los tokens que puede poner en un momento interesante.

## Activador de tokens {#trigger-tokens}

Según el activador utilizado en una campaña inteligente, hay disponibles tokens de activador adicionales.

* `{{trigger.Trigger Name}}` que siempre es el activador real. Por ejemplo: Clics en vínculo en el correo electrónico.
* `{{trigger.Name}}` es el nombre del recurso que activó la campaña. Por ejemplo: Clicks Link on Webpage es la propia URL, el asunto de los activadores de Salesforce, etc.
* Hay activadores adicionales disponibles en función de las restricciones que se enumeran a continuación.

**Activadores de correo electrónico**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Vínculo de clics en correo electrónico</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Devoluciones de correo electrónico duras</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Entregas de correo electrónico en blanco</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>El Correo Electrónico Se Entrega</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Abre el correo electrónico</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Correo electrónico de reenvío a amigo recibido</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Enviar correo electrónico de reenvío a amigo</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td>
  </tr> 
  <tr> 
   <td>Cancelación de suscripción desde correo electrónico</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Activadores de Salesforce**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Vínculo de clics en el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Se envía el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Abre el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Devoluciones de correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Se ha actualizado la oportunidad</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Cambios del propietario</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Persona convertida</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>La persona se elimina del SFDC</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Persona sincronizada con SFDC</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Eliminada de oportunidad</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Eliminado de la campaña SFDC</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>La actividad está registrada</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Actividad actualizada</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Se ha agregado a Oportunidad</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Se agregó a la campaña SFDC</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>El estado se cambia en la campaña SFDC</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Activadores de conexión de ventas**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Vínculo de clics en el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Se envía el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Abre el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Devoluciones de correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Se añade a la campaña de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>Cambios del propietario</td> 
   <td>Se Elimina De La Campaña De Ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Llamada de ventas recibida</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Varios**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Rellena el formulario</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Página web de visitas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Vínculo de clics en la página web</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Si no tiene una comprobación ![(visto)](assets/check.svg) entonces devolverá una cadena vacía (nada) en el momento interesante.

*El activador **Visitas a la página web** tiene algunos tokens adicionales:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Pruebe siempre sus momentos interesantes para asegurarse de que representan el modo que desea.
>
>Además, asegúrese de que es interesante para el vendedor, no solo para usted. ![(guiño)](assets/wink.svg)>
