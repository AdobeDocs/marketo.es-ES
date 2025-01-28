---
title: Fragmentos
description: Aprenda a crear y utilizar fragmentos de contenido visual como componentes reutilizables para correos electrónicos y plantillas de correo electrónico.
hide: true
hidefromtoc: true
source-git-commit: 32aff679ec2de3f4ff93f89ac298b1fec3cb9792
workflow-type: tm+mt
source-wordcount: '2429'
ht-degree: 3%

---

# Fragmentos

Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos y plantillas de correo electrónico. Normalmente es un bloque de contenido (texto, imagen o ambos) que se puede crear e insertar rápidamente en el proyecto. Con esta funcionalidad, puede generar varios bloques de contenido personalizados para que los utilicen los integrantes del equipo de marketing a fin de combinar el contenido del correo electrónico para mejorar el proceso de diseño. Los casos de uso comunes incluyen bloques de contenido de encabezado/pie de página para correo electrónico, titulares de invitaciones a eventos, mensajes de temporada y mucho más.

Para aprovechar al máximo los fragmentos de sus flujos de trabajo:

* _Cree sus propios fragmentos_: cree fragmentos visuales desde cero o guarde contenido como un fragmento desde el editor de contenido visual.
* _Reutilizar fragmentos_: utilícelos tantas veces como sea necesario en el contenido.

## Fragmentos visuales {#visual-fragments}

Los fragmentos visuales son bloques visuales predefinidos creados con el editor de contenido visual que se pueden reutilizar en varios correos electrónicos o plantillas de correo electrónico.

## Acceso y administración de fragmentos {#access-and-manage-fragments}

Para acceder a los fragmentos visuales, vaya a la navegación izquierda y haga clic en **[!UICONTROL Administración de contenido]** > **[!UICONTROL Fragmentos]**. Esta acción abre una página de lista con todos los fragmentos creados en la instancia enumerados en una tabla.

CAPTURA DE PANTALLA

La tabla está ordenada por la columna _[!UICONTROL Modificado]_, con los fragmentos actualizados más recientemente en la parte superior de forma predeterminada. Haga clic en el título de la columna para cambiar entre ascendente y descendente.

### Estado del fragmento y ciclo vital

El estado del fragmento determina su disponibilidad para utilizarlo en un correo electrónico o plantilla de correo electrónico, y los cambios que puede realizar en él.

<table>
<tbody>
  <tr>
    <td><b>Borrador</b></td>
    <td>Cuando crea un fragmento, está en estado de borrador. Permanece como borrador hasta que se publica para utilizarlo en un correo electrónico o en una plantilla de correo electrónico.
    <p>Acciones disponibles:
    <li>Editar todos los detalles</li>
    <li>Editar en el diseñador visual</li>
    <li>Publicar</li>
    <li>Duplicado</li>
    <li>Eliminar</li>
  </td>
  <tr>
    <td><b>Publicadas</b></td>
    <td>Al publicar un fragmento, pasa a estar disponible para su uso en un correo electrónico o plantilla de correo electrónico. El contenido de fragmento publicado no se puede modificar en el diseñador visual.
    <p>Acciones disponibles:
    <li>Editar descripción</li>
    <li>Añadir a un correo electrónico o plantilla</li>
    <li>Crear versión de borrador</li>
    <li>Duplicado</li>
    <li>Eliminar (si no está en uso)</li>
    </td>
  </tr>
  <tr>
    <td><b>Publicado con borrador</b></td>
    <td>Cuando crea un borrador a partir de un fragmento publicado, la versión publicada permanece disponible para su uso en una plantilla de correo electrónico o correo electrónico, y el contenido del borrador se puede modificar en el diseñador visual. Si publica la versión de borrador, reemplazará la versión publicada actual y el contenido se actualizará en <i>todos</i> los correos electrónicos y las plantillas de correo electrónico en los que esté en uso. 
    <p>Acciones disponibles:
    <li>Editar descripción</li>
    <li>Añadir a un correo electrónico o plantilla</li>
    <li>Editar versión de borrador en el diseñador visual</li>
    <li>Versión de borrador de Publish</li>
    <li>Duplicado</li>
    <li>Eliminar (si no está en uso)</li>
    </td>
  </tr>
</tbody></table>

CAPTURA DE PANTALLA

### Filtrado de la lista de fragmentos {#filter-the-fragments-list}

Utilice la barra de búsqueda para buscar un fragmento por nombre. Haga clic en el icono _Filtro_ ( ![Mostrar u ocultar filtros](assets/icon-filter.svg) ) para mostrar las opciones de filtro disponibles y elegir la configuración que desee.

CAPTURA DE PANTALLA

### Personalización de la visualización de columnas {#customize-the-column-display}

Personalice las columnas que desee mostrar en la tabla haciendo clic en el icono _Personalizar tabla_ ( ![Personalizar icono de tabla](assets/icon-column-settings.svg) ) en la parte superior derecha.

En el cuadro de diálogo, seleccione las columnas que desee y haga clic en **[!UICONTROL Aplicar]**.

CAPTURA DE PANTALLA

## Creación de fragmentos {#create-fragments}

Cree un nuevo fragmento visual haciendo clic en **[!UICONTROL Crear fragmento]** en la parte superior derecha.

1. En el cuadro de diálogo _[!UICONTROL Crear fragmento]_, escriba un **[!UICONTROL Nombre]** y una **[!UICONTROL Descripción]** opcional.

   Requisitos de fragmento:

   * Nombre: máximo de 100 caracteres, debe ser único, sin distinción de mayúsculas y minúsculas
   * Descripción: máximo de 300 caracteres
   * Los caracteres Alpha, numéricos y especiales están bien
   * Los caracteres reservados **_no se permiten_**: `\ / : * ? " < > |`

CAPTURA DE PANTALLA

1. Haga clic en **[!UICONTROL Crear]**.

   El diseñador visual se abre con un lienzo vacío.

1. Utilice las herramientas de diseño de contenido para crear el contenido del fragmento visual:

   * [Añadir estructura y contenido](#add-structure-and-content)
   * [Añadir Assets](#add-assets)
   * [Desplazamiento por las capas, la configuración y los estilos](#navigate-the-layers-settings-and-styles)
   * [Personalizar contenido](#personalize-content)
   * [Editar seguimiento de URL vinculadas](#edit-linked-url-tracking)

1. Haga clic en **[!UICONTROL Guardar]** en cualquier momento para guardar el fragmento de borrador.

1. Cuando esté listo para que el fragmento esté disponible para usarlo en un correo electrónico o plantilla de correo electrónico, haga clic en **[!UICONTROL Publish]**.

### Añadir estructura y contenido {#add-structure-and-content}

>[!CONTEXTUALHELP]
>id="ajo-b2b_structure_components_fragment"
>title="Adición de componentes de estructura"
>abstract="Los componentes de estructura definen el diseño del fragmento. Arrastre y suelte un componente **Estructura** en el lienzo para empezar a diseñar el contenido del fragmento."

>[!CONTEXTUALHELP]
>id="ajo-b2b_content_components_fragment"
>title="Acerca de los componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de un fragmento."

{{$include /help/_includes/content-design-components.md}}

### Añadir recursos

{{$include /help/_includes/content-design-assets.md}}

### Desplazamiento por las capas, la configuración y los estilos

{{$include /help/_includes/content-design-navigation.md}}

### Personalizar contenido

{{$include /help/_includes/content-design-personalization.md}}

### Editar seguimiento de URL vinculadas

{{$include /help/_includes/content-design-links.md}}

## Ver detalles del fragmento {#view-fragment-details}

Haga clic en el nombre de cualquier fragmento de la página de lista para abrir la página de detalles del fragmento. Puede editar el fragmento, cambiarle el nombre o actualizar su descripción. Realice actualizaciones y haga clic fuera del nombre o del campo de descripción para guardar automáticamente los cambios.

>[!NOTE]
>
>Si un fragmento publicado está siendo utilizado por una plantilla de correo electrónico o de correo electrónico, no puede cambiar su nombre ni editar el contenido. Puede crear una versión de borrador si desea realizar cambios en el fragmento.

CAPTURA DE PANTALLA

Haga clic en **[!UICONTROL Editar fragmento]** para abrir el fragmento en el editor de contenido visual.

Salga de la vista en cualquier momento haciendo clic en la flecha _Atrás_ en la parte superior izquierda, que le devuelve a la página de lista _Fragmentos_.

## Ver fragmento utilizado por referencias {#view-fragment-used-by-references}

En la página de detalles del fragmento, haga clic en la ficha **[!UICONTROL Utilizado por]** para ver los detalles de dónde se está utilizando el fragmento en el Marketo Engage.

>[!IMPORTANT]
>
>Un fragmento que esté siendo utilizado actualmente por un correo electrónico o una plantilla de correo electrónico no se puede eliminar.

Las referencias se muestran según la categoría: _Correo electrónico_ o _Plantilla de correo electrónico_. Los correos electrónicos de Journey Optimizer B2B edition están incrustados y creados en recorridos de cuenta, por lo que el recorrido principal del correo electrónico que utiliza el fragmento se muestra en las referencias. &lt;— ¿QUÉ HAY DE ESTA PARTE, NILESH

CAPTURA DE PANTALLA

Haga clic en el vínculo para abrir el correo electrónico o la plantilla de correo electrónico correspondiente donde se utiliza el fragmento.

## Eliminar fragmentos {#delete-fragments}

Debido a que un fragmento que se encuentra actualmente en uso por una plantilla de correo electrónico o de correo electrónico no se puede eliminar, asegúrese de comprobar las referencias de _usado por_ antes de iniciar la eliminación de un fragmento. Además, una eliminación no se puede deshacer, por lo que debe comprobarla antes de iniciar una acción de eliminación.

Puede eliminar un fragmento mediante cualquiera de los siguientes métodos:

* En los detalles del fragmento a la derecha, haga clic en **[!UICONTROL Eliminar]**.
* En la página de lista _[!UICONTROL Fragmentos]_, haga clic en los puntos suspensivos junto al fragmento y elija **[!UICONTROL Eliminar]**.

Esta acción abre un cuadro de diálogo de confirmación. Puede anular el proceso haciendo clic en **[!UICONTROL Cancelar]** o en **[!UICONTROL Eliminar]** para confirmar la eliminación.

CAPTURA DE PANTALLA

## Editar fragmentos

Las ediciones en un fragmento dependen de su estado actual:

* Cuando un fragmento tiene el estado _Borrador_, puede editar cualquiera de sus detalles y el contenido visual.
* Cuando un fragmento tiene el estado _Publicado_, puede editar la descripción del fragmento, pero no el nombre. No puede editar el contenido visual.
* Cuando un fragmento está en _Publicado con estado de borrador_, la edición de los detalles se limita a la descripción. También puede editar el contenido visual de la versión de borrador.

>[!BEGINTABS]

>[!TAB Borrador]

1. En la página de lista _[!UICONTROL Fragmentos]_, haga clic en el nombre del fragmento para abrirlo.

   Se muestra una previsualización del contenido visual, con los detalles del fragmento a la derecha.

1. Realice las ediciones que desee.

CAPTURA DE PANTALLA

1. Para realizar cambios en el contenido en el diseñador visual, haga clic en **[!UICONTROL Editar fragmento]**.

   Utilice las herramientas del diseñador visual según sea necesario:

   * [Añadir estructura y contenido](#add-structure-and-content)
   * [Añadir Assets](#add-assets)
   * [Desplazamiento por las capas, la configuración y los estilos](#navigate-the-layers-settings-and-styles)
   * [Personalizar contenido](#personalize-content)
   * [Editar seguimiento de URL vinculadas](#edit-linked-url-tracking)

   Haga clic en **[!UICONTROL Guardar]** o **[!UICONTROL Guardar y cerrar]** para volver a los detalles del fragmento.

1. Cuando el fragmento cumpla sus criterios y desee que esté disponible para utilizarlo en un correo electrónico o una plantilla de correo electrónico, haga clic en **[!UICONTROL Publish]**.

>[!TAB Publicado]

1. En la página de lista _[!UICONTROL Fragmentos]_, haga clic en el nombre del fragmento para abrirlo.

   Se muestra una previsualización del contenido visual, con los detalles del fragmento a la derecha.

1. Modifique la descripción, si es necesario.

   Para un fragmento publicado, todos los demás detalles no se pueden cambiar.

1. Si desea actualizar el contenido, haga clic en **[!UICONTROL Crear versión de borrador]** en la parte superior derecha.

   Haga clic en **[!UICONTROL Aceptar]** en el cuadro de diálogo para abrir la versión de borrador en el diseñador visual. Puede cambiar el `image source` KG - LINK HERE si es necesario.

CAPTURA DE PANTALLA

Utilice las herramientas del diseñador visual según sea necesario:

* [Añadir estructura y contenido](#add-structure-and-content)
* [Añadir Assets](#add-assets)
* [Desplazamiento por las capas, la configuración y los estilos](#navigate-the-layers-settings-and-styles)
* [Personalizar contenido](#personalize-content)
* [Editar seguimiento de URL vinculadas](#edit-linked-url-tracking)

Haga clic en **[!UICONTROL Guardar]** o **[!UICONTROL Guardar y cerrar]** para volver a los detalles del fragmento.

1. Cuando el fragmento de borrador cumpla los criterios y desee que los cambios estén disponibles para usarlos en un correo electrónico o una plantilla de correo electrónico, haga clic en **[!UICONTROL Publish]**.

   Cuando publica la versión de borrador, reemplaza la versión publicada actual y el contenido se actualiza en los correos electrónicos y las plantillas de correo electrónico donde ya se utiliza.

>[!TAB Publicado con borrador]

Hay dos formas de abrir la versión de borrador para editarla desde la página de listado _[!UICONTROL Fragmentos]_:

* Haga clic en el icono _Más_ (**...**) junto al nombre del fragmento y elija **[!UICONTROL Abrir versión de borrador]**.

CAPTURA DE PANTALLA

* Haga clic en el nombre del fragmento para abrirlo. A continuación, haga clic en **[!UICONTROL Abrir versión de borrador]** en la parte superior derecha.

  Se mostrará una vista previa del contenido visual de la versión de borrador, con los detalles del fragmento a la derecha.

Para actualizar el contenido:

1. Haga clic en **[!UICONTROL Editar fragmento]** en la parte superior derecha. Utilice las herramientas del diseñador visual según sea necesario:

   * [Añadir estructura y contenido](#add-structure-and-content)
   * [Añadir Assets](#add-assets)
   * [Desplazamiento por las capas, la configuración y los estilos](#navigate-the-layers-settings-and-styles)
   * [Personalizar contenido](#personalize-content)
   * [Editar seguimiento de URL vinculadas](#edit-linked-url-tracking)

   Haga clic en **[!UICONTROL Guardar]** o **[!UICONTROL Guardar y cerrar]** para volver a los detalles del fragmento.

1. Cuando el fragmento de borrador cumpla los criterios y desee que los cambios estén disponibles para usarlos en un correo electrónico o una plantilla de correo electrónico, haga clic en **[!UICONTROL Publish]**.

   Cuando publica la versión de borrador, reemplaza la versión publicada actual y el contenido se actualiza en los correos electrónicos y las plantillas de correo electrónico donde ya se utiliza.

>[!ENDTABS]

## Duplicar fragmentos {#duplicate-fragments}

Puede duplicar un fragmento mediante cualquiera de los siguientes métodos:

* En la página de listado de _[!UICONTROL Fragmentos]_, haga clic en el icono _Más_ (**...**) junto al nombre del fragmento y elija **[!UICONTROL Duplicado]**.
* En la parte superior derecha de la página de detalles del fragmento, haga clic en **[!UICONTROL ... Más]** y elige **[!UICONTROL Duplicar]**.

CAPTURA DE PANTALLA

En el cuadro de diálogo, introduzca un nombre único y una descripción opcional. Haga clic en **[!UICONTROL Duplicar]** para completar la acción.

CAPTURA DE PANTALLA

El fragmento duplicado aparecerá en la lista _Fragmentos_.

## Guardar un nuevo fragmento del contenido del correo electrónico o de la plantilla {#save-a-new-fragment-from-email-or-template-content}

Al crear o editar un correo electrónico o una plantilla de correo electrónico en el editor de contenido visual, puede elegir guardar todo o parte del contenido como un fragmento para que esté disponible para reutilizarlo.

1. Para guardar contenido como un fragmento, haga clic en **[!UICONTROL Más]** y elija **[!UICONTROL Guardar como fragmento]**.

1. Seleccione los diferentes elementos que desea incluir en el fragmento.

   Para seleccionar varias estructuras, mantenga pulsado el botón Mayús o Control.

   Solo se pueden seleccionar estructuras adyacentes entre sí y la interfaz no permite seleccionar elementos no adyacentes.

1. Con el contenido seleccionado, haz clic en **[!UICONTROL Crear]** en la parte superior derecha.

1. En el cuadro de diálogo, escriba un nombre y una descripción opcional para el fragmento. Luego haga clic en **[!UICONTROL Crear]**.

   A continuación, el fragmento se mostrará en la página de lista _Fragmentos_ y también estará disponible para su uso en correos electrónicos y plantillas de correo electrónico.

## Añadir fragmentos visuales al contenido del correo electrónico o de la plantilla {#add-visual-fragments-to-your-email-or-template-content}

Los fragmentos están diseñados para su reutilización y puede añadir hasta 30 en un correo electrónico o plantilla de correo electrónico. Los fragmentos se pueden anidar hasta un solo nivel.

>[!BEGINTABS]

>[!TAB Agregar fragmentos a un correo electrónico]

1. Vaya a **[!UICONTROL Recorridos de cuenta]** y abra un recorrido recorrido existente o cree uno nuevo. &lt;— COMPRUEBE ESTO DOS VECES

----------DEJÓ DE EDITAR AQUÍ---------

1. Crear un nodo [_[!UICONTROL Enviar correo electrónico ]_](./email-authoring.md#add-an-email-action-in-an-account-journey).

1. Cree o edite el contenido de [correo electrónico para el nodo](./email-authoring.md#create-the-email-content).

1. Arrastre y suelte un elemento del menú **[!UICONTROL Componentes]** para proporcionar una _estructura_ para el fragmento.

1. Para abrir la lista de fragmentos publicados, haga clic en el icono _Fragmentos_.

   Puede hacer lo siguiente:
   * Ordenar el listado.
   * Examine, busque y filtre la lista.
   * Cambiar entre las vistas de tarjeta (miniatura) y de lista.
   * Actualice la lista para reflejar cualquiera de los fragmentos creados recientemente.

CAPTURA DE PANTALLA

1. Arrastre y suelte cualquier fragmento en el marcador de posición del componente de estructura.

   El editor procesa el fragmento dentro de la sección o el elemento de la estructura de correo electrónico.

El contenido del fragmento se actualiza dinámicamente dentro de la estructura para procesar una representación visual de cómo aparece el contenido en el correo electrónico.

>[!TIP]
>
>Si desea que el fragmento ocupe todo el diseño horizontal del correo electrónico, agregue una estructura de columna [!UICONTROL 1:1] y, a continuación, arrastre y suelte el fragmento en él.

Una vez guardado el correo electrónico, aparecerá en la página de detalles del fragmento cuando la pestaña _[!UICONTROL Utilizado por]_ esté seleccionada. Los fragmentos agregados a un correo electrónico no se pueden editar dentro del correo electrónico o la plantilla: el fragmento de origen publicado define el contenido.

>[!TAB Agregar fragmentos a una plantilla de correo electrónico]

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Administración de contenido]** > **[!UICONTROL Plantillas]**.

1. Cree una nueva plantilla o abra una plantilla de correo electrónico existente y haga clic en **[!UICONTROL Editar plantilla de correo electrónico]**.

1. Arrastre y suelte un elemento del menú **[!UICONTROL Componentes]** para proporcionar una _estructura_ para el fragmento.

1. Para abrir la lista de fragmentos, haga clic en el icono _Fragmentos_.

   Puede hacer lo siguiente:
   * Ordenar el listado.
   * Examine, busque y filtre la lista.
   * Cambiar entre las vistas de tarjeta (miniatura) y de lista.
   * Actualice la lista para reflejar cualquiera de los fragmentos creados recientemente.

CAPTURA DE PANTALLA

1. Arrastre y suelte cualquier fragmento en el marcador de posición del componente de estructura.

   El editor procesa el fragmento dentro de la sección o el elemento de la estructura de la plantilla de correo electrónico.

1. Arrastre y suelte cualquier fragmento en el marcador de posición del componente de estructura.

   El editor procesa el fragmento dentro de la sección o el elemento de la estructura de la plantilla de correo electrónico.

>[!TIP]
>
>Si desea que el fragmento ocupe todo el diseño horizontal de la plantilla de correo electrónico, agregue una estructura de columna _[!UICONTROL 1:1]_ y, a continuación, arrastre y suelte el fragmento en ella.

Una vez guardada la plantilla de correo electrónico, aparece en la página de detalles del fragmento cuando se selecciona la pestaña _[!UICONTROL Utilizado por]_. Los fragmentos agregados a una plantilla de correo electrónico no se pueden editar dentro de la plantilla: el fragmento de origen publicado define el contenido.

>[!ENDTABS]

## Acciones de fragmento durante la creación de correos electrónicos y plantillas

Cuando se agrega un fragmento a un correo electrónico o a una plantilla de correo electrónico, el contenido del fragmento no se puede editar dentro del correo electrónico o la plantilla. Sin embargo, puede aplicar las siguientes acciones:

* **[!UICONTROL Eliminar]**: esta acción elimina el fragmento del contenido actual del correo electrónico o de la plantilla de correo electrónico (el origen del fragmento no se ve afectado).
* **[!UICONTROL Actualizar]**: esta acción actualiza el contenido del fragmento en el correo electrónico o la plantilla de correo electrónico actual. La actualización es útil cuando desea reflejar cualquier edición reciente en el fragmento después de la adición al correo electrónico o a la plantilla de correo electrónico.
* **[!UICONTROL Duplicado]**: esta acción duplica el fragmento dentro del mismo correo electrónico o plantilla de correo electrónico dentro del editor, con las mismas dimensiones y se agrega justo debajo de él.
* **[!UICONTROL Abrir fragmento]**: esta acción abre una nueva pestaña del explorador con la página del editor de fragmentos y los detalles.
* **[!UICONTROL Romper herencia]**: esta acción interrumpe la herencia del fragmento (y sus cambios) del origen. Utilice esta acción para que el contenido del fragmento esté disponible como contenido independiente y editable dentro del correo electrónico o la plantilla de correo electrónico. Esta acción también quita el correo electrónico o la plantilla de correo electrónico de la referencia _Utilizada por_ para el fragmento original.

Al seleccionar el fragmento en la página del editor, estas acciones están disponibles en la barra de herramientas contextual y en el panel de propiedades de la derecha.

CAPTURA DE PANTALLA
