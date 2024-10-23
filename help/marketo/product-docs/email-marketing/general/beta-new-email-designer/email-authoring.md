---
description: 'Creación de correos electrónicos: documentos de Marketo, documentación del producto'
title: Creación de correo electrónico
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 22f667b27168eafe51df75f81be74e18f5497c3f
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 1%

---

# Creación de correo electrónico {#email-authoring}

Obtenga información sobre cómo crear, personalizar y previsualizar correos electrónicos en el nuevo Designer de correo electrónico del Marketo Engage.

>[!IMPORTANT]
>
>Este artículo es solo para miembros de la versión beta de New Marketo Engage Email Designer. Por favor, no disemine.

## Crear un correo electrónico {#create-an-email}

1. Inicie sesión en el Marketo Engage a través de [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. En Mi Marketo, seleccione **Design Studio**.

   ![](assets/create-an-email-1.png)

1. En el árbol, seleccione **Correos electrónicos (nuevo editor)**.

   ![](assets/create-an-email-2.png)

1. Haga clic en el botón **Crear correo electrónico**.

   ![](assets/create-an-email-3.png)

1. Introduzca un nombre de correo electrónico y una línea de asunto. Haga clic en **Crear**.

   ![](assets/create-an-email-4.png)

Eso es todo. Ahora es el momento de diseñar su correo electrónico.

## Elija su tipo de contenido {#choose-your-content-type}

1. En el correo electrónico que acaba de crear, haga clic en **Agregar contenido de correo electrónico**.

   ![](assets/choose-your-content-type-1.png)

1. Se carga la página _Crear tu correo electrónico_. Puede elegir entre algunas opciones:

* [Diseñe desde cero](#design-from-scratch) con el editor de correo electrónico visual

* [Importe su propio HTML](#import-html) a través de un HTML o archivo zip

* [Seleccione una plantilla existente](#choose-a-template) (una de nuestras muestras o una que ya haya guardado)

### Diseñe desde cero {#design-from-scratch}

Cuando comience desde cero en el editor de correo electrónico, utilice las opciones siguientes para definir el contenido.

1. En la página _Crear tu correo electrónico_, selecciona **Diseñar desde cero**.

1. Agregue [estructura y contenido](#add-structure-and-content) a su correo electrónico.

1. Agregar [imágenes](#add-assets).

1. [Personaliza](#personalize-content) tu contenido.

1. Revisar vínculos y [editar seguimiento](#edit-url-tracking).

### Importar HTML {#import-html}

Puede importar contenido existente del HTML para diseñar el correo electrónico. El contenido puede ser:

* Archivo de HTML con una hoja de estilos incorporada

* Archivo .zip que incluye un archivo de HTML, la hoja de estilos (.css) y las imágenes

>[!NOTE]
>
>No hay restricciones en la estructura de archivos .zip. Sin embargo, las referencias deben ser relativas y ajustarse a la estructura de árbol de la carpeta .zip.

1. En la página Diseñar su plantilla, seleccione **HTML de importación**.

1. Arrastre y suelte el HTML o archivo .zip deseado (o seleccione un archivo del equipo) y haga clic en **Importar**.

   ![](assets/authoring-import-your-html-1.png)

>[!NOTE]
>
>Cuando se carga el contenido del HTML, el contenido se encuentra en modo de compatibilidad. En este modo, solo puede personalizar el texto, agregar vínculos o agregar recursos al contenido.

Puede realizar los cambios que desee en el contenido importado con [las herramientas visuales del editor de correo electrónico](#add-structure-and-content).

### Elija una plantilla {#choose-a-template}

Existen dos tipos de plantillas para elegir.

* **Plantillas de ejemplo**: El Marketo Engage ofrece cuatro plantillas de correo electrónico predeterminadas.

* **Plantillas guardadas**: son plantillas que creó desde cero mediante el menú Plantillas o un mensaje de correo electrónico que creó y eligió guardar como plantilla.

>[!BEGINTABS]

>[!TAB Plantillas de muestra]

Elija una de las plantillas listas para usar para empezar con su diseño de plantillas de correo electrónico.

1. La pestaña Plantillas de muestra está abierta de forma predeterminada.

1. Seleccione la plantilla que desee utilizar.

   ![](assets/authoring-sample-templates-1.png)

1. Haga clic en **Usar esta plantilla**.

   ![](assets/authoring-sample-templates-2.png)

1. Edite el contenido como desee con el diseñador de contenido visual.

>[!TAB Plantillas guardadas]

1. Haga clic en la ficha **Plantillas guardadas** y seleccione la plantilla que desee.

   ![](assets/authoring-saved-templates-1.png)

1. Haga clic en **Usar esta plantilla**.

   ![](assets/authoring-saved-templates-2.png)

1. Edite el contenido como desee con el diseñador de contenido visual.

>[!ENDTABS]

## Añadir estructura y contenido {#add-structure-and-content}

1. Para empezar a crear o modificar contenido, arrastre y suelte un elemento de Estructuras en el lienzo. Edite su configuración en el panel de la derecha.

   >[!TIP]
   >
   >Seleccione el componente de columna n:n para definir el número de columnas que desea (entre tres y 10). También puede definir el ancho de cada columna moviendo las flechas debajo de la columna.

   ![](assets/authoring-add-structure-and-content-1.png)

   >[!NOTE]
   >
   >Cada tamaño de columna no puede ser inferior al 10 % de la anchura total del componente de estructura. Solo se pueden eliminar columnas vacías.

1. En la sección Contenido, arrastre sobre los elementos deseados y suéltelos en uno o más componentes de estructura.

   ![](assets/authoring-add-structure-and-content-2.png)

1. Cada componente se puede personalizar mediante las pestañas Settings o Style. Cambie la fuente, el estilo del texto, el margen, etc.

### Añadir Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY? - For now, only from Marketo Images and Files section!!!
```

1. Para acceder a sus imágenes, haga clic en el icono Selector de recursos.

   CAPTURA DE PANTALLA

1. Arrastre y suelte la imagen deseada en un componente de estructura.

   CAPTURA DE PANTALLA

   >[!NOTE]
   >
   >Para reemplazar una imagen existente, selecciónela y haga clic en **Seleccionar un recurso** en la pestaña Configuración a la derecha.

Haga clic en Habilitar contenido de condición para añadir contenido dinámico y adaptar el contenido a los perfiles de destino según las reglas condicionales.



Si es necesario, puede personalizar aún más el correo electrónico haciendo clic en Cambiar al editor de código desde el menú avanzado. Esto le permite editar el código fuente del correo electrónico, por ejemplo para añadir etiquetas de seguimiento o de HTML personalizadas.

PRECAUCIÓN
No puede volver al diseñador visual para este correo electrónico después de cambiar al editor de código.

Una vez que el contenido esté listo, haga clic en el botón Simular contenido para comprobar la renderización. Puede elegir la vista de escritorio o la vista móvil.

Cuando esté listo, haga clic en Guardar

### Capas, configuración y estilos {#layers-settings-styles}

Abra el árbol de navegación para acceder a estructuras específicas y a sus columnas/componentes para una edición más granular. Para acceder a, haga clic en el icono del árbol de navegación.

![](assets/authoring-layers-settings-styles-1.png)

En el ejemplo siguiente se describen los pasos para ajustar el relleno y la alineación vertical dentro de un componente de estructura compuesto por columnas.

1. Seleccione la columna en el componente de estructura directamente en el lienzo o mediante el _árbol de navegación_ que se muestra a la izquierda.

1. En la barra de herramientas de la columna, haga clic en la herramienta _[!UICONTROL Seleccionar una columna]_ y elija la que desee editar.

   También puede seleccionarlo en el árbol de estructura. Los parámetros editables de esa columna se muestran en las fichas _[!UICONTROL Configuración]_ y _[!UICONTROL Estilos]_ de la derecha.

   ![](assets/authoring-layers-settings-styles-2.png)

1. Para editar las propiedades de la columna, haga clic en la ficha _[!UICONTROL Estilos]_ de la derecha y cámbielas según sus necesidades:

   * Para **[!UICONTROL Background]**, cambie el color de fondo según sea necesario.

     Desactive la casilla de verificación para un fondo transparente. Habilite la configuración de **[!UICONTROL imagen de fondo]** para usar una imagen como fondo en lugar de un color sólido.

   * Para **[!UICONTROL Alignment]**, selecciona el icono _Top_, _Middle_ o _Bottom_.
   * Para **[!UICONTROL Padding]**, defina el relleno para todos los lados.

     Seleccione **[!UICONTROL relleno diferente para cada lado]** si desea ajustar el relleno. Haga clic en el icono _Bloquear_ para interrumpir la sincronización.

   * Expanda la sección **[!UICONTROL Avanzado]** para definir estilos en línea para la columna.

   ![](assets/authoring-layers-settings-styles-3.png)

1. Repita estos pasos según sea necesario para ajustar la alineación y el relleno de las demás columnas del componente.

1. Guarde los cambios.

### Personalizar contenido {#personalize-content}

Los tokens funcionan en el nuevo editor del mismo modo que en el antiguo, pero el icono tiene un aspecto diferente. El ejemplo siguiente describe cómo agregar un token de nombre con texto de reserva.

1. Seleccione el componente de texto. Coloque el cursor donde desee que aparezca el token y haga clic en el icono **Agregar personalización**.

   ![](assets/authoring-personalize-content-1.png)

1. Haga clic en el [tipo de token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} deseado.

   ![](assets/authoring-personalize-content-2.png)

1. Busque el token deseado y haga clic en el icono **...** (al hacer clic en el icono + se agrega un token sin texto de reserva).

   ![](assets/authoring-personalize-content-3.png)

   >[!NOTE]
   >
   >&quot;Texto de reserva&quot; es el nuevo término del editor para el valor predeterminado. Ejemplo: ``{{lead.First Name:default=Friend}}``. Se recomienda en caso de que no haya ningún valor para la persona en el campo que elija.

1. Establece el texto de reserva y haz clic en **Agregar**.

   ![](assets/authoring-personalize-content-4.png)

1. Haga clic en **Guardar**.

### Editar seguimiento de URL {#edit-url-tracking}

A veces no se desea habilitar la URL de seguimiento de Marketo en un vínculo de un mensaje de correo electrónico. Esto resulta útil cuando la página de destino no admite parámetros de URL y puede provocar que se rompa un vínculo.

1. Haga clic en el icono Links para mostrar todas las direcciones URL del correo electrónico.

   ![](assets/authoring-edit-url-tracking-1.png)

1. Haga clic en el icono de lápiz para editar el seguimiento de cualquier vínculo deseado.

1. Haga clic en el menú desplegable **Tipo de seguimiento** y realice la selección.

   ![](assets/authoring-edit-url-tracking-2.png)

   <table><tbody>
     <tr>
       <td><b>Seguimiento sin mkt_tok</b></td>
       <td>Activa el seguimiento en la dirección URL sin usar el parámetro de cadena de consulta mkt_tok en la dirección URL de destino</td>
     </tr>
     <tr>
       <td><b>Seguimiento con mkt_tok</b></td>
       <td>Activa el seguimiento en la URL con el uso del parámetro de cadena de consulta mkt_tok en la URL de destino</td>
     </tr>
     <tr>
       <td><b>No rastrear</b></td>
       <td>Deshabilita el seguimiento de la dirección URL</td>
     </tr>
   </tbody>
   </table>

1. De forma opcional, puede asignar una etiqueta a la dirección URL o agregar etiquetas.

1. Haga clic en **Guardar** cuando termine.

## Comprobar alertas {#check-alerts}

A medida que diseña el contenido, las alertas se muestran en la parte superior derecha de la pantalla cuando falta la configuración clave.

Existen dos tipos de alertas:

**Advertencias**

Las advertencias hacen referencia a recomendaciones y prácticas recomendadas, como:

* **El vínculo de no participación no está presente en el cuerpo del correo electrónico**: aunque los vínculos de cancelación de suscripción son un requisito, se recomienda agregarlos al cuerpo del correo electrónico.

>[!NOTE]
>
>No es necesario agregar una opción de cancelación de suscripción para [Correos electrónicos operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (que no sean de marketing).

* **La versión de texto del HTML está vacía**: debe definir una versión de texto del cuerpo del correo electrónico para los casos en los que no se pueda mostrar el contenido del HTML.

* **El vínculo vacío está presente en el cuerpo del correo electrónico**: compruebe que todos los vínculos del correo electrónico sean correctos.

* **El tamaño del correo electrónico ha superado el límite de 100 KB**: para una entrega óptima, asegúrese de que el tamaño del correo electrónico no supere los 100 KB.

**Errores**

Los errores impiden enviar o probar el correo electrónico hasta que se resuelvan:

* **Falta la línea de asunto**: se requiere una línea de asunto de correo electrónico.

* **La versión de correo electrónico del mensaje está vacía**: este error se produce cuando no se ha configurado el contenido del correo electrónico.

## Prueba del correo electrónico {#test-your-email}

Cuando se define el contenido del mensaje, puede utilizar perfiles de prueba para previsualizarlo, enviar pruebas y controlar cómo se procesa en clientes populares de escritorio, móviles y basados en web. Si ha insertado contenido personalizado, puede comprobar cómo se muestra en el mensaje mediante los datos del perfil de prueba.

Para obtener una vista previa del contenido del correo electrónico, haga clic en **Simular contenido** y, a continuación, agregue un perfil de prueba para comprobar el mensaje mediante los datos del perfil de prueba.

![](assets/test-your-email-1.png)

## Referencia a un correo electrónico {#reference-an-email}

Después de crear un correo electrónico en el nuevo editor, puede hacer referencia a él en campañas inteligentes o listas inteligentes como lo haría con cualquier otro correo electrónico.

* Haga referencia a él en una lista inteligente al [seguir los pasos habituales](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Haga referencia a él en una campaña inteligente al [seguir los pasos habituales](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Solo se puede hacer referencia a los correos electrónicos guardados. No hay estado &quot;aprobado&quot; en el nuevo diseñador de correo electrónico.

>[!MORELIKETHIS]
>
>[Plantillas de correo electrónico](/help/marketo/product-docs/email-marketing/general/beta-new-email-designer/email-templates.md){target="_blank"}: Aprenda a crear, diseñar y obtener acceso a una plantilla de correo electrónico en el nuevo diseñador.
