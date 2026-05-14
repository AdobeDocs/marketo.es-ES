---
solution: Marketo Engage
product: marketo
title: Fragmentos personalizables
description: Aprenda a personalizar fragmentos haciendo que algunos campos sean editables. Cree fragmentos reutilizables flexibles en el Designer de correo electrónico.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1403
ht-degree: 0%

---

# Fragmentos personalizables {#customizable-fragments}

Cuando los fragmentos se utilizan en una plantilla de correo electrónico o de correo electrónico, están bloqueados de forma predeterminada debido a la herencia, lo que significa que los cambios realizados en un fragmento se propagan automáticamente a todos los recursos donde se utiliza. Con los fragmentos personalizables, los campos específicos de un fragmento se pueden definir como editables cuando el fragmento se agrega a un correo electrónico o a una plantilla de correo electrónico. Por ejemplo, si tiene un fragmento con un titular, texto y un botón, puede designar ciertos campos, como la imagen o la dirección URL de destino del botón, como editables.

Los fragmentos personalizables le permiten administrar y personalizar el contenido sin crear bloques de contenido completamente nuevos ni interrumpir la herencia de fragmentos. Los cambios realizados en el nivel de fragmento se siguen propagando, pero permiten la personalización en el nivel de correo electrónico o de plantilla de correo electrónico.

Los fragmentos visuales y de expresión se pueden marcar como personalizables.

## Agregar campos editables en fragmentos visuales {#visual}

Para poder editar partes de un fragmento visual, siga estos pasos:

>[!NOTE]
>
>Los campos editables se pueden agregar a los componentes **image**, **text** y **button**. Para los componentes de **HTML**, se agregan campos editables mediante el editor de personalización, de forma similar a los fragmentos de expresiones. [Obtenga información acerca de campos editables en componentes de HTML en fragmentos](#editable-html)

1. Abra la pantalla de edición de contenido del fragmento.

1. Seleccione el componente del fragmento en el que desea configurar los campos editables.

1. El panel de propiedades del componente se abre en el lado derecho. Seleccione la pestaña **[!UICONTROL Campos editables]** y luego cambie la opción **[!UICONTROL Habilitar edición]**.

1. Todos los campos que se pueden editar para el componente seleccionado se muestran en el panel. Los campos disponibles para editar dependen del tipo de componente seleccionado.

   En el ejemplo siguiente, la dirección URL del botón &quot;Haga clic aquí&quot; está configurada como editable.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Haga clic en **[!UICONTROL Información general]** para comprobar todos los campos editables y sus valores predeterminados.

   En este ejemplo, el campo URL del botón se muestra con el valor predeterminado definido en el componente. Los usuarios pueden personalizar este valor después de agregar el fragmento a su contenido.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Guarde los cambios cuando haya terminado.

Después de agregar el fragmento a un correo electrónico, los usuarios pueden personalizar todos los campos editables configurados en el fragmento.

## Componentes editables de HTML en fragmentos {#editable-html}

Dentro de un componente de HTML, los siguientes tipos de elementos se pueden convertir en editables:

* Parte de **contenido de texto** (por ejemplo, un titular o una etiqueta de CTA).
* Una **URL** completa que se usa como destino de vínculo o como origen de imagen. No se admiten direcciones URL parciales; la variable debe representar el valor de dirección URL completo.
* Un **valor de propiedad CSS** completo (por ejemplo, un valor de color completo, un valor de relleno completo o un valor de ancho completo). No se admiten valores de propiedad CSS parciales.

Cada valor de propiedad de CSS parametrizado debe ser exactamente `{{{varName}}}`: sin sufijos, sin texto adicional, sin múltiples variables y sin concatenación dentro de una sola propiedad.

Para parametrizar propiedades de varios lados, como el relleno, haga lo siguiente:

* declarar cada lado como una propiedad independiente _(recomendado)_, o
* declare una sola variable que contenga el valor abreviado completo.

## Funcionamiento de los campos editables en los componentes de HTML {#components}

Los campos editables de un componente de HTML se crean declarando variables en línea directamente dentro del código fuente del componente. Cada variable tiene un ID único y un valor predeterminado. A continuación, se hace referencia a la variable siempre que el valor editable deba aparecer en el marcado.

Una vez guardado y publicado el fragmento, cada variable declarada en el componente HTML aparece automáticamente como un parámetro editable cuando se agrega el fragmento a un correo electrónico.

El autor del correo electrónico puede anular el valor predeterminado de cualquier variable de la Designer de correo electrónico (por ejemplo, cambiar un color de fondo, intercambiar una URL de CTA o actualizar un titular) sin modificar la HTML subyacente.

## Referencia de sintaxis {#syntax}

Los campos editables se definen y se hace referencia a ellos mediante dos patrones:

### Declarar una variable {#declaring}

Utilice la declaración en línea para definir una variable con un ID único y un valor predeterminado:

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

Reemplace `variableID` con un identificador único para el campo editable. El ID debe ser único dentro del componente y no debe contener espacios.

Reemplace `default_value` con el valor que debería usarse si el autor del correo electrónico no lo anula.

### Referencia a una variable {#referencing}

Utilice llaves triples para hacer referencia a la variable dondequiera que su valor deba aparecer en el marcado:

```handlebars
{{{variableID}}}
```

Se puede hacer referencia al mismo ID de variable cualquier número de veces dentro de HTML. Todas las referencias se resolverán con el valor que establezca el autor del correo electrónico (o con el valor predeterminado si no se proporciona ninguna anulación).

### Parámetros opcionales {#optional}

La declaración en línea admite parámetros opcionales que cambian la forma en que se presenta o procesa el campo editable:

| Acción | Parámetro | Ejemplo |
|---|---|---|
| Declarar un campo editable con un **valor predeterminado**. Cuando se agrega el fragmento a un correo electrónico, se utiliza este valor predeterminado a menos que el autor lo anule. | Agregue el valor predeterminado entre las etiquetas en línea. | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| Defina una **etiqueta** para el campo editable. Esta etiqueta se muestra en el Designer de correo electrónico cuando el autor del correo electrónico edita los campos del fragmento. | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| Declarar un campo editable que contenga **origen de imagen**. | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| Declare un campo editable que contenga una **URL** de la que deba realizarse un seguimiento. | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## Añadir campos editables a un componente de HTML {#adding-editable-fields}

Para poder editar partes de un componente de HTML dentro de un fragmento visual, siga estos pasos:

1. Abra el fragmento visual para editarlo en el Designer de correo electrónico.
1. Agregue un **componente HTML** al fragmento desde el panel Componentes o seleccione un componente HTML existente.
1. Con el componente HTML seleccionado, haga clic en **Mostrar código fuente** para abrir la vista de código fuente de HTML en el editor de personalización.
1. En el editor de personalización, declare cada variable editable con la sintaxis de declaración en línea. Coloque todas las declaraciones de variables en la parte superior del componente para facilitar la lectura y asigne a cada variable un ID único.
1. Haga referencia a cada variable en el marcado de HTML usando la sintaxis `{{{variableID}}}` siempre que aparezca el valor editable. Se puede hacer referencia a la misma variable varias veces en el mismo componente.
1. Guarde el componente HTML y, a continuación, guarde el fragmento.
1. Publique el fragmento para que esté disponible para su uso en correos electrónicos.

## Uso del fragmento en un correo electrónico {#using-fragment}

Una vez publicado el fragmento, todas las variables declaradas en sus componentes de HTML aparecen como parámetros editables en el Designer de correo electrónico.

Para personalizarlos al utilizar el fragmento en un correo electrónico:

1. Abra o cree un correo electrónico en Marketo Engage Email Designer.
1. Añada el fragmento publicado al lienzo del correo electrónico.
1. Seleccione el fragmento para abrir su panel de propiedades. La lista de campos editables se muestra en la sección **Campos editables**, con cada campo etiquetado por su ID de variable (o por la etiqueta descriptiva especificada a través del parámetro `name`).
1. Actualice el valor de cualquier campo editable directamente desde el panel de propiedades. El cambio solo se aplica al correo electrónico actual; el fragmento publicado y otros correos electrónicos que hacen referencia a él no se ven afectados.
1. Guarde el correo electrónico.

El fragmento se procesa con los valores personalizados, al tiempo que hereda las futuras actualizaciones estructurales realizadas en el fragmento publicado.

### Ejemplo: fragmento simple con texto, color y dirección URL editables {#example}

En el siguiente ejemplo se crea un pequeño titular promocional con cuatro campos editables:

* un color de fondo
* un texto de titular
* una etiqueta de CTA
* una URL de CTA

Después de publicar el fragmento, un autor de correo electrónico puede anular cualquiera de estos valores al añadir el fragmento a un correo electrónico.

**Titular editable simple**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

En este ejemplo:

* Se hace referencia a `bgColor` dos veces: una vez para el color de fondo de tabla y otra para el color de texto de CTA. Ambas referencias se resuelven en el mismo valor, por lo que una sola edición se propaga a ambas ubicaciones.
* `ctaUrl` se declaró con `assetType="url"`, lo que indica que el valor debe procesarse como una dirección URL rastreada.

## Prácticas recomendadas {#best-practices}

* Incluya unidades (`px`, `em`, `%`) dentro del valor predeterminado de la variable para que la variable represente un valor CSS completo. Esto evita la concatenación, que no es compatible.
* Prefiera las propiedades CSS de longitud por lado (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) en lugar de las de abreviatura cuando sea necesario editar cada lado de forma independiente.
* Cuando sea necesario rastrear una dirección URL, declárela con `assetType="url"`.
* Cuando un campo editable lleva un origen de imagen, declárelo con `assetType="image"`.
* Pruebe el fragmento agregándolo a un correo electrónico de borrador y comprobando que todos los campos editables aparecen en el panel de propiedades y se resuelven correctamente cuando se anulan.

## Cosas que hay que saber {#things-to-know}

* Los campos editables de los componentes de HTML admiten contenido de texto completo, direcciones URL completas y valores de propiedad CSS completos. Las direcciones URL parciales y los valores de propiedad CSS parciales no se pueden parametrizar.
* Un solo valor de propiedad CSS no puede combinar una variable con texto estático adicional o con otra variable. Cada valor de propiedad parametrizado debe ser exactamente una referencia de variable.
* Los ID de variable deben ser únicos dentro de un componente de HTML y no deben contener espacios.
* Los vínculos de sistema listos para usar, como el vínculo de cancelación de suscripción y la URL de la página espejo, no se pueden convertir en campos editables.

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[Fragmentos](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
