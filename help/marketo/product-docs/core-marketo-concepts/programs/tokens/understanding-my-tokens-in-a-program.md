---
unique-page-id: 1147114
description: 'Explicación de mis tokens en un programa: Marketo Docs: documentación del producto'
title: Explicación de mis tokens en un programa
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 2%

---

# Explicación de mis tokens en un programa {#understanding-my-tokens-in-a-program}

Un token es una variable que puede usar en correos electrónicos, páginas de aterrizaje y campañas inteligentes para facilitar su vida.

Además de Mis tokens, también puede utilizar cualquiera de los tokens integrados en sus programas. Consulte la [Información general sobre tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## Mis tokens  {#my-tokens}

Mis tokens son variables personalizadas que cualquiera puede crear. Son [created](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) en carpetas de campañas o programas.

Mis tokens se muestran de esta manera: `{{my.Name Of Token}}`

Ejemplos:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Archivo de calendario <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Use este token para <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">agregar un archivo de eventos de calendario (.i)</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> a sus correos electrónicos y páginas de aterrizaje.</td> 
  </tr> 
  <tr> 
   <td><p>Fecha <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Este token contiene un valor de fecha. La fecha se muestra como año-mes-día (por ejemplo, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script de email <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilice este token para ejecutar un script de Velocity en los mensajes de correo electrónico. Más información <a href="https://developers.marketo.com/documentation/email-scripting/" title="Seguir vínculo" rel="nofollow">here</a>. </td> 
  </tr> 
  <tr> 
   <td>Número<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Cualquier entero. Incluso puede ser negativo.</td> 
  </tr> 
  <tr> 
   <td>Texto enriquecido <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Esto es HTML. Úselo en correos electrónicos y páginas de aterrizaje.</td> 
  </tr> 
  <tr> 
   <td>Puntuación <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilice este token en la variable <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">paso cambiar flujo de puntuación</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">Campaña SFDC <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Utilice este token para permitir que los posibles clientes que formen parte de un programa de Marketo también se agreguen a cualquier campaña de SFDC.</td> 
  </tr> 
  <tr> 
   <td>Texto <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Sólo texto. Utilícelo cuando el HTML sea demasiado agudo. El límite de tamaño para tokens de texto es de 524 288 caracteres (UTF-8) o 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Mis tokens no se resolverán al enviar un correo electrónico desde Sales Insight en Microsoft Dynamics o Salesforce; solo se rellenarán los tokens estándar (posible cliente, empresa, etc.). Valores predeterminados para tokens _will_ sin embargo, trabajan.

## Anidado de tokens {#nesting-tokens}

Cuando se crea un nuevo token, otros objetos del árbol pueden hacer referencia a él. Hay una estructura de nombres para la que el token se creó para facilitar la administración.

* **Token local:** El token se creó directamente en ese programa o carpeta.
* **Token heredado:** El token se creó en el árbol en algún lugar de un programa o carpeta de nivel superior.
* **Token ignorado:** El token se heredó y luego alguien hizo una excepción en este programa o carpeta.

Puede crear variables globales y luego anularlas en niveles inferiores del árbol.

Mover programas y carpetas también afecta a los tokens. Compruebe siempre que las referencias no estén rotas durante el movimiento.

>[!NOTE]
>
>Si el correo electrónico que envía desde un programa de participación es un correo electrónico secundario de un programa predeterminado (no local para el programa de participación), cualquier My Tokens utilizado en el correo electrónico se resuelve desde el programa predeterminado en el que reside el correo electrónico secundario.

>[!MORELIKETHIS]
>
>* [Información general sobre tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Administración de tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

