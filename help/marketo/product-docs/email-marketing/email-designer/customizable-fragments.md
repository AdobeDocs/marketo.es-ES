---
solution: Marketo Engage
product: marketo
title: Fragmentos personalizables
description: Aprenda a personalizar fragmentos haciendo que algunos de sus campos sean editables.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Fragmentos personalizables {#customizable-fragments}

Cuando los fragmentos se utilizan en una plantilla de correo electrónico o de correo electrónico, están bloqueados de forma predeterminada debido a la herencia. Esto significa que los cambios realizados en un fragmento se propagan automáticamente a todos los recursos donde se utiliza el fragmento. Con los fragmentos personalizables, los campos específicos de un fragmento se pueden definir como editables cuando el fragmento se agrega a un correo electrónico o a una plantilla de correo electrónico. Por ejemplo, supongamos que tiene un fragmento con un titular, texto y un botón. Puede designar ciertos campos, como la dirección URL de destino de la imagen o el botón, como editables. Esto permite a los usuarios modificar estos elementos cuando incorporan el fragmento en su plantilla de correo electrónico/correo electrónico, lo que proporciona una experiencia adaptada sin afectar al fragmento original.

Al aprovechar los fragmentos personalizables, puede administrar y personalizar el contenido de forma eficaz sin crear bloques de contenido completamente nuevos ni interrumpir la herencia del fragmento original. Esto garantiza que los cambios realizados en el nivel de fragmento se sigan propagando, al tiempo que permite la personalización necesaria en el nivel de plantilla de correo electrónico/correo electrónico.

Los fragmentos visuales y de expresión se pueden marcar como personalizables. Para obtener instrucciones detalladas sobre cómo proceder con cada tipo de fragmento, consulte las secciones siguientes.

## Agregar campos editables en fragmentos visuales {#visual}

Para poder editar partes de un fragmento visual, siga estos pasos:

>[!NOTE]
>
>Los campos editables se pueden agregar a los componentes **image**, **text** y **button**. Para los componentes de **HTML**, se agregan campos editables mediante el editor de personalización, de forma similar a los fragmentos de expresiones. [Aprenda a agregar campos editables en componentes de HTML y fragmentos de expresiones](#expression)

1. Abra la pantalla de edición de contenido del fragmento.

1. Seleccione el componente del fragmento en el que desea configurar los campos editables.

1. El panel de propiedades del componente se abre en el lado derecho. Seleccione la pestaña **[!UICONTROL Campos editables]** y luego cambie la opción **[!UICONTROL Habilitar edición]**.

1. Todos los campos que se pueden editar para el componente seleccionado se muestran en el panel. Los campos disponibles para editar dependen del tipo de componente seleccionado.

   En el ejemplo siguiente, permitimos la edición de la URL del botón &quot;Haga clic aquí&quot;.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Haga clic en **[!UICONTROL Información general]** para comprobar todos los campos editables y sus valores predeterminados.

   En este ejemplo, el campo URL del botón se muestra con el valor predeterminado definido en el componente. Los usuarios podrán personalizar este valor una vez que hayan agregado el fragmento a su contenido.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Guarde los cambios cuando haya terminado.

Después de agregar el fragmento a un correo electrónico, los usuarios podrán personalizar todos los campos editables configurados en el fragmento.

## Añadir campos editables en componentes de HTML y fragmentos de expresiones {#expression}

Para poder editar partes de un componente de HTML o de un fragmento de expresión, debe utilizar una sintaxis específica en el editor de expresiones. Esto implica declarar una _variable_ con un valor predeterminado que los usuarios pueden anular después de agregar el fragmento a su contenido.

Por ejemplo, supongamos que desea crear un fragmento para agregarlo a los correos electrónicos y permitir a los usuarios personalizar un color específico utilizado en diferentes ubicaciones, como marcos o colores de fondo de botones. Al crear el fragmento, debe declarar una variable con un _ID único_ (por ejemplo, &quot;color&quot;) e invocarla en las ubicaciones deseadas del contenido del fragmento donde desee aplicar este color. Al añadir el fragmento a su contenido, los usuarios pueden personalizar el color utilizado siempre que se haga referencia a la variable.

Para los componentes de HTML, solo los elementos específicos pueden convertirse en campos editables. Expanda la sección siguiente para obtener más información.

+++Elementos editables en componentes de HTML:

Los elementos siguientes pueden convertirse en campos editables en un componente de HTML:

* Una parte del texto
* Una dirección URL completa para un vínculo o una imagen (no funciona con una parte de una dirección URL)
* Propiedad CSS completa (no funciona con la propiedad parcial)

Por ejemplo, en el siguiente código, cada elemento resaltado en rojo puede convertirse en una propiedad:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++

>[!MORELIKETHIS]
>
>[Fragmentos](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
