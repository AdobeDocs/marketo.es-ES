---
unique-page-id: 1146999
description: Tokens para momentos interesantes - Documentos de marketing - Documentación del producto
title: Tokens para momentos interesantes
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Tokens para momentos interesantes {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Aprenda a utilizar el paso [Flujo de momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Tokens disponibles {#available-tokens}

Consulte [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para ver todos los tokens que puede poner en un momento interesante.

## Tokens de déclencheur {#trigger-tokens}

En función del déclencheur utilizado en una campaña inteligente, hay disponibles tokens de Déclencheur adicionales.

* `{{trigger.Trigger Name}}` que es siempre el déclencheur mismo. Por ejemplo: Vínculo de clics en correo electrónico.
* `{{trigger.Name}}` es el nombre del recurso que activó la campaña. Por ejemplo: Vínculo de clics en la página web es la propia dirección URL, sujeto de déclencheur de Salesforce, etc.
* Existen déclencheur adicionales en función de las restricciones, que se enumeran a continuación:

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
  </tr> 
  <tr> 
   <td>Devoluciones de correo electrónico con fuerza</td> 
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
  </tr> 
  <tr> 
   <td>Devoluciones de correo electrónico en pantalla</td> 
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
  </tr> 
  <tr> 
   <td>Se entrega el correo electrónico</td> 
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
  </tr> 
  <tr> 
   <td>Cancelación de suscripciones desde correo electrónico</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Vínculo de clics en correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas enviado</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Abre el correo electrónico de ventas</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(visto)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Correo electrónico de ventas facturado</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(visto)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(visto)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
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
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Página Web Visitas*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(visto)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(visto)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Si no tiene una marca de verificación ![(tic)](assets/check.svg), devolverá una cadena vacía (nada) en el momento interesante.

*El Déclencheur **Visitas a la página Web** tiene algunos tokens adicionales:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Pruebe siempre los momentos interesantes para asegurarse de que representan el modo que usted desea.
>
>Además, asegúrese de que es interesante para el vendedor, no sólo para usted. ![(wink)](assets/wink.svg)>
