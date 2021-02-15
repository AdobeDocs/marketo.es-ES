---
unique-page-id: 1147114
description: Explicación de mis tokens en un Programa - Documentos de marketing - Documentación del producto
title: Explicación de mis tokens en un Programa
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Explicación de mis tokens en un Programa {#understanding-my-tokens-in-a-program}

Un token es una variable que puede utilizar en correos electrónicos, páginas de aterrizaje y campañas inteligentes para facilitar su vida.

Además de Mis tokens, también puede usar cualquiera de los tokens integrados en sus programas. Consulte la [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## Mis tokens {#my-tokens}

Mis tokens son variables personalizadas que cualquiera puede crear. Se [crean](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) en carpetas de campaña o programas.

Mis tokens se muestran así: `{{my.Name Of Token}}`

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
   <td>Utilice este token para <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">agregar un archivo de evento de calendario (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> a sus correos electrónicos y páginas de aterrizaje.</td> 
  </tr> 
  <tr> 
   <td><p>Fecha <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Este token contiene un valor de fecha. La fecha se muestra como año-mes-día (por ejemplo, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Secuencia de comandos de correo electrónico <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilice este token para ejecutar una secuencia de comandos Velocity en los mensajes de correo electrónico. Obtenga más información <a href="https://developers.marketo.com/documentation/email-scripting/" title="Seguir vínculo" rel="nofollow">aquí</a>. </td> 
  </tr> 
  <tr> 
   <td>Número<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Cualquier entero. Puede incluso ser negativo.</td> 
  </tr> 
  <tr> 
   <td>Texto enriquecido <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Esto es HTML. Utilícelo en correos electrónicos y páginas de aterrizaje.</td> 
  </tr> 
  <tr> 
   <td>Puntuación <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilice este token en el paso <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">del flujo de puntuación de cambio</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">Campaña SFDC <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">Utilice este token para permitir que los leads que formen parte de un Programa de marketing también se agreguen a cualquier Campaña de SFDC.</td> 
  </tr> 
  <tr> 
   <td>Texto <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Sólo un texto. Utilícelo cuando el HTML sea exagerado. El límite de tamaño de los tokens de texto es de 524.288 caracteres (UTF-8) o 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Mis tokens no se resolverán al enviar un correo electrónico desde Sales Insight en Microsoft Dynamics o Salesforce; solo se rellenarán los tokens estándar (posible cliente, Compañía, etc.). Sin embargo, los valores predeterminados para los tokens _funcionarán_.

## Anidado de tokens {#nesting-tokens}

Al crear un nuevo token, otros objetos del árbol pueden hacer referencia a él. Hay una estructura de nombres para la que se creó el token para facilitar la administración.

* **Token local:** el token se creó en ese programa o carpeta.
* **Token heredado:** el token se creó en el árbol en algún lugar de un programa o carpeta de nivel superior.
* **Token anulado:** el token se heredó y, a continuación, alguien hizo una excepción en este programa o carpeta.

Puede crear variables globales y luego anularlas en niveles inferiores en el árbol.

Mover programas y carpetas también afecta a los tokens. Compruebe siempre que las referencias no estén rotas durante el movimiento.

>[!NOTE]
>
>Si el correo electrónico que envía desde un programa de participación es un correo electrónico secundario de un programa predeterminado (no local para el programa de participación), cualquier Mi token utilizado en el correo electrónico se resuelve a partir del programa predeterminado en el que reside el correo electrónico secundario.

>[!MORELIKETHIS]
>
>* [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Administración de mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

