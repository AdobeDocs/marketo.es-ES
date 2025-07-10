---
solution: Marketo Engage
product: marketo
title: Componentes de contenido
description: DESCRIPCIÓN.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: ca8644c43cfbdbaf7be9f21c5e440949b796cfdb
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Componentes de contenido {#content-components}

Al crear el contenido del correo electrónico, **[!UICONTROL los componentes de contenido]** le permiten personalizar aún más el correo electrónico con componentes sin procesar que puede editar una vez colocados en un correo electrónico.

Puede añadir tantos componentes de contenido como necesite dentro de uno o más componentes de estructura, que definen el diseño del correo electrónico.

## Añadir componentes de contenido {#add-content-components}

Para añadir componentes de contenido al correo electrónico y ajustarlos a sus necesidades, siga los pasos a continuación.

1. En el Designer de correo electrónico, usa un contenido existente o arrastra y suelta **[!UICONTROL Componentes de estructura]** en el contenido vacío para definir el diseño del correo electrónico. `[Learn how](content-from-scratch.md)`

1. Para acceder a la sección **[!UICONTROL Componentes de contenido]**, seleccione el botón correspondiente en el panel izquierdo de Designer de correo electrónico.

   CAPTURA DE PANTALLA

1. Arrastre y suelte los componentes de contenido que desee dentro de los componentes de estructura relevantes.

   CAPTURA DE PANTALLA

   >[!NOTE]
   >
   >Puede añadir varios componentes en un solo componente de estructura y en cada columna de un componente de estructura.

1. Ajuste los atributos y el estilo de cada componente mediante las fichas **[!UICONTROL Configuración]** y **[!UICONTROL Estilo]** de la derecha. Por ejemplo, puede cambiar el estilo del texto, el relleno o el margen de cada componente. `[Learn more about alignment and padding](alignment-and-padding.md)`

   CAPTURA DE PANTALLA

1. Desde el menú avanzado de su **[!UICONTROL componente de contenido]**, puede eliminar o duplicar fácilmente cualquier componente de contenido según sea necesario.

   CAPTURA DE PANTALLA

## Contenedor {#container}

Para aplicar un estilo específico a un grupo de componentes de contenido, puede agregar un componente **[!UICONTROL Contenedor]** y, a continuación, agregar los componentes de contenido que desee dentro de él. Esto permite aplicar un estilo distinto al contenedor, que será diferente del estilo aplicado a los componentes de contenido dentro de.

Por ejemplo, agregue un componente **[!UICONTROL Container]** y, a continuación, agregue un componente [Button](#button) dentro de ese contenedor. Puede utilizar un fondo específico para el contenedor y otro para el botón.

CAPTURA DE PANTALLA

## Botón {#button}

Use el componente **[!UICONTROL Botón]** para insertar uno o varios botones en el correo electrónico y redirigir la audiencia de correo electrónico a otra página.

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL Button]** en un **[!UICONTROL Componente de estructura]**.

1. Haga clic en el botón recién agregado para personalizar el texto y tener acceso a las pestañas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]** del panel derecho de Designer de correo electrónico.

   CAPTURA DE PANTALLA

1. En el menú **[!UICONTROL Vínculo]**, agregue la dirección URL a la que desee redirigir al hacer clic en el botón.

1. Elige cómo se redirigirá tu audiencia con la lista desplegable **[!UICONTROL Target]**:

   * **[!UICONTROL Ninguno]**: abre el vínculo en el mismo fotograma en el que se hizo clic (predeterminado).
   * **[!UICONTROL En blanco]**: abre el vínculo en una nueva ventana o ficha.
   * **[!UICONTROL Self]**: abre el vínculo en el mismo fotograma en el que se hizo clic.
   * **[!UICONTROL Principal]**: abre el vínculo en el marco principal.
   * **[!UICONTROL Top]**: abre el vínculo en todo el cuerpo de la ventana.

   CAPTURA DE PANTALLA

1. Puede personalizar aún más el botón cambiando atributos de estilo como **[!UICONTROL Borde]**, **[!UICONTROL Tamaño]**, **[!UICONTROL Margen]**, etc. en el panel **[!UICONTROL Configuración de componentes]**.

## Texto {#text}

Use el componente **[!UICONTROL Texto]** para insertar texto en el correo electrónico y ajustar el estilo (borde, tamaño, relleno, etc.) con la ficha **[!UICONTROL Estilos]**.

CAPTURA DE PANTALLA

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL Texto]** en un **[!UICONTROL Componente de estructura]**.

1. Haga clic en el componente que acaba de agregar para personalizar el texto y tener acceso a las pestañas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]** en el panel derecho del Designer de correo electrónico.

1. Cambie el texto con las siguientes opciones disponibles en la barra de herramientas:

   CAPTURA DE PANTALLA

   * **[!UICONTROL Cambiar estilo de texto]**: aplique negrita, cursiva, subrayado o tachado al texto.
   * **Cambiar alineación**: elija entre alineación a la izquierda, a la derecha, al centro o justificada para el texto.
   * **[!UICONTROL Crear lista]**: agregue una lista de viñetas o números al texto.
   * **[!UICONTROL Establecer encabezado]**: agregue hasta seis niveles de encabezado al texto.
   * **Tamaño de fuente**: seleccione el tamaño de fuente del texto en píxeles.
   * **[!UICONTROL Cambiar color de fuente]**: elija el color de la fuente.
   * **[!UICONTROL Insertar vínculo]**: agregue cualquier tipo de vínculo al contenido.
   * **[!UICONTROL Editar imagen]**: agregue una imagen o un recurso al componente de texto. `[Learn more about asset management](../integrations/assets.md)`
   * **[!UICONTROL Cambiar color de fuente]**: elija el color de la fuente.
   * **[!UICONTROL Agregar personalización]**: agregue campos de personalización para personalizar el contenido de los datos de perfiles. `[Learn more about content personalization](../personalization/personalize.md)`
   * **[!UICONTROL Mostrar el código fuente]**: muestra el código fuente del texto. No se puede modificar.
   * **[!UICONTROL Habilitar contenido condicional]**: agregue contenido condicional para adaptar el contenido del componente a los perfiles de destino. `[Learn more about dynamic content](../personalization/get-started-dynamic-content.md)`
   * **[!UICONTROL Duplicado]**: agregue una copia del componente de texto.
   * **[!UICONTROL Eliminar]**: elimina el componente de texto seleccionado del correo electrónico.

1. Ajuste los demás atributos de estilo, como el color del texto, la familia de fuentes, el borde, el relleno, el margen, etc. de la ficha **[!UICONTROL Estilos]**.

   CAPTURA DE PANTALLA

## Divisor {#divider}

Use el componente **[!UICONTROL Divisor]** para insertar una línea divisoria y organizar el diseño y el contenido del correo electrónico.

Puede ajustar atributos de estilo como el color, el estilo y la altura de la línea desde las fichas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]**.

CAPTURA DE PANTALLA

## HTML {#HTML}

Use el componente **[!UICONTROL HTML]** para copiar y pegar las diferentes partes de su HTML existente. Esto le permite crear componentes modulares de HTML gratuitos para reutilizar contenido externo.

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL HTML]** en un **[!UICONTROL componente de estructura]**.

1. Haga clic en el componente que acaba de agregar y, a continuación, seleccione **[!UICONTROL Mostrar código fuente]** en la barra de herramientas contextual para agregar su HTML.

   CAPTURA DE PANTALLA

1. Copie y pegue el código de HTML que desee agregar a su correo electrónico y haga clic en **[!UICONTROL Guardar]**.

   CAPTURA DE PANTALLA

>[!NOTE]
>
>Para que un contenido externo sea compatible con Email Designer, Adobe recomienda crear un mensaje desde cero y copiar el contenido del correo electrónico existente en los componentes.

## Imagen {#image}

Utilice el componente **[!UICONTROL Image]** para insertar un archivo de imagen del equipo en el contenido del correo electrónico.

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL Imagen]** en un **[!UICONTROL Componente de estructura]**.

   CAPTURA DE PANTALLA

1. En la pestaña **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Examinar]** para elegir un archivo de imagen de sus recursos o en **[!UICONTROL Importar medios]** para cargar un recurso en Adobe Experience Manager Assets.

   Para obtener más información sobre [!DNL Adobe Experience Manager Assets], consulte [Documentación de Adobe Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/introduction.html){target="_blank"}.

   >[!NOTE]
   >
   > Para garantizar que los vínculos permanezcan activos y evitar problemas de caducidad, se recomienda utilizar Adobe Assets en lugar de depender de una dirección URL de origen para las imágenes.

1. También puedes buscar directamente en Adobe Stock con la opción **[!UICONTROL Buscar fotos de Adobe Stock]**.

1. Haga clic en el componente recién agregado y configure las propiedades de la imagen:

   * **[!UICONTROL Título de imagen]** le permite definir un título para su imagen.
   * **[!UICONTROL Texto alternativo]** le permite definir el pie de ilustración vinculado a la imagen. Esto corresponde al atributo alternativo de HTML.

   CAPTURA DE PANTALLA

1. También puede elegir **[!UICONTROL Buscar fotografías similares de Stock]**. `[Learn more](../integrations/stock.md)`

1. En la ficha **[!UICONTROL Estilos]**, ajuste los demás atributos de estilo como margen, borde, etc. o agregando un vínculo para redirigir la audiencia a otro contenido desde el panel **[!UICONTROL Configuración de componentes]**.

## Social {#social}

Use el componente **[!UICONTROL Social]** para insertar vínculos a páginas de medios sociales en el contenido del correo electrónico.

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL Social]** en un **[!UICONTROL componente de estructura]**.

1. Seleccione el componente recién agregado.

1. En el campo **[!UICONTROL Social]** de la ficha **[!UICONTROL Configuración]**, elija los medios sociales que desee agregar o quitar.

   CAPTURA DE PANTALLA

1. Elija el tamaño de los iconos en el campo dedicado.

1. Haga clic en cada uno de los iconos de medios sociales para configurar la **[!UICONTROL URL]** a la que se redirigirá la audiencia.

   CAPTURA DE PANTALLA

1. También puede cambiar los iconos de cada uno de sus medios sociales si es necesario desde su Assets.

1. Ajuste los demás atributos de estilo, como estilo, margen, borde, etc. de la ficha **[!UICONTROL Estilos]**.

## Decisión de oferta {#offer-decision}

Utilice el componente **[!UICONTROL Decisión de oferta]** para insertar ofertas en los mensajes. El motor `[decision management](../offers/get-started/starting-offer-decisioning.md)` elegirá la mejor oferta para entregarla a sus clientes.

1. Desde **[!UICONTROL Componentes de contenido]**, arrastre y suelte el componente **[!UICONTROL Decisión de oferta]** en un **[!UICONTROL Componente de estructura]**.

1. Haga clic en **[!UICONTROL Agregar]** para seleccionar su **[!UICONTROL decisión de oferta]**.

   CAPTURA DE PANTALLA

1. En la lista desplegable, seleccione sus **[!UICONTROL ubicaciones]**.  A continuación, seleccione la **[!UICONTROL decisión de oferta]** que desee agregar al contenido y haga clic en **[!UICONTROL Agregar]**.

   CAPTURA DE PANTALLA

1. Desde la pestaña **[!UICONTROL Decisión de oferta]**, puede obtener una vista previa de la oferta insertada o cambiarla.

Aprenda a agregar ofertas personalizadas a un correo electrónico en `[this section](add-offers-email.md)`.

>[!IMPORTANT]
>
>Si se realizan cambios en una decisión de oferta que se utiliza en el mensaje de un recorrido, se debe cancelar la publicación del recorrido y volver a publicarlo.  Esto garantizará que los cambios se incorporen al mensaje del recorrido y que el mensaje sea coherente con las últimas actualizaciones.

