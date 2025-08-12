---
solution: Marketo Engage
product: marketo
title: TÍTULO
description: Aprenda a optimizar la creación de correos electrónicos con temáticas y módulos reutilizables, lo que garantiza la coherencia y la eficacia del diseño.
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 1cfb28f47ba3c168292b298e1fc7ab2ff638b412
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 4%

---

# Aplicar temáticas al contenido del correo electrónico {#apply-email-themes}

>[!AVAILABILITY]
>
>Actualmente, esta función está en versión Beta y solo se encuentra disponible para los clientes de dicha versión. Para unirse al programa beta, póngase en contacto con su representante de Adobe.

Con las temáticas, los usuarios no técnicos tienen la capacidad de crear contenido reutilizable que se ajuste a una marca y un idioma de diseño específicos agregando estilo personalizado sobre las plantillas estándar<!-- to achieve brand specific results-->.

Esta función permite a los especialistas en marketing aprovechar correos electrónicos visualmente atractivos y coherentes con la marca de forma más rápida y con menos esfuerzo, a la vez que proporciona opciones de personalización avanzadas para satisfacer necesidades de diseño únicas.

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## Protecciones y limitaciones {#themes-guardrails}

* Al crear un correo electrónico desde cero, puede elegir empezar a crear el contenido con un tema para aplicar rápidamente un estilo específico que se ajuste a su marca y diseño.

  Si eliges el modo _Estilo manual_, no podrás aplicar ningún tema a menos que restablezcas tu correo electrónico.

* Los [fragmentos](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) no son compatibles entre los modos _Usar temas_ y _Estilo manual_.

  Para poder usar un fragmento en un contenido donde se aplique un tema, este fragmento debe crearse en el modo _Usar temas_.

* Si usa contenido creado en HTML, estará en [modo de compatibilidad](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) y no podrá aplicar temáticas a este contenido.

  Para aprovechar al máximo todas las funcionalidades de Email Designer, incluidas las temáticas, debe crear contenido nuevo en el modo _Usar temas_ o convertir el [contenido de HTML importado](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html).

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## Crear una temática {#create-and-edit-themes}

Para definir una temática que pueda aprovechar en el contenido futuro del correo electrónico, siga los pasos a continuación.

1. Para empezar, cree una nueva [plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template).

1. Seleccione la opción **[!UICONTROL Crear o editar temáticas]**.

   `![](assets/theme-create.png)`

1. Puede seleccionar la temática predeterminada o utilizar una plantilla Adobe o personalizada. En este ejemplo, seleccione el tema predeterminado y haga clic en **[!UICONTROL Crear]**.

   `![](assets/theme-select.png)`

1. En la ficha **[!UICONTROL Configuración general]**, empiece a definir el tema asignándole un nombre específico para su marca. Puede ajustar la anchura predeterminada de los correos electrónicos y también exportar la temática actual para compartirla en entornos limitados.

   `<!--![](assets/theme-general-settings.png)-->`

1. Utilice el carril de la derecha para navegar por las diferentes pestañas y actualizar la configuración de diseño.

   `![](assets/theme-right-pane.png)`

1. Desde la ficha **[!UICONTROL Colores]**:

   * Use el botón **[!UICONTROL Editar]** para configurar una **[!UICONTROL paleta de colores]** con colores predeterminados para su marca. Seleccione un **[!UICONTROL ajuste preestablecido]** para crear rápidamente una combinación de colores o ajustar cada color de su tema individualmente. También puede utilizar una combinación de ambos.

     `![](assets/theme-colors.gif)`

   * Haga clic en **[!UICONTROL Agregar variante]** para crear varias variantes de color, como el modo claro y oscuro, en las que cada variante tiene su propia paleta de colores y controles de matices.

     `![](assets/theme-colors-variant.png)`

   * Para cada variante, haga clic en el icono Editar para editar cualquier elemento individual. Puede utilizar la paleta predeterminada que ha creado o cualquier color personalizado.

     `![](assets/theme-colors-edit-variant.gif)`

1. En la **[!UICONTROL configuración de texto]**, puede establecer la fuente global que desee usar para todo el tema. Para un control más granular, también puede editar cada título y tipo de párrafo para ajustar la fuente, el tamaño, el estilo, etc.

   `![](assets/theme-text.png)`

1. En la ficha **[!UICONTROL Espaciado]**, seleccione un elemento individual de la lista para espaciarlo correctamente entre los distintos componentes.

   `<!--![](assets/theme-spacing.png)-->`

1. Con las otras pestañas de la derecha, puede administrar por separado cada elemento de botón, divisor, formato de imagen adicional y espaciado del diseño de cuadrícula para esta temática.

   `<!--![](assets/theme-buttons.png)-->`

1. Haga clic en **[!UICONTROL Guardar]** para almacenar este tema para uso futuro.

## Aplicar temáticas a un correo electrónico {#apply-themes}

Para aplicar temáticas de estilo predeterminadas o personalizadas a un correo electrónico, siga los pasos a continuación.

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. Puede seleccionar una de las siguientes acciones:

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >Si eliges el modo _Estilo manual_, no podrás aplicar ningún tema a menos que restablezcas tu correo electrónico.
     >
     >Para usar un [fragmento](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) en el modo _Usar temas_, este fragmento debe haberse creado solo usando el modo _Usar temas_.

1. Una vez que se encuentre en el Designer de correo electrónico, haga clic en el botón **[!UICONTROL Temas]** en el carril derecho. Se muestra el tema predeterminado o el tema de la plantilla. Puede cambiar entre las dos variantes de color para esta temática.

   `![](assets/theme-default-hero.png)`

1. Haga clic en la flecha situada junto a la temática utilizada actualmente. Se muestra la lista de las temáticas personalizadas y de Adobe disponibles.

   `![](assets/theme-hero-change.png)`

1. Haga clic en **[!UICONTROL Temas personalizados]** y seleccione el tema que ha creado.

   `![](assets/theme-select-custom.png)`

1. Haga clic fuera de la lista desplegable. La temática personalizada recién seleccionada aplica automáticamente sus estilos a todos los componentes del correo electrónico. Puede alternar entre las dos variantes de color.

1. Cuando se selecciona un componente, aún se puede desbloquear su estilo mediante el icono dedicado.

   `![](assets/theme-unlock-style.png)`

Puede cambiar de tema en cualquier momento. El contenido del correo electrónico permanece sin cambios, pero los estilos se actualizan para reflejar la nueva temática.

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
