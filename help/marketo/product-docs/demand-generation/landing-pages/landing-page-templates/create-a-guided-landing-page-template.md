---
unique-page-id: 7515401
description: Aprenda a crear una plantilla de página de aterrizaje guiada en Marketo. Utilice la sintaxis para definir regiones editables y variables para el editor guiado.
title: Crear una plantilla de la página de destino guiada
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
TQID: https://experienceleague.adobe.com/0dAw-HmJskYDA8uvu4ffMPPWwaQV3M-l8-kxLN-Vx-o
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: b2861922f7d2732a3286bab93243bdc0515a5995
workflow-type: tm+mt
source-wordcount: 1132
ht-degree: 21%

---

# Crear una plantilla de la página de destino guiada {#create-a-guided-landing-page-template}

Las plantillas de página de aterrizaje guiada tienen una sintaxis especial. Utilice esta sintaxis para especificar qué se puede personalizar y dónde terminará el contenido en cada página de aterrizaje creada a partir de la plantilla. Solo las regiones o variables que especifique como editables estarán disponibles para la personalización en el editor de páginas de aterrizaje &quot;Guiado&quot;.

>[!TIP]
>
>El uso de convenciones de nomenclatura claras facilita al equipo de marketing el trabajo con la plantilla.

Existen dos maneras de declarar que algo en su página debe ser editable:

* Declare un objeto como un &quot;elemento&quot;. El creador de la página de aterrizaje podrá agregar imágenes, texto o recursos de Marketo a esas regiones especificadas.
* Declare una cadena como &quot;variable&quot;. El creador de la página de aterrizaje podrá reemplazar esa variable con una cadena, un color o un estado booleano desde una palanca true/false.

## Elementos editables {#editable-elements}

Los elementos se declaran agregando un elemento DOM normal a la plantilla y decorando el elemento con un nombre de clase específico de Marketo.

## Texto {#text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [con el Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Atributos necesarios:

**class**: &quot;mktoText&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:

El contenido de un elemento con clase mktoText (si se proporciona) se utilizará como valor predeterminado para el área editable.

Ejemplo: `<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Imagen {#image}

Tiene dos opciones para definir elementos de imagen editables. Puede usar un `<div>`, que especifica el contenedor en el que se insertará la imagen, o una etiqueta `<img>`.

## Opción 1: usar un `<div>` {#option-use-a-div}

Atributos necesarios:

clase: &quot;mktoImg&quot;
id: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
mktoName : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:
mktoImgClass: String. El valor aquí se añadirá al atributo class del elemento `<img>` dentro del div.

Ejemplo: `<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opción 2 - Usar un `<img>` {#option-use-a-img}

Atributos necesarios:

clase: &quot;mktoImg&quot;
id: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
mktoName : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:

src: URL de cadena. Se utilizará como valor predeterminado para la imagen.

Ejemplo: `<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Al utilizar la versión `<img>`, el HTML procesado contendrá un contenedor div generado alrededor de la etiqueta `<img>`. Se establecerá en la clase &quot;mktoImg mktoGen&quot; y se mostrará :inline-block.

## Formulario {#form}

Atributos necesarios:

**class**: &quot;mktoForm&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo: `<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Fragmento {#snippet}

Atributos necesarios:

**class**: &quot;mktoSnippet&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo: `<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Compartir botón {#share-button}

Atributos necesarios:

**class**: &quot;mktoShareButton&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo: `<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Vídeo {#video}

>[!NOTE]
>
>Al utilizar el elemento de vídeo en una página de aterrizaje, Marketo solo admite vídeos de YouTube. Si utiliza otro servicio, le recomendamos que utilice un cuadro de texto enriquecido y pegue el código incrustado del vídeo.

Atributos necesarios:

**clase**: &quot;mktoVideo&quot;
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Ejemplo: `<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Variables editables {#editable-variables}

Todos los tipos de variables se utilizan haciendo referencia al valor de su atributo id dentro de una secuencia de caracteres ${ }. Se pueden utilizar en cualquier parte del documento, excepto en el interior de otras declaraciones de variables.

Ejemplo: `${var1}`

**Declaración:**

Las variables se declaran como metaetiquetas dentro del elemento `<head>` de la plantilla. Existen tres tipos de variables disponibles para su uso: cadena, color y booleano.

## Cadena {#string}

Atributos necesarios:

**clase** : &quot;mktoString&quot;,
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:

**default**: valor de cadena para el atributo. Vacío si no se proporciona ninguno.
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controla si el valor se imprimirá sin omitir HTML. Si no se establece, el valor predeterminado es &quot;false&quot;.

Ejemplo básico: `<meta class="mktoString" id="var1" mktoName="My Variable">`

Ejemplo con todos los atributos: `<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Color {#color}

Atributos necesarios:

**clase** : &quot;mktoColor&quot;,
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:

**default**: código de color de carácter HEX de 7 dígitos. P. ej.: #336699

Ejemplo básico: `<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Ejemplo con todos los atributos: `<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Atributos necesarios:

**clase** : &quot;mktoBoolean&quot;,
**id**: cadena de ID. Solo contiene letras, números, guiones “-” y guiones bajos “_”. No se permiten espacios. El nombre debe ser único.
**mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de páginas de aterrizaje. Una práctica recomendada es utilizar un nombre descriptivo.

Opcional:

**predeterminado**: cadena booleana. Los controles &quot;true&quot; o &quot;false&quot; si el valor comienza en la posición ON u OFF. &quot;false&quot; si no se proporciona.
**false_value**: String. Valor que se va a insertar para la variable cuando está en la posición OFF. &quot;false&quot; si no se proporciona.
**true_value**: String. Valor que se va a insertar para la variable cuando está en la posición ON. &quot;true&quot; si no se proporciona.
**false_value_name**: String. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición OFF. &quot;OFF&quot; si no se proporciona.
**true_value_name**: String. Nombre para mostrar que se mostrará en el editor de páginas de aterrizaje cuando el valor esté en la posición ON. &quot;ON&quot; si no se proporciona.

Ejemplo básico: `<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Ejemplo con todos los atributos: `<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="false" true_value="block" false_value="none" true_value_name="Show" false_value_name="Hide">`

El ejemplo siguiente muestra un caso de uso común en el que una variable booleana controla la visibilidad de un elemento css estableciendo el valor de la propiedad de visualización css en &quot;block&quot; o &quot;none&quot; para mostrar/ocultar un elemento por ID con CSS. El editor de la página de aterrizaje utilizará el nombre para mostrar Mostrar/Ocultar en lugar de OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Los tokens de programa (my.token) también se pueden usar en cualquier lugar de las páginas de aterrizaje guiadas o de forma libre.
