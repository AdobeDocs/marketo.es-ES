---
unique-page-id: 11371040
description: Sintaxis de plantillas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Sintaxis de plantilla de correo electrónico
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 2%

---

# Sintaxis de plantilla de correo electrónico {#email-template-syntax}

En la nueva experiencia de Marketo Email 2.0, las plantillas de correo electrónico están compuestas por cualquier combinación de elementos, variables, módulos o contenedores. Cada uno se define añadiendo sintaxis específica de Marketo a la HTML. Las plantillas de correo electrónico antiguas (v1.0) se admiten en el Editor de correo electrónico 2.0; sin embargo, no incluirán todas las funciones del nuevo Editor.

La sintaxis del correo electrónico de Marketo solo funciona en plantillas y correos electrónicos individuales; **no funciona** si está incrustada en fragmentos o tokens de texto enriquecido.

>[!NOTE]
>
>La compatibilidad con Marketo no está configurada para ayudar con CSS/HTML. Si no está familiarizado con CSS/HTML, consulte a su desarrollador.

>[!CAUTION]
>
>Los valores de clase que contienen sintaxis de Marketo (es decir, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (por ejemplo mktoimgwidth, mktoname) no están disponibles.

## Elementos {#elements}

Los elementos son áreas de contenido que se definen como editables en la plantilla de correo electrónico. La experiencia de edición de un elemento es única para su tipo y ofrece una forma sencilla de trabajar con contenido. Los posibles elementos que se pueden incluir en una plantilla de correo electrónico son los siguientes:

* Texto enriquecido
* Imágenes
* Fragmentos
* Vídeos

## Texto enriquecido {#rich-text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [con el Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Existen dos formas de definir un elemento de texto enriquecido dentro de una plantilla de correo electrónico: mktEditable y mktoText. Tenga en cuenta que un elemento de texto enriquecido siempre se puede convertir en un fragmento de código desde el editor de correo electrónico.

### Opción 1: mktEditable {#option-mkteditable}

Dado que el Editor de correo electrónico 2.0 es compatible con versiones anteriores, algunas plantillas de correo electrónico antiguas pueden especificar elementos de texto enriquecido añadiendo class=&quot;mktEditable&quot; en cualquier elemento de HTML. Esto sigue siendo compatible y el ID del elemento es lo que se utilizará como nombre para mostrar dentro del editor de correo electrónico.

Atributos obligatorios

* **class**: &quot;mktEditable&quot;.
* **id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.

Atributos opcionales

* **mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktEditable&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Por ejemplo:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Opción 2: mktoText {#option-mktotext}

Se recomienda especificar los elementos de texto enriquecido mediante la sintaxis class=&quot;mktoText&quot;. Esto garantiza que siempre haya un nombre para mostrar adecuado para el elemento.

Atributos obligatorios

* **class**: &quot;mktoText&quot;
* **id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktoText&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Por ejemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Imágenes {#images}

Tiene dos opciones para definir elementos de imagen editables. Puede usar un `<div>`, que especifica el contenedor en el que se insertará el `<img>`, o una etiqueta `<img>`. Si tiene intención de que el usuario final simplemente elija una imagen que devuelva la URL de la imagen (en oposición al DOM), consulte &quot;variables de imagen&quot; en la sección siguiente. Las dos opciones siguientes insertarán un elemento `<img>` de HTML.

### Opción 1: usar `<div>` {#option-use-a-div}

Atributos obligatorios

* **clase:** &quot;mktoImg&quot;.
* **id:** cadena de identificador. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName :** cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** String. El valor aquí se agregará al atributo class del elemento `<img>` dentro del div.
* **mktoImgSrc:** Se utilizará como valor predeterminado para la imagen que se coloca dentro de este div. Si se omite, se utiliza un marcador de posición.
* **mktoImgLink:** Indica que `<img>` debe estar rodeado por una etiqueta `<a>` con esta dirección URL de destino. El usuario puede cambiar esto en el Editor de correo electrónico.
* **mktoImgLinkTarget:** Indique que la etiqueta `<a>` del atributo mktoImgLink debe utilizar este destino. No tiene efecto si mktoImgLink no se utiliza también.
* **mktoImgWidth:** se usa como ancho en el `<img>` incluido.
* **mktoImgHeight:** se usa como alto en el `<img>` incluido.
* **mktoLockImgSize:** Se utilizó para desbloquear la propiedad height y width del elemento `<img>` de modo que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** se utilizó para bloquear la propiedad de estilo del elemento `<img>` (el valor predeterminado es false).

Valor predeterminado (opcional)

**`<img>`**: para usar como el elemento `<img>` en el que se colocará la imagen. Resulta útil si desea agregar estilos en línea a la imagen. Recuerde incluir las etiquetas `<a> </a>` que lo rodean, de modo que si el usuario agrega un vínculo, no se eliminará su estilo.

Por ejemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Opción 2: usar un \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Esta opción no permite a los usuarios finales añadir un vínculo a su imagen. Utilice la opción 1 si esto es importante para la plantilla.

Atributos obligatorios

* **clase:** &quot;mktoImg&quot;.
* **id:** cadena de identificador. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.  Valor predeterminado (opcional)
* **src:** se utilizará como el valor predeterminado de la imagen. Si se omite, se utiliza un marcador de posición.
* **mktoLockImgSize:** Se utilizó para desbloquear la propiedad height y width del elemento `<img>` de modo que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** se utilizó para bloquear la propiedad de estilo del elemento `<img>` (el valor predeterminado es false).

Ejemplo:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Fragmentos {#snippets}

Si define una región como un fragmento de código, los usuarios finales podrán elegir qué [fragmento de código](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)aprobado desean insertar en esta región. Aunque los elementos de texto enriquecido se pueden convertir en fragmentos de código desde el editor de correo electrónico, al definir una región específicamente como fragmento de código, no se pueden convertir en texto enriquecido. Puede especificar una región de fragmento utilizando `<div>` con class=&quot;mktoSnippet&quot;

Atributos obligatorios

* **id:** cadena de identificador. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado (opcional)

**mktoDefaultSnippetId**: El identificador numérico del fragmento de Marketo que debería aparecer de forma predeterminada (solo funcionará si existe un fragmento con ese identificador y está aprobado en ese espacio de trabajo).

Por ejemplo:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Vídeo {#video}

Si define una región como Vídeo, los usuarios finales podrán insertar una URL de YouTube o Vimeo que se mostrará como una imagen en miniatura (con el botón &quot;reproducir&quot;) dentro del correo electrónico. Puede especificar una región de vídeo mediante `<div>` con class=&quot;mktoVideo&quot;

Atributos obligatorios

* **id:** cadena de identificador. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** String. El valor aquí se agregará al atributo class de la miniatura de vídeo `<img>` dentro del div.

Por ejemplo:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variables {#variables}

Las variables son como tokens. Primero debe definirlos dentro de la sección `<head>` de la plantilla de correo electrónico mediante las etiquetas `<meta>` y, a continuación, utilizarlos tantas veces como desee en toda la plantilla. Como se definen en la plantilla, el usuario final podrá modificar sus valores según sus reglas. Tenga en cuenta que puede definir una variable como de ámbito local o global. Si utiliza una variable dentro de un &quot;módulo&quot; (consulte a continuación) y un usuario final duplica ese módulo, las variables locales tendrán valores independientes, mientras que las variables globales se aplicarán a ambos módulos.

## Cadena {#string}

Si especifica una variable como String, el usuario final podrá introducir texto en un cuadro de texto del editor de correo electrónico. Usted especifica una variable String usando `<meta>` con class=&quot;mktoString&quot;

Atributos obligatorios

* **id:** Cómo se hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **allowHTML:** Boolean. Controla si el valor de la variable es HTML-escaped. Si se omite, el valor predeterminado es False.
* **default**: Valor predeterminado de la cadena. Vacío si se omite.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Ejemplo de uso:

`${textHeader}`

## Lista {#list}

Si especifica una variable como una lista, el usuario final podrá elegir entre un conjunto de valores definidos en el editor de correo electrónico. Usted especifica una Variable de lista usando `<meta>` con class=&quot;mktoList&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName:** String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.
* **valores:** Lista de valores separados por comas. Debe tener al menos una cadena.

Atributos opcionales

* **valor predeterminado:** valor predeterminado de la lista desplegable de selección. Si se omite, se utiliza el primer valor del atributo &quot;values&quot;.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Ejemplo de uso:

`${textFontFamily}`

## Número {#number}

Si especifica una variable como Número, el usuario final podrá introducir un número en el editor de correo electrónico. Usted especifica una variable Number usando `<meta>` con class=&quot;mktoNumber&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.
* **valor predeterminado:** valor numérico predeterminado para la variable.

Atributos opcionales

* **min:** Valor mínimo aceptado.
* **máximo:** valor máximo aceptado.
* **unidades:** unidades que se agregarán al valor numérico (p. ej.: px, pt, em, etc.) cuando se muestren en el Editor de correo electrónico, así como en el código resultante.
* **paso:** Cuántas unidades debe aumentar/disminuir la variable numérica en (0,1, 1, 10, etc.). Si se omite, el valor predeterminado es 1.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Ejemplo de uso:

`${textFontSize}`

## Color {#color}

Si especifica una variable como Color, el usuario final podrá introducir un valor de color hexadecimal o elegir un color del selector de color dentro del editor de correo electrónico. Usted especifica una variable Color usando `<meta>` con class=&quot;mktoColor&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** valor predeterminado para el color. Código de color hexadecimal de 6 dígitos. Ejemplo: #ffffff.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Ejemplo de uso:

`${textColor}`

## Booleano {#boolean}

Si especifica una variable como Boolean, el usuario final podrá activar o desactivar la opción en el editor de correo electrónico. Usted especifica una variable booleana usando `<meta>` con class=&quot;mktoBoolean&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** Valor booleano que determina el estado predeterminado del conmutador de alternancia. False si se omite.
* **false_value:** Valor que se insertará cuando el conmutador esté en la posición OFF. False si se omite.
* **true_value:** Valor que se insertará cuando el conmutador esté en la posición ON. True si se omite.
* **false_value_name:** interfaz de usuario que se muestra en la opción cuando está en la posición OFF. False si se omite.
* **true_value_name:** interfaz de usuario que se muestra en el conmutador cuando está en la posición ON. True si se omite.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Ejemplo de uso:

`${showFooter}`

## Bloque de HTML {#html-block}

Si especifica una variable como un bloque de HTML, el usuario final podrá introducir HTML literalmente desde el editor de correo electrónico. Usted especifica una variable de bloque de HTML usando `<meta>` con class=&quot;mktoHTML&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** valor codificado en HTML que servirá como contenido predeterminado del bloque.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Ejemplo de uso:

`${trackingPixel}`

## Variable de imagen {#image-variable}

Si especifica una variable como Imagen, el usuario final podrá elegir una imagen del selector de imágenes dentro del editor de correo electrónico. La URL de imagen seleccionada será el valor de la variable. Usted especifica una variable Image usando `<meta>` con class=&quot;mktoImg&quot;

Atributos obligatorios

* **id**: Cómo hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:** URL de imagen predeterminada para el elemento.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Ejemplo de uso:

`${heroBackgroundImage}`

## Módulos {#modules}

Los módulos son secciones con plantillas definidas en el nivel de plantilla que se mostrarán a los usuarios finales para que las inserten en sus correos electrónicos. Debido a que ha creado previamente estos módulos, puede asegurarse de que interactuarán con el resto del contenido del correo electrónico correctamente (de forma totalmente adaptable). Solo puede colocar un módulo en un contenedor.

>[!IMPORTANT]
>
>Cuando se genera un correo electrónico a partir de una plantilla de correo electrónico que contiene componentes de módulo definidos, cualquier cambio realizado en los módulos de la plantilla **no** se insertará en dicho correo electrónico.

**Para contenedores de tipo `<table>`, `<tbody>`, `<thead>` o `<tfoot>`:**

Especificado usando `<tr>` con class=&quot;mktoModule&quot;

**Para contenedores de tipo `<td>`:**

Especificado usando `<table>` con class=&quot;mktoModule&quot;

Atributos obligatorios

* **id**: Cómo hace referencia al módulo en la plantilla de correo electrónico.
* **mktoName**: String. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoActive:** Determina si este módulo aparece en la lista de módulos dentro del editor de correo electrónico. El valor predeterminado es True. Si es false, un usuario final no puede agregar el módulo a un correo electrónico.
* **mktoAddByDefault:** Determina si este módulo estará en el lienzo de un nuevo mensaje de correo electrónico que utilice esta plantilla al crearlo. El valor predeterminado es true (si mktoActive es false, se omite este valor).

>[!NOTE]
>
>Los valores de clase que contienen sintaxis de Marketo (es decir, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (por ejemplo mktoimgwidth, mktoname) no están disponibles.

## Contenedores {#containers}

Un contenedor contiene módulos y define dónde se pueden colocar. Cuando los usuarios finales reordenan e insertan módulos en su correo electrónico, el contenedor controla hacia dónde pueden ir.

**Especificado usando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=&quot;mktoContainer&quot;**

Atributos obligatorios

**id**: Cómo hace referencia al módulo en la plantilla de correo electrónico.

>[!CAUTION]
>
>Los contenedores solo pueden contener módulos: si hay algo más presente, el contenedor se considera no válido. Solo se permite un contenedor por plantilla.
