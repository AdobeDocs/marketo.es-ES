---
unique-page-id: 11371040
description: Sintaxis de las plantillas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Sintaxis de la plantilla de correo electrónico
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# Sintaxis de la plantilla de correo electrónico {#email-template-syntax}

En la nueva experiencia de correo electrónico 2.0 de Marketo, las plantillas de correo electrónico están compuestas por cualquier combinación de elementos, variables, módulos o contenedores. Cada una de ellas se define añadiendo sintaxis específica de Marketo al HTML. Las plantillas de correo electrónico antiguas (v1.0) se admiten en el Editor de correo electrónico 2.0; sin embargo, no incluirán todas las funciones del nuevo editor.

La sintaxis de correo electrónico de Marketo solo funciona en plantillas y en correos electrónicos individuales; it **not** funciona si está incrustado en fragmentos o tokens de texto enriquecido.

>[!NOTE]
>
>La compatibilidad con Marketo no está configurada para ayudar con CSS/HTML. Si no está familiarizado con CSS/HTML, consulte a su desarrollador.

>[!CAUTION]
>
>Los valores de clase que contienen sintaxis Marketo (por ejemplo, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (es decir, mktoimgwidth, mktoname) no lo son.

## Elementos {#elements}

Los elementos son regiones de contenido que se definen como editables en la plantilla de correo electrónico. La experiencia de edición de un elemento es única para su tipo y ofrece una forma sencilla de trabajar con contenido. Los posibles elementos que se pueden incluir en una plantilla de correo electrónico son:

* Texto enriquecido
* Imágenes
* Fragmentos
* Videos

## Texto enriquecido {#rich-text}

Si define una región como Texto enriquecido, los usuarios podrán editar su contenido [uso del Editor de texto enriquecido de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Existen dos formas de definir un elemento de texto enriquecido dentro de una plantilla de correo electrónico: mktEditable y mktoText. Tenga en cuenta que un elemento de texto enriquecido siempre se puede convertir en un fragmento desde el editor de correo electrónico.

### Opción 1: mktEditable {#option-mkteditable}

Como el Editor de correo electrónico 2.0 es compatible con versiones anteriores, algunas plantillas de correo electrónico antiguas pueden especificar elementos de texto enriquecido añadiendo class=&quot;mktEditable&quot; en cualquier elemento de HTML. Esto sigue siendo compatible y el ID del elemento es lo que se utilizará como nombre para mostrar dentro del editor de correo electrónico.

Atributos requeridos

* **class**: &quot;mktEditable&quot;.
* **id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.

Atributos opcionales

* **mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktEditable&quot; se utilizará como valor predeterminado para el elemento Texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opción 2: mktoText {#option-mktotext}

Se recomienda especificar elementos de texto enriquecido utilizando la sintaxis class=&quot;mktoText&quot;. Esto garantiza que siempre haya un nombre para mostrar adecuado para el elemento.

Atributos requeridos

* **class**: &quot;mktoText&quot;
* **id**: Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName** : Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado

El contenido del elemento HTML (si se proporciona) con class=&quot;mktoText&quot; se utilizará como valor predeterminado para el elemento Texto enriquecido.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imágenes {#images}

Tiene dos opciones para definir elementos de imagen editables. Puede utilizar una `<div>`, que especifica un contenedor que `<img>` se insertará en o en `<img>` etiqueta. Si tiene intención de que el usuario final simplemente elija una imagen que devuelva la URL de la imagen (a diferencia del DOM), consulte &quot;variables de imagen&quot; en la sección siguiente. Las dos opciones siguientes insertan un HTML `<img>` elemento.

### Opción 1: usar un `<div>` {#option-use-a-div}

Atributos requeridos

* **Clase :** &quot;mktoImg&quot;.
* **id:** Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName :** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** Cadena. El valor aquí se agregará al atributo de clase del `<img>` dentro del div.
* **mktoImgSrc:** Se utilizará como valor predeterminado para la imagen que se coloca dentro de este div. Si se omite, se utiliza un marcador de posición.
* **mktoImgLink:** Indique que la variable `<img>` debe estar rodeado por un `<a>` con esta dirección URL de destino. El usuario puede cambiar esto en el Editor de correo electrónico.
* **mktoImgLinkTarget:** Indique que la variable `<a>` del atributo mktoImgLink debe utilizar este destino. No tiene ningún efecto si mktoImgLink no se utiliza también.
* **mktoImgWidth:** Se usa como la anchura del entorno. `<img>`.
* **mktoImgHeight:** Se utiliza como la altura en el adjunto. `<img>`.
* **mktoLockImgSize:** Se utiliza para desbloquear el `<img>` la propiedad height and width del elemento para que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** Se usa para bloquear la variable `<img>` propiedad style del elemento (el valor predeterminado es false).

Valor predeterminado (opcional)

**`<img>`**: Para usar como el `<img>` elemento en el que se colocará la imagen. Útil si desea agregar estilo en línea a la imagen. Recuerde incluir los alrededores `<a> </a>` , así que si el usuario agrega un vínculo, el estilo no se eliminará.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opción 2: usar un&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Esta opción no permite que los usuarios finales agreguen un vínculo a su imagen. Utilice la Opción 1 si esto es importante para la plantilla.

Atributos requeridos

* **Clase :** &quot;mktoImg&quot;.
* **id:** Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.  Valor predeterminado (opcional)
* **src:** Para usar como valor predeterminado de la imagen. Si se omite, se utiliza un marcador de posición.
* **mktoLockImgSize:** Se utiliza para desbloquear el `<img>` la propiedad height and width del elemento para que el usuario final pueda modificarla (el valor predeterminado es true si se omite).
* **mktoLockImgStyle:** Se usa para bloquear la variable `<img>` propiedad style del elemento (el valor predeterminado es false).

Ejemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Fragmentos {#snippets}

Si define una región como un fragmento de código, los usuarios finales podrán elegir qué área aprobada [Fragmento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)les gustaría insertar en esta región. Aunque los elementos de texto enriquecido pueden convertirse en fragmentos de texto desde el editor de correo electrónico, cuando define una región específicamente como un fragmento de código, no se puede convertir en texto enriquecido. Puede especificar una región de fragmento de código mediante un `<div>` con class=&quot;mktoSnippet&quot;

Atributos requeridos

* **id:** Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Valor predeterminado (opcional)

**mktoDefaultSnippetId**: El ID numérico del fragmento de código Marketo que debe aparecer de forma predeterminada (solo funcionará si existe un fragmento con ese ID y se aprueba en ese espacio de trabajo).

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vídeo {#video}

Si define una región como un vídeo, los usuarios finales podrán insertar una URL de YouTube o Vimeo que se mostrará como una imagen en miniatura (con el botón &quot;reproducir&quot;) dentro del correo electrónico. Puede especificar una región de vídeo mediante un `<div>` con class=&quot;mktoVideo&quot;

Atributos requeridos

* **id:** Cadena de ID. Contiene sólo letras, números, guión &quot;-&quot; y guión bajo &quot;_&quot;. No se permiten espacios. Debe ser único.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoImgClass:** Cadena. El valor aquí se agregará al atributo de clase de la miniatura de vídeo `<img>` dentro del div.

Ejemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Las variables son como tokens. Primero debe definirlos dentro de la variable `<head>` sección de la plantilla de correo electrónico que utiliza `<meta>` y, a continuación, utilícelas todas las veces que desee en toda la plantilla. Como están definidos en la plantilla, el usuario final puede modificar sus valores según sus reglas. Tenga en cuenta que puede definir una variable como local o global en el ámbito. Si utiliza una variable dentro de un &quot;módulo&quot; (consulte a continuación) y un usuario final duplica ese módulo, las variables locales tendrán valores independientes, mientras que las variables globales se aplicarán a ambos módulos.

## Cadena {#string}

Si especifica una variable como String, el usuario final podrá introducir texto dentro de un cuadro de texto en el editor de correo electrónico. Especifique una variable de cadena mediante `<meta>` con class=&quot;mktoString&quot;

Atributos requeridos

* **id:** Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **allowHTML:** Booleano. Controla si el valor de la variable se escapa al HTML. Si se omite, el valor predeterminado es False.
* **default**: Valor predeterminado de la cadena. En blanco si se omite.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Si especifica una variable como Lista, el usuario final podrá elegir entre un conjunto de valores definidos en el editor de correo electrónico. Especifique una variable de lista mediante `<meta>` con class=&quot;mktoList&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName:** Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.
* **valores:** Lista de valores separados por comas. Debe tener al menos una cadena.

Atributos opcionales

* **predeterminado:** Valor predeterminado de la lista desplegable de selección. Si se omite, se utiliza el primer valor del atributo &quot;values&quot;.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Si especifica una variable como Number, el usuario final podrá introducir un número en el editor de correo electrónico. Especifique una variable Number usando `<meta>` con class=&quot;mktoNumber&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.
* **predeterminado:** Valor numérico predeterminado para la variable .

Atributos opcionales

* **min:** Valor mínimo aceptado.
* **max:** Valor máximo aceptado.
* **unidades:** Unidades que se anexarán al valor numérico (por ejemplo: px, pt, em, etc.) cuando se muestra en el Editor de correo electrónico, así como en el código resultante.
* **paso:** Cuántas unidades debe aumentar/disminuir la variable numérica (0.1, 1, 10, etc.). Si se omite, el valor predeterminado es 1.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Color {#color}

Si especifica una variable como Color, el usuario final podrá introducir un valor de color hexadecimal o elegir un color del selector de color dentro del editor de correo electrónico. Especifique una variable de color mediante `<meta>` con class=&quot;mktoColor&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:** Valor predeterminado del color. Código de color hexadecimal de 6 dígitos. Ejemplo: #ffff.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Si especifica una variable como booleana, el usuario final podrá activar o desactivar la opción en el editor de correo electrónico. Especifique una variable booleana mediante `<meta>` con class=&quot;mktoBoolean&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:** Valor booleano que determina el estado predeterminado del conmutador. False si se omite.
* **false_value:** Valor que debe insertarse cuando la opción de alternancia está en la posición OFF. False si se omite.
* **true_value:** Valor que se debe insertar cuando la opción está en la posición ON. True si se omite.
* **false_value_name:** La IU se muestra en la opción cuando está en la posición OFF. False si se omite.
* **true_value_name:** La IU se muestra en la opción cuando está en la posición ON. True si se omite.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloque de HTML {#html-block}

Si especifica una variable como bloque de HTML, el usuario final podrá introducir un HTML de comentarios desde el editor de correo electrónico. Especifique una variable Bloque de HTML usando `<meta>` con class=&quot;mktoHTML&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:** Valor codificado del HTML para que sirva como contenido predeterminado del bloque.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable de imagen {#image-variable}

Si especifica una variable como imagen, el usuario final podrá elegir una imagen del selector de imágenes dentro del editor de correo electrónico. La URL de imagen seleccionada será el valor de la variable . Especifique una variable de imagen mediante `<meta>` con class=&quot;mktoImg&quot;

Atributos requeridos

* **id**: Cómo se hace referencia a la variable dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **predeterminado:** URL de imagen predeterminada para el elemento.
* **mktoModuleScope**: Booleano. Controla si la variable es local (true) o global (false) cuando se utiliza en un módulo. Si se omite, el valor predeterminado es False.

Ejemplo de declaración:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Ejemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Los módulos son secciones con plantillas definidas en el nivel de plantilla que aparecerán para que los usuarios finales las inserten en su correo electrónico. Como ya ha creado previamente estos módulos, puede asegurarse de que interactúen con el resto del contenido del correo electrónico correctamente (de forma totalmente adaptable). Solo puede colocar un módulo en un contenedor.

>[!IMPORTANT]
>
>Cuando se genera un correo electrónico a partir de una plantilla de correo electrónico que contiene componentes de módulo definidos, cualquier cambio realizado en los módulos de la plantilla **not** se insertará en dicho correo electrónico.

**Para contenedores de tipo `<table>`, `<tbody>`, `<thead>`o `<tfoot>`:**

Especificado con `<tr>` con class=&quot;mktoModule&quot;

**Para contenedores de tipo `<td>`:**

Especificado con `<table>` con class=&quot;mktoModule&quot;

Atributos requeridos

* **id**: Cómo se hace referencia al módulo dentro de la plantilla de correo electrónico.
* **mktoName**: Cadena. Este es el nombre para mostrar que se mostrará en el Editor de correo electrónico 2.0. Se recomienda utilizar un nombre descriptivo.

Atributos opcionales

* **mktoActive:** Determina si este módulo aparece en la lista de módulos dentro del editor de correo electrónico. El valor predeterminado es true. Si es false, un usuario final no puede agregar el módulo a un correo electrónico.
* **mktoAddByDefault:** Determina si este módulo estará en el lienzo de un nuevo correo electrónico que utiliza esta plantilla al crearlo. El valor predeterminado es true (si mktoActive es false, se ignora este valor).

>[!NOTE]
>
>Los valores de clase que contienen sintaxis Marketo (por ejemplo, mktoModule, mktoContainer, mktoText) distinguen entre mayúsculas y minúsculas. Los nombres de atributos personalizados (es decir, mktoimgwidth, mktoname) no lo son.

## Contenedores {#containers}

Un contenedor contiene módulos y define dónde se pueden colocar. Cuando los usuarios finales vuelven a ordenar e insertan módulos en su correo electrónico, el contenedor controla adónde pueden ir.

**Especificado mediante `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=&quot;mktoContainer&quot;**

Atributos requeridos

**id**: Cómo se hace referencia al módulo dentro de la plantilla de correo electrónico.

>[!CAUTION]
>
>Los contenedores solo pueden contener módulos. Si hay algo más, ¡el contenedor se considera no válido! Solo se permite un contenedor por plantilla.
