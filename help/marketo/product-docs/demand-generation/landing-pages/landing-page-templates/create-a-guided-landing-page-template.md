---
unique-page-id: 7515401
description: Creación de una plantilla de Página de aterrizaje guiada - Documentos de marketing - Documentación del producto
title: Creación de una plantilla de Página de aterrizaje guiada
translation-type: tm+mt
source-git-commit: 975e048271dae6a877ae9ff5d39360b159afcc8a
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---


# Crear una plantilla de Página de aterrizaje guiada {#create-a-guided-landing-page-template}

>[!NOTE]
>
>**Buceo profundo: ¿** Cansado de leer? [Vea este fantástico ](https://youtu.be/3O7e4GdZKsM) vídeo con instrucciones paso a paso.

Las plantillas de página de aterrizaje guiadas tienen una sintaxis especial. Utilice esta sintaxis para especificar qué es personalizable y dónde terminará el contenido en cada página de aterrizaje creada a partir de la plantilla. Solo las regiones o variables que especifique como editables estarán disponibles para la personalización dentro del editor de páginas de aterrizaje &quot;Guiado&quot;.

>[!TIP]
>
>Use buenas convenciones de nombres y su equipo de mercadotecnia se enamorará de usted.

Existen dos maneras de declarar que algo en la página debe ser editable:

* Declarar un objeto como &quot;elemento&quot;. El creador de la página de aterrizaje podrá añadir imágenes, texto o recursos de marketing en las regiones especificadas.
* Declare una cadena como una &quot;variable&quot;. El creador de páginas de aterrizaje podrá reemplazar esa variable con una cadena, color o estado booleano de una palanca true/false.

## Elementos editables {#editable-elements}

Los elementos se declaran agregando un elemento DOM normal a la plantilla y, a continuación, decorando el elemento con un nombre de clase específico de Marketing.

## Texto {#text}

Si define una región como texto enriquecido, los usuarios podrán editar su contenido [con el Editor de texto enriquecido](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md) de Marketing Cloud.

Atributos requeridos:\
**clase**: &quot;mktoText&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
El contenido de un elemento con la clase mktoText (si se proporciona) se utilizará como valor predeterminado para la región editable.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Imagen {#image}

Tiene dos opciones para definir elementos de imagen editables. Puede utilizar una etiqueta `<div>`, que especifica un contenedor en el que se insertará la imagen, o una etiqueta `<img>`.

## Opción 1: Usar una <div> {#option-use-a-div}

Atributos requeridos:

class: &quot;mktoImg&quot;\
id: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
mktoImgClass: Cadena. El valor aquí se agregará al atributo de clase del elemento `<img>` dentro del div.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Opción 2: Usar un `<img>` {#option-use-a-img}

Atributos requeridos:\
class: &quot;mktoImg&quot;\
id: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
mktoName : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
src: URL de cadena. Se utilizará como valor predeterminado para la imagen.

Ejemplo:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Al utilizar la versión `<img>`, el HTML procesado contendrá un envoltorio div generado alrededor de la etiqueta `<img>`. Se establecerá en la clase .&quot;mktoImg.mktoGen,&quot; y se mostrará:inline-block.

## Formulario {#form}

Ejemplo:Atributos requeridos:\
**clase**: &quot;mktoForm&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Fragmento {#snippet}

Atributos requeridos:\
**clase**: &quot;mktoSnippet&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Botón Compartir {#share-button}

Atributos requeridos:\
**clase**: &quot;mktoShareButton&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Video {#video}

>[!NOTE]
>
>Cuando se utiliza el elemento de vídeo en una página de aterrizaje, Marketing solo admite vídeos de YouTube. Si utiliza otro servicio, recomendamos utilizar un cuadro de texto enriquecido y pegar en el código incrustado del vídeo.

Atributos requeridos:
**clase**: &quot;mktoVideo&quot;
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Encuesta {#poll}

Atributos requeridos:\
**clase**: &quot;mktoPoll&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Remisión {#referral}

Atributos requeridos:\
**clase**: &quot;mktoReferral&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Apuestas {#sweepstakes}

Atributos requeridos:\
**clase**: &quot;mktoSweepstakes&quot;\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variables editables {#editable-variables}

Todos los tipos de variables se utilizan haciendo referencia al valor de su atributo de identificación ajustado dentro de una secuencia de caracteres ${ }. Pueden utilizarse en cualquier parte del documento, excepto dentro de otras declaraciones de variables.

Ejemplo:

`<pre data-theme="Confluence">${var1}</pre>`

**Declaración:**

Las variables se declaran como etiquetas meta dentro del elemento `<head>` de la plantilla. Existen tres tipos de variables disponibles para su uso: Cadena, Color y Booleano.

## Cadena {#string}

Atributos requeridos:\
**clase** : &quot;mktoString&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
**predeterminado**: Valor de cadena para el atributo. En blanco si no se proporciona ninguno.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controla si el valor se va a imprimir sin que se escape HTML. El valor predeterminado es &quot;false&quot; si se desactiva.

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Ejemplo con todos los atributos:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Color {#color}

Atributos requeridos:\
**clase** : &quot;mktoColor&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
**predeterminado**: Código de color HEX de 7 dígitos. Por ejemplo: &quot;#336699&quot;

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Ejemplo con todos los atributos:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booleano {#boolean}

Atributos requeridos:\
**clase** : &quot;mktoBoolean&quot;,\
**id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.\
**mktoName** : Cadena. Es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Se recomienda utilizar un nombre descriptivo.

Opcional:\
**predeterminado**: Cadena booleana. &quot;true&quot; o &quot;false&quot; controla si el valor inicio en la posición ON o OFF. &quot;false&quot; si no se proporciona.\
**false_value**: Cadena. Valor que se va a insertar para la variable cuando se encuentra en la posición OFF. &quot;false&quot; si no se proporciona.\
**true_value**: Cadena. El valor que se va a insertar para la variable cuando se encuentra en la posición ON. &quot;true&quot; si no se proporciona.\
**false_value_name**: Cadena. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor se encuentre en la posición OFF. &quot;OFF&quot; si no se proporciona.\
**true_value_name**: Cadena. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición ON. &quot;ON&quot; si no se proporciona.

Ejemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Ejemplo con todos los atributos:

En este ejemplo se muestra un caso de uso común en el que una variable booleana controla la visibilidad de un elemento css estableciendo el valor de la propiedad de visualización css en &quot;block&quot; o &quot;none&quot; para mostrar u ocultar un elemento por ID con CSS. El editor de páginas de aterrizaje usará el nombre para mostrar Mostrar/Ocultar en lugar de Desactivar/Activar.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Los tokens de programa (my.token) también se pueden usar en cualquier lugar de las páginas de aterrizaje guiadas o de forma libre.
