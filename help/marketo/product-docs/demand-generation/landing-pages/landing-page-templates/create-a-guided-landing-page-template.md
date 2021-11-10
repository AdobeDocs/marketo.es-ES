---
unique-page-id: 7515401
description: Creación de una plantilla de página de aterrizaje guiada - Documentos de Marketo - Documentación del producto
title: Crear una plantilla de página de aterrizaje guiada
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: c309b69198c6f61d7475c6d3a6b1672e045b9b4a
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 1%

---

# Crear una plantilla de página de aterrizaje guiada {#create-a-guided-landing-page-template}

Las plantillas de página de aterrizaje guiadas tienen una sintaxis especial. Utilice esta sintaxis para especificar qué es personalizable y dónde terminará el contenido en cada página de aterrizaje creada a partir de la plantilla. Solo las regiones o variables que especifique como editables estarán disponibles para la personalización dentro del editor de páginas de aterrizaje &quot;Guiado&quot;.

>[!TIP]
>
>Use buenas convenciones de nomenclatura y su equipo de marketing se enamorará de usted.

Hay dos maneras de declarar que algo en la página debería ser editable:

* Declare un objeto como &quot;elemento&quot;. El creador de páginas de aterrizaje podrá agregar imágenes, texto o recursos de Marketo a esas regiones especificadas.
* Declare una cadena como una &quot;variable&quot;. El creador de la página de aterrizaje podrá reemplazar esa variable con un estado de cadena, color o booleano de una palanca &quot;true/false&quot;.

## Elementos editables {#editable-elements}

Los elementos se declaran agregando un elemento DOM normal a la plantilla y decorando el elemento con un nombre de clase específico de Marketo.

## Texto {#text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [uso del Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Atributos requeridos:\
**class**: &quot;mktoText&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
El contenido de un elemento con la clase mktoText (si se proporciona) se utilizará como valor predeterminado para la región editable.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

## Imagen {#image}

Tiene dos opciones para definir elementos de imagen editables. Puede utilizar una `<div>`, que especifica un contenedor en el que se insertará la imagen, o un `<img>` etiqueta.

## Opción 1: usar un `<div>` {#option-use-a-div}

Atributos requeridos:

Clase : &quot;mktoImg&quot;\
id: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
mktoImgClass: Cadena. El valor aquí se agregará al atributo de clase del `<img>` dentro del div.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Opción 2: usar un `<img>` {#option-use-a-img}

Atributos requeridos:\
Clase : &quot;mktoImg&quot;\
id: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
src: URL de cadena. Se utilizará como valor predeterminado para la imagen.

Ejemplo:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Al usar la variable `<img>` versión, el HTML procesado contendrá un envoltorio div generado alrededor de la variable `<img>` etiqueta. Se establecerá en class .&quot;mktoImg.mktoGen&quot;, y se mostrará:inline-block.

## Formulario {#form}

Ejemplo: Atributos requeridos:\
**class**: &quot;mktoForm&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Fragmento {#snippet}

Atributos requeridos:\
**class**: &quot;mktoSnippet&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Botón Compartir {#share-button}

Atributos requeridos:\
**class**: &quot;mktoShareButton&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Vídeo {#video}

>[!NOTE]
>
>Al utilizar el elemento de vídeo en una página de aterrizaje, Marketo solo admite vídeos de YouTube. Si utiliza otro servicio, recomendamos utilizar un cuadro de texto enriquecido y pegar el código incrustado del vídeo.

Atributos requeridos:
**class**: &quot;mktoVideo&quot;
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Sondeo {#poll}

Atributos requeridos:\
**class**: &quot;mktoPoll&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Referencia {#referral}

Atributos requeridos:\
**class**: &quot;mktoReferral&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Sorteos {#sweepstakes}

Atributos requeridos:\
**class**: &quot;mktoSweepstakes&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variables editables {#editable-variables}

Todos los tipos de variables se utilizan haciendo referencia al valor de su atributo de id envuelto en una secuencia de caracteres ${ }. Pueden utilizarse en cualquier parte del documento, excepto dentro de otras declaraciones de variables.

Ejemplo:

`<pre data-theme="Confluence">${var1}</pre>`

**Declaración:**

Las variables se declaran como metaetiquetas dentro de la variable `<head>` elemento de la plantilla. Hay tres tipos de variables disponibles para su uso: Cadena, Color y Booleano.

## Cadena {#string}

Atributos requeridos:\
**class** : &quot;mktoString&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**default**: Valor de cadena para el atributo . En blanco si no se proporciona ninguno.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controla si el valor se imprimirá sin que el HTML haya escapado. Si no se configura de forma distinta, el valor predeterminado es &quot;false&quot;.

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Ejemplo con todos los atributos:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Color {#color}

Atributos requeridos:\
**class** : &quot;mktoColor&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**default**: Código de color de 7 dígitos HEX. Por ejemplo: &quot;#336699&quot;

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Ejemplo con todos los atributos:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booleano {#boolean}

Atributos requeridos:\
**class** : &quot;mktoBoolean&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:\
**default**: Cadena booleana. &quot;true&quot; o &quot;false&quot; controla si el valor comienza en la posición ON o OFF. &quot;false&quot; si no se proporciona.\
**false_value**: Cadena. El valor que debe insertarse para la variable cuando se encuentra en la posición OFF. &quot;false&quot; si no se proporciona.\
**true_value**: Cadena. El valor que se va a insertar para la variable cuando se encuentra en la posición ON. &quot;true&quot; si no se proporciona.\
**false_value_name**: Cadena. El nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición OFF. &quot;OFF&quot; si no se proporciona.\
**true_value_name**: Cadena. El nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición ON. &quot;ON&quot; si no se proporciona.

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Ejemplo con todos los atributos:

Este ejemplo muestra un caso de uso común en el que una variable booleana controla la visibilidad de un elemento css configurando el valor de la propiedad de visualización css en &quot;block&quot; o &quot;none&quot; para mostrar u ocultar un elemento por id con CSS. El editor de páginas de aterrizaje usará el nombre para mostrar Mostrar/Ocultar en lugar de OFF/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Los tokens de programa (my.token) también se pueden usar en cualquier lugar de las páginas de aterrizaje guiadas o de forma libre.
