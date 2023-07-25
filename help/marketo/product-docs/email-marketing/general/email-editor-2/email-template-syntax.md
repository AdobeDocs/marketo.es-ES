---
unique-page-id: 11371040
description: Sintaxis de plantillas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Sintaxis de plantilla de correo electrónico
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# Sintaxis de plantilla de correo electrónico {#email-template-syntax}

En la nueva experiencia de Marketo Email 2.0, las plantillas de correo electrónico están compuestas por cualquier combinación de elementos, variables, módulos o contenedores. Cada se define añadiendo sintaxis específica de Marketo al HTML. Las plantillas de correo electrónico antiguas (v1.0) se admiten en el Editor de correo electrónico 2.0; sin embargo, no incluirán todas las funciones del nuevo Editor.

La sintaxis del correo electrónico de Marketo solo funciona en plantillas y correos electrónicos individuales; sí lo hace **no** funciona si está incrustado en fragmentos o tokens de texto enriquecido.

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
* Videos

## Texto enriquecido {#rich-text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [uso del Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Existen dos formas de definir un elemento de texto enriquecido dentro de una plantilla de correo electrónico: mktEditable y mktoText. Tenga en cuenta que un elemento de texto enriquecido siempre se puede convertir en un fragmento de código desde el editor de correo electrónico.

### Opción 1: mktEditable {#option-mkteditable}

Dado que Email Editor 2.0 es compatible con versiones anteriores, algunas plantillas de correo electrónico antiguas pueden especificar elementos de texto enriquecido añadiendo class=&quot;mktEditable&quot; en cualquier elemento del HTML. Esto sigue siendo compatible y el ID del elemento es lo que se utilizará como nombre para mostrar dentro del editor de correo electrónico.

Atributos requeridos

* **clase**: &quot;mktEditable&quot;.
* **id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.

Atributos opcionales

* **mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktEditable&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opción 2: mktoText {#option-mktotext}

Se recomienda especificar los elementos de texto enriquecido mediante la sintaxis class=&quot;mktoText&quot;. Esto garantiza que siempre haya un nombre para mostrar adecuado para el elemento.

Atributos requeridos

* **clase**: &quot;mktoText&quot;
* **id**: cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName** : cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktoText&quot; se utilizará como valor predeterminado para el elemento de texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imágenes {#images}

Tiene dos opciones para definir elementos de imagen editables. Puede usar una de las siguientes opciones `<div>`, que especifica un contenedor que el `<img>` se insertará en, o en un `<img>` etiqueta. Si tiene intención de que el usuario final simplemente elija una imagen que devuelva la URL de la imagen (en oposición al DOM), consulte &quot;variables de imagen&quot; en la sección siguiente. Las dos opciones siguientes insertan un HTML `<img>` Elemento.

### Opción 1: usar un `<div>` {#option-use-a-div}

Atributos requeridos

* **clase:** &quot;mktoImg&quot;.
* **id:** Cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName :** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** Cadena. El valor aquí se agregará al atributo class del `<img>` dentro del div.
* **mktoImgSrc:** Se utilizará como el valor predeterminado para la imagen que se coloca dentro de este div. Si se omite, se utiliza un marcador de posición.
* **mktoImgLink:** Indique que la variable `<img>` debe estar rodeado por un `<a>` con esta dirección URL de destino. El usuario puede cambiar esto en el Editor de correo electrónico.
* **mktoImgLinkTarget:** Indique que la variable `<a>` La etiqueta del atributo mktoImgLink debe utilizar este destino. No tiene efecto si mktoImgLink no se utiliza también.
* **mktoImgWidth:** Se utiliza como anchura en el `<img>`.
* **mktoImgHeight:** Se utiliza como altura en el `<img>`.
* **mktoLockImgSize:** Se utiliza para desbloquear el `<img>` propiedad height y width del elemento para que el usuario final pueda modificarlo (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** Se utiliza para bloquear el `<img>` propiedad style del elemento (el valor predeterminado es false).

Valor predeterminado (opcional)

**`<img>`**: se utilizará como `<img>` elemento en el que se colocará la imagen. Resulta útil si desea agregar estilos en línea a la imagen. Recuerde incluir los elementos circundantes `<a> </a>` , de modo que si el usuario añade un vínculo, no se eliminará su estilo.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opción 2: usar una \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Esta opción no permite a los usuarios finales añadir un vínculo a su imagen. Utilice la opción 1 si esto es importante para la plantilla.

Atributos requeridos

* **clase:** &quot;mktoImg&quot;.
* **id:** Cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.  Valor predeterminado (opcional)
* **src:** Se utilizará como valor predeterminado para la imagen. Si se omite, se utiliza un marcador de posición.
* **mktoLockImgSize:** Se utiliza para desbloquear el `<img>` propiedad height y width del elemento para que el usuario final pueda modificarlo (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** Se utiliza para bloquear el `<img>` propiedad style del elemento (el valor predeterminado es false).

Ejemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Fragmentos {#snippets}

Si define una región como un fragmento, los usuarios finales podrán elegir el aprobado [Fragmento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)les gustaría insertar en esta región. Aunque los elementos de texto enriquecido se pueden convertir en fragmentos de código desde el editor de correo electrónico, al definir una región específicamente como fragmento de código, no se pueden convertir en texto enriquecido. Puede especificar una región de fragmento de código mediante una `<div>` with class=&quot;mktoSnippet&quot;

Atributos requeridos

* **id:** Cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Valor predeterminado (opcional)

**mktoDefaultSnippetId**: ID numérico del fragmento de Marketo que debería aparecer de forma predeterminada (solo funcionará si existe un fragmento con ese ID y se aprueba en ese espacio de trabajo).

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vídeo {#video}

Si define una región como Vídeo, los usuarios finales podrán insertar una URL de YouTube o Vimeo que se mostrará como una imagen en miniatura (con el botón &quot;reproducir&quot;) dentro del correo electrónico. Puede especificar una región de vídeo mediante una `<div>` with class=&quot;mktoVideo&quot;

Atributos requeridos

* **id:** Cadena de ID. Solo contiene letras, números, guiones &quot;-&quot; y guiones bajos &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** Cadena. El valor aquí se añade al atributo class de la miniatura de vídeo `<img>` dentro del div.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Las variables son como tokens. Primero debe definirlos dentro de la variable `<head>` de la plantilla de correo electrónico mediante `<meta>` a continuación, utilícelas tantas veces como desee en toda la plantilla. Como se definen en la plantilla, el usuario final podrá modificar sus valores según sus reglas. Tenga en cuenta que puede definir una variable como de ámbito local o global. Si utiliza una variable dentro de un &quot;módulo&quot; (consulte a continuación) y un usuario final duplica ese módulo, las variables locales tendrán valores independientes, mientras que las variables globales se aplicarán a ambos módulos.

## Cadena {#string}

Si especifica una variable como String, el usuario final podrá introducir texto en un cuadro de texto del editor de correo electrónico. Puede especificar una variable de cadena mediante `<meta>` with class=&quot;mktoString&quot;

Atributos requeridos

* **id:** Cómo se hace referencia a la variable en la plantilla de correo electrónico.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **allowHTML:** Booleano. Controla si el valor de la variable es de escape HTML. Si se omite, el valor predeterminado es False.
* **predeterminado**: Valor predeterminado para la cadena. Vacío si se omite.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Si especifica una variable como una lista, el usuario final podrá elegir entre un conjunto de valores definidos en el editor de correo electrónico. Puede especificar una Variable de lista mediante `<meta>` with class=&quot;mktoList&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.
* **valores:** Lista de valores separados por comas. Debe tener al menos una cadena.

Atributos opcionales

* **valor predeterminado:** Valor predeterminado de la lista desplegable de selección. Si se omite, se utiliza el primer valor del atributo &quot;values&quot;.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Si especifica una variable como Número, el usuario final podrá introducir un número en el editor de correo electrónico. Puede especificar una variable Number utilizando `<meta>` with class=&quot;mktoNumber&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.
* **valor predeterminado:** Valor numérico predeterminado para la variable.

Atributos opcionales

* **min:** Valor mínimo aceptado.
* **máximo:** Valor máximo aceptado.
* **unidades:** Unidades que se van a anexar al valor numérico (por ejemplo: px, pt, em, etc.) cuando se muestra en el Editor de correo electrónico, así como en el código resultante.
* **paso:** Cuántas unidades debe aumentar/disminuir la variable numérica en (0,1, 1, 10, etc.). Si se omite, el valor predeterminado es 1.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Color {#color}

Si especifica una variable como Color, el usuario final podrá introducir un valor de color hexadecimal o elegir un color del selector de color dentro del editor de correo electrónico. La variable Color se especifica mediante `<meta>` with class=&quot;mktoColor&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** Valor predeterminado para el color. Código de color hexadecimal de 6 dígitos. Ejemplo: #ffffff.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Si especifica una variable como Boolean, el usuario final podrá activar o desactivar la opción en el editor de correo electrónico. Puede especificar una variable booleana mediante `<meta>` with class=&quot;mktoBoolean&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** Valor booleano que determina el estado predeterminado del conmutador. False si se omite.
* **false_value:** Valor que se inserta cuando la palanca está en la posición OFF. False si se omite.
* **true_value:** Valor que se inserta cuando el conmutador se encuentra en la posición ON. True si se omite.
* **nombre_valor_falso:** IU mostrada en la opción cuando está en la posición OFF. False si se omite.
* **true_value_name:** Interfaz de usuario que se muestra en el conmutador cuando se encuentra en la posición ON. True si se omite.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloque de HTML {#html-block}

Si especifica una variable como un bloque HTML, el usuario final podrá introducir el HTML textual desde el editor de correo electrónico. Puede especificar una variable de bloque de HTML mediante `<meta>` with class=&quot;mktoHTML&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** Valor codificado por el HTML que sirve como contenido predeterminado del bloque.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable de imagen {#image-variable}

Si especifica una variable como Imagen, el usuario final podrá elegir una imagen del selector de imágenes dentro del editor de correo electrónico. La URL de imagen seleccionada será el valor de la variable. Puede especificar una variable de imagen mediante `<meta>` with class=&quot;mktoImg&quot;

Atributos requeridos

* **id**: Cómo hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **valor predeterminado:** URL de imagen predeterminada para el elemento.
* **mktoModuleScope**: booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Declaración de ejemplo:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Los módulos son secciones con plantillas definidas en el nivel de plantilla que se mostrarán a los usuarios finales para que las inserten en sus correos electrónicos. Debido a que ha creado previamente estos módulos, puede asegurarse de que interactuarán con el resto del contenido del correo electrónico correctamente (de forma totalmente adaptable). Solo puede colocar un módulo en un contenedor.

>[!IMPORTANT]
>
>Cuando se genera un correo electrónico a partir de una plantilla de correo electrónico que contiene componentes de módulo definidos, cualquier cambio realizado en los módulos de la plantilla **no** ser insertado en dicho correo electrónico.

**Para contenedores de tipo `<table>`, `<tbody>`, `<thead>`, o `<tfoot>`:**

Especificado mediante `<tr>` with class=&quot;mktoModule&quot;

**Para contenedores de tipo `<td>`:**

Especificado mediante `<table>` with class=&quot;mktoModule&quot;

Atributos requeridos

* **id**: Cómo hace referencia al módulo en la plantilla de correo electrónico.
* **mktoName**: cadena. Este es el nombre para mostrar que se mostrará en el editor de correo electrónico 2.0. Una práctica recomendada es utilizar un nombre descriptivo.

Atributos opcionales

* **mktoActive:** Determina si este módulo aparece en la lista de módulos del editor de correo electrónico. El valor predeterminado es True. Si es false, un usuario final no puede agregar el módulo a un correo electrónico.
* **mktoAddByDefault:** Determina si este módulo estará en el lienzo de un nuevo correo electrónico que utilice esta plantilla tras la creación. El valor predeterminado es true (si mktoActive es false, se omite este valor).

>[!NOTE]
>
>Los valores de clase que contienen sintaxis de Marketo (es decir, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (por ejemplo mktoimgwidth, mktoname) no están disponibles.

## Contenedores {#containers}

Un contenedor contiene módulos y define dónde se pueden colocar. Cuando los usuarios finales reordenan e insertan módulos en su correo electrónico, el contenedor controla hacia dónde pueden ir.

**Especificado mediante `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` with class=&quot;mktoContainer&quot;**

Atributos requeridos

**id**: Cómo hace referencia al módulo en la plantilla de correo electrónico.

>[!CAUTION]
>
>Los contenedores solo pueden contener módulos: si hay algo más presente, el contenedor se considera no válido. Solo se permite un contenedor por plantilla.
