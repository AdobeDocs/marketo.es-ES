---
unique-page-id: 7515401
description: 'Creación de una plantilla de página de aterrizaje guiada: documentos de Marketo, documentación del producto'
title: Crear una plantilla de página de aterrizaje guiada
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 1%

---

# Crear una plantilla de página de aterrizaje guiada {#create-a-guided-landing-page-template}

Las plantillas de página de aterrizaje guiada tienen una sintaxis especial. Utilice esta sintaxis para especificar qué se puede personalizar y dónde terminará el contenido en cada página de aterrizaje creada a partir de la plantilla. Solo las regiones o variables que especifique como editables estarán disponibles para la personalización en el editor de páginas de aterrizaje &quot;Guiado&quot;.

>[!TIP]
>
>Use buenas convenciones de nomenclatura y su equipo de marketing se enamorará de usted.

Existen dos maneras de declarar que algo en su página debe ser editable:

* Declare un objeto como un &quot;elemento&quot;. El creador de la página de aterrizaje podrá agregar imágenes, texto o recursos de Marketo a esas regiones especificadas.
* Declare una cadena como &quot;variable&quot;. El creador de la página de aterrizaje podrá reemplazar esa variable con una cadena, un color o un estado booleano desde una palanca true/false.

## Elementos editables {#editable-elements}

Los elementos se declaran agregando un elemento DOM normal a la plantilla y decorando el elemento con un nombre de clase específico de Marketo.

## Texto {#text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [con el Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Atributos necesarios:\
**class**: &quot;mktoText&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
El contenido de un elemento con clase mktoText (si se proporciona) se utilizará como valor predeterminado para el área editable.

Ejemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Imagen {#image}

Tiene dos opciones para definir elementos de imagen editables. Puede usar un `<div>`, que especifica el contenedor en el que se insertará la imagen, o una etiqueta `<img>`.

## Opción 1: usar `<div>` {#option-use-a-div}

Atributos necesarios:

clase: &quot;mktoImg&quot;\
id: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
mktoImgClass: String. El valor aquí se agregará al atributo class del elemento `<img>` dentro del div.

Ejemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opción 2 - Usar un `<img>` {#option-use-a-img}

Atributos necesarios:\
clase: &quot;mktoImg&quot;\
id: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
src: URL de cadena. Se utilizará como valor predeterminado para la imagen.

Ejemplo:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Al utilizar la versión `<img>`, el HTML procesado contendrá un contenedor div generado alrededor de la etiqueta `<img>`. Se establecerá en clase .&quot;mktoImg.mktoGen,&quot; y se mostrarán:inline-block.

## Formulario {#form}

Ejemplo: Atributos requeridos:\
**class**: &quot;mktoForm&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Fragmento {#snippet}

Atributos necesarios:\
**class**: &quot;mktoSnippet&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Compartir botón {#share-button}

Atributos necesarios:\
**class**: &quot;mktoShareButton&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Vídeo {#video}

>[!NOTE]
>
>Al utilizar el elemento de vídeo en una página de aterrizaje, Marketo solo admite vídeos de YouTube. Si utiliza otro servicio, le recomendamos que utilice un cuadro de texto enriquecido y pegue el código incrustado del vídeo.

Atributos necesarios:
**clase**: &quot;mktoVideo&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Sondeo {#poll}

Atributos necesarios:\
**clase**: &quot;mktoPoll&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Referencia {#referral}

Atributos necesarios:\
**clase**: &quot;mktoReferral&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Sorteos {#sweepstakes}

Atributos necesarios:\
**clase**: &quot;mktoSweepstakes&quot;\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Variables editables {#editable-variables}

Todos los tipos de variables se utilizan haciendo referencia al valor de su atributo id dentro de una secuencia de caracteres ${ }. Se pueden utilizar en cualquier parte del documento, excepto en el interior de otras declaraciones de variables.

Ejemplo:

`${var1}`

**Declaración:**

Las variables se declaran como metaetiquetas dentro del elemento `<head>` de la plantilla. Existen tres tipos de variables disponibles para su uso: cadena, color y booleano.

## Cadena {#string}

Atributos necesarios:\
**clase** : &quot;mktoString&quot;,\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**default**: valor de cadena para el atributo. Vacío si no se proporciona ninguno.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controla si el valor se imprimirá sin que se escape el HTML. Si no se establece, el valor predeterminado es &quot;false&quot;.

Ejemplo básico:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Ejemplo con todos los atributos:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Color {#color}

Atributos necesarios:\
**clase** : &quot;mktoColor&quot;,\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**default**: código de color de carácter HEX de 7 dígitos. P. ej.: #336699

Ejemplo básico:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Ejemplo con todos los atributos:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Atributos necesarios:\
**clase** : &quot;mktoBoolean&quot;,\
**id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**predeterminado**: cadena booleana. Los controles &quot;true&quot; o &quot;false&quot; si el valor comienza en la posición ON u OFF. &quot;false&quot; si no se proporciona.\
**false_value**: String. Valor que se va a insertar para la variable cuando está en la posición OFF. &quot;false&quot; si no se proporciona.\
**true_value**: String. Valor que se va a insertar para la variable cuando está en la posición ON. &quot;true&quot; si no se proporciona.\
**false_value_name**: String. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición OFF. &quot;OFF&quot; si no se proporciona.\
**true_value_name**: String. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición ON. &quot;ON&quot; si no se proporciona.

Ejemplo básico:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Ejemplo con todos los atributos:

Este ejemplo muestra un caso de uso común en el que una variable booleana controla la visibilidad de un elemento css estableciendo el valor de la propiedad de visualización css en &quot;block&quot; o &quot;none&quot; para mostrar/ocultar un elemento por ID con CSS. El editor de la página de aterrizaje utilizará el nombre para mostrar Mostrar/Ocultar en lugar de OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Los tokens de programa (my.token) también se pueden usar en cualquier lugar de las páginas de aterrizaje guiadas o de forma libre.
