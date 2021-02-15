---
unique-page-id: 11371040
description: Sintaxis de la plantilla de correo electrónico - Documentos de marketing - Documentación del producto
title: Sintaxis de la plantilla de correo electrónico
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 0%

---


# Sintaxis de plantilla de correo electrónico {#email-template-syntax}

En la nueva experiencia de correo electrónico 2.0 de Marketing, las plantillas de correo electrónico están compuestas por cualquier combinación de elementos, variables, módulos o Contenedores. Cada una de ellas se define agregando sintaxis específica de Marketing a su HTML. Las plantillas de correo electrónico antiguas (v1.0) son compatibles con el Editor de correo electrónico 2.0; sin embargo, no incluirán todas las funciones del nuevo editor.

La sintaxis de correo electrónico de marketing solo funciona en plantillas y correos electrónicos individuales; **no** funciona si está incrustado en fragmentos o tokens de texto enriquecido.

>[!NOTE]
>
>La compatibilidad con el marketing no está configurada para ayudar con CSS/HTML. Si no está familiarizado con CSS/HTML, consulte a su desarrollador.

>[!CAUTION]
>
>Los valores de clase que contienen sintaxis de marketing (por ejemplo, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (por ejemplo, mktoimgwidth, mktoname) no lo son.

## Elementos {#elements}

Los elementos son regiones de contenido que se definen como editables en la plantilla de correo electrónico. La experiencia de edición de un elemento es única para su tipo y oferta una forma sencilla de trabajar con contenido. Los elementos posibles que se pueden incluir en una plantilla de correo electrónico son:

* Texto enriquecido
* Imágenes
* Recortes
* Vídeos

## Texto enriquecido {#rich-text}

Si define una región como texto enriquecido, los usuarios podrán editar su contenido [con el Editor de texto enriquecido](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md) de Marketing Cloud. Existen dos formas de definir un elemento de texto enriquecido dentro de una plantilla de correo electrónico: mktEditable y mktoText. Tenga en cuenta que siempre se puede convertir un elemento de texto enriquecido en un fragmento desde el editor de correo electrónico.

### Opción 1 - mktEditable {#option-mkteditable}

Dado que el Editor de correo electrónico 2.0 es compatible con versiones anteriores, algunas plantillas de correo electrónico antiguas pueden especificar elementos de texto enriquecido agregando class=&quot;mktEditable&quot; en cualquier elemento HTML. Esto sigue siendo compatible y el ID del elemento es lo que se utilizará como nombre para mostrar dentro del editor de correo electrónico.

Atributos requeridos

* **clase**: &quot;mktEditable&quot;.
* **id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.

Atributos opcionales

* **mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado

El contenido dentro del elemento HTML (si se proporciona) con class=&quot;mktEditable&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opción 2 - mktoText {#option-mktotext}

Se recomienda especificar elementos de texto enriquecido con la sintaxis class=&quot;mktoText&quot;. Esto garantiza que siempre haya un nombre para mostrar adecuado para el elemento.

Atributos requeridos

* **clase**: &quot;mktoText&quot;
* **id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado

El contenido dentro del elemento HTML (si se proporciona) con class=&quot;mktoText&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imágenes {#images}

Existen dos opciones para definir elementos de imagen editables. Puede utilizar una etiqueta `<div>`, que especifica un contenedor en el que se insertará el `<img>` o una etiqueta `<img>`. Si desea que el usuario final simplemente elija una imagen que devuelva la dirección URL de la imagen (a diferencia del DOM), consulte &quot;variables de imagen&quot; en la sección siguiente. Las dos opciones siguientes insertarán un elemento HTML `<img>`.

### Opción 1: Usar un `<div>` {#option-use-a-div}

Atributos requeridos

* **clase:** &quot;mktoImg&quot;.
* **id:cadena** de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** String. El valor aquí se agregará al atributo de clase del elemento `<img>` dentro del div.
* **mktoImgSrc:** Se utilizará como valor predeterminado para la imagen que se coloca dentro de este div. Si se omite, se utiliza un marcador de posición.
* **mktoImgLink:** indique que la  `<img>` etiqueta debe estar rodeada por una  `<a>` etiqueta con esta dirección URL de destino. El usuario puede cambiar esto en el Editor de correo electrónico.
* **mktoImgLinkTarget:** indique que la  `<a>` etiqueta del atributo mktoImgLink debe utilizar este destinatario. No tiene ningún efecto si no se utiliza mktoImgLink.
* **mktoImgWidth:** se utiliza como la anchura en el  `<img>`.
* **mktoImgHeight:** se utiliza como altura en el  `<img>`elemento adjunto.
* **mktoLockImgSize:** se utiliza para desbloquear la propiedad height y width del  `<img>` elemento para que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** se utiliza para bloquear la propiedad de estilo del  `<img>` elemento (el valor predeterminado es false).

Valor predeterminado (opcional)

**`<img>`**:: Se utilizará como  `<img>` elemento en el que se colocará la imagen. Resulta útil si desea añadir estilo en línea a la imagen. Recuerde incluir las etiquetas `<a> </a>` que lo rodean, de modo que si el usuario agrega un vínculo, el estilo no se depurará.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opción 2 - Usar una \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Esta opción no permite que los usuarios finales agreguen un vínculo a su imagen. Utilice la opción 1 si esto es importante para la plantilla.

Atributos requeridos

* **clase:** &quot;mktoImg&quot;.
* **id:cadena** de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.  Valor predeterminado (opcional)
* **src:** Se utilizará como valor predeterminado para la imagen. Si se omite, se utiliza un marcador de posición.
* **mktoLockImgSize:** se utiliza para desbloquear la propiedad height y width del  `<img>` elemento para que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** se utiliza para bloquear la propiedad de estilo del  `<img>` elemento (el valor predeterminado es false).

Ejemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Fragmentos {#snippets}

Si define una región como un fragmento de código, los usuarios finales podrán elegir qué fragmento de código aprobado [](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)desea insertar en esta región. Aunque los elementos de texto enriquecido se pueden convertir en fragmentos de texto desde el editor de correo electrónico, cuando define una región específicamente como un fragmento de código, no se puede convertir a texto enriquecido. Puede especificar una región de fragmentos con un `<div>` con class=&quot;mktoSnippet&quot;

Atributos requeridos

* **id:cadena** de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado (opcional)

**mktoDefaultSnippetId**: El ID numérico del fragmento de marketing que debe aparecer de forma predeterminada (solo funcionará si existe un fragmento con ese ID y se aprueba en esa área de trabajo).

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Video {#video}

Si define una región como un vídeo, los usuarios finales podrán insertar una URL de YouTube o Vimeo que se mostrará como una imagen en miniatura (con el botón &quot;reproducir&quot;) dentro del correo electrónico. Puede especificar una región de vídeo mediante `<div>` con class=&quot;mktoVideo&quot;

Atributos requeridos

* **id:cadena** de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** String. El valor aquí se agregará al atributo de clase de la miniatura de vídeo `<img>` dentro del div.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Las variables son como tokens. Primero debe definirlos dentro de la sección `<head>` de la plantilla de correo electrónico mediante etiquetas `<meta>` y luego usarlos tantas veces como desee en toda la plantilla. Dado que están definidos en la plantilla, el usuario final podrá modificar sus valores según sus reglas. Tenga en cuenta que puede definir una variable como local o global en el ámbito. Si utiliza una variable dentro de un &quot;Módulo&quot; (ver más adelante) y un usuario final duplicado ese módulo, las variables locales tendrán valores independientes, mientras que las variables globales se aplicarán a ambos módulos.

## Cadena {#string}

Si especifica una variable como String, el usuario final podrá introducir texto en un cuadro de texto en el editor de correo electrónico. Especifique una variable String usando `<meta>` con class=&quot;mktoString&quot;

Atributos requeridos

* **id:** Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **allowHTML:** Boolean. Controla si el valor de la variable es de escape HTML. Si se omite, el valor predeterminado es False.
* **predeterminado**: Valor predeterminado de la cadena. En blanco si se omite.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Si especifica una variable como Lista, el usuario final podrá elegir entre un conjunto de valores que defina en el editor de correo electrónico. Especifique una variable de Lista mediante `<meta>` con class=&quot;mktoList&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.
* **valores:lista de valores separados por** comas. Debe tener al menos una cadena.

Atributos opcionales

* **predeterminado:valor** predeterminado de la lista desplegable de selección. Si se omite, se utiliza el primer valor del atributo &quot;values&quot;.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Si especifica una variable como Número, el usuario final podrá introducir un número en el editor de correo electrónico. Especifique una variable Number usando `<meta>` con class=&quot;mktoNumber&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.
* **predeterminado:valor numérico** predeterminado para la variable.

Atributos opcionales

* **valor mínimo:** mínimo aceptado.
* **valor máximo:** máximo aceptado.
* **unidades:** Unidades que se anexarán al valor numérico (por ejemplo: px, pt, em, etc.) cuando se muestra en el Editor de correo electrónico, así como en el código resultante.
* **paso:** cuántas unidades debe aumentar o disminuir la variable de número (0.1, 1, 10, etc.). Si se omite, el valor predeterminado es 1.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Color {#color}

Si especifica una variable como Color, el usuario final podrá introducir un valor de color hexadecimal o elegir un color del selector de color dentro del editor de correo electrónico. Especifique una variable Color usando `<meta>` con class=&quot;mktoColor&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:valor** predeterminado para el color. Código de color hexadecimal de 6 dígitos. Por ejemplo: #ffffff.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Si especifica una variable como booleana, el usuario final podrá activar o desactivar la opción en el editor de correo electrónico. Especifique una variable booleana con `<meta>` class=&quot;mktoBoolean&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **default:valor** booleano que determina el estado predeterminado del conmutador. False si se omite.
* **false_value:** Valor que se insertará cuando el alternador esté en la posición OFF. False si se omite.
* **true_value:** Valor que se insertará cuando el alternador esté en la posición ON. True si se omite.
* **false_value_name:** UI que se muestra en el conmutador cuando se encuentra en la posición OFF. False si se omite.
* **true_value_name:** UI que se muestra en el conmutador cuando se encuentra en la posición ON. True si se omite.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloque HTML {#html-block}

Si especifica una variable como un bloque HTML, el usuario final podrá introducir HTML literal desde el editor de correo electrónico. Especifique una variable de bloque HTML mediante `<meta>` con class=&quot;mktoHTML&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:valor codificado** HTML para que sirva como contenido predeterminado del bloque.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable de imagen {#image-variable}

Si especifica una variable como imagen, el usuario final podrá elegir una imagen del selector de imágenes dentro del editor de correo electrónico. La dirección URL de imagen seleccionada será el valor de la variable. Especifique una variable de imagen con `<meta>` class=&quot;mktoImg&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **default:URL de imagen** predeterminada para el elemento.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Los módulos son secciones con plantillas definidas en el nivel de plantilla que se mostrarán para que los usuarios finales los inserten en su correo electrónico. Debido a que ya ha creado estos módulos, puede asegurarse de que interactuarán con el resto del contenido del correo electrónico de forma correcta (de forma totalmente adaptable). Solo puede colocar un módulo en un contenedor.

**Para contenedores de tipo  `<table>`,  `<tbody>`,  `<thead>`o  `<tfoot>`:**

Especificado con `<tr>` con class=&quot;mktoModule&quot;

**Para contenedores de tipo  `<td>`:**

Especificado con `<table>` con class=&quot;mktoModule&quot;

Atributos requeridos

* **id**: Cómo se hace referencia al módulo dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoActive:** determina si este módulo aparece en la lista de módulos dentro del editor de correo electrónico. El valor predeterminado es true. Si es false, un usuario final no puede agregar el módulo a un correo electrónico.
* **mktoAddByDefault:** determina si este módulo estará en el lienzo de un nuevo correo electrónico que utilice esta plantilla al crearlo. El valor predeterminado es true (si mktoActive es false, este valor se omite).

>[!NOTE]
>
>Los valores de clase que contienen sintaxis de marketing (por ejemplo, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (por ejemplo, mktoimgwidth, mktoname) no lo son.

## Contenedores {#containers}

Un contenedor contiene los módulos y define dónde se pueden colocar. Cuando los usuarios finales reordenan e insertan módulos en su correo electrónico, el contenedor controla a dónde pueden ir.

**Especificado mediante  `<table>`,  `<tbody>`,  `<thead>`o  `<tfoot>`   `<td>` con class=&quot;mktoContainer&quot;**

Atributos requeridos

**id**: Cómo se hace referencia al módulo dentro de la plantilla de correo electrónico.

>[!CAUTION]
>
>Los contenedores solo pueden contener módulos. Si hay algo más presente, ¡el Contenedor se considera no válido! Solo se permite un contenedor por plantilla.
