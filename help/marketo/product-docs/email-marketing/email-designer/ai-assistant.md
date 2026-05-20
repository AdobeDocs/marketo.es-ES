---
solution: Marketo Engage
product: marketo
title: Utilizar el Asistente de IA
description: Aprenda a utilizar el asistente de IA para añadir texto e imágenes a los correos electrónicos. Utilice la IA generativa de Adobe en el Designer de correo electrónico para ideas de contenido.
level: Beginner, Intermediate
feature: Email Designer
exl-id: e07ed645-d8a3-483f-aa1f-f82bc9cb8634
TQID: https://experienceleague.adobe.com/iqJs2yG5ip5vNlwtjvIEjLXp0o0P3-mHVEZmOLcAqBE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 936
ht-degree: 1%

---

# Asistente de IA para Email Designer {#ai-assistant-email-designer}

El asistente de IA de Marketo Engage Email Designer le ayuda a crear correos electrónicos contemporáneos, eficaces e intuitivos. Esto se logra a través de la tecnología de IA generativa de Adobe y la biblioteca rápida junto con Firefly para la generación de imágenes que ayuda a crear contenido adecuado para una persona en particular / grupo de compra, etapa de recorrido de marketing, estrategia de comunicación, tono, etc. Los activos específicos de la marca también se pueden utilizar para crear contenido.

>[!PREREQUISITES]
>
>El Asistente de IA no está habilitado de forma predeterminada. Primero debe aceptar los [términos básicos de la generación de IA y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} para usar la funcionalidad de generación de IA en el Designer de correo electrónico. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Configurar permisos {#set-up-permissions}

_Después de_ que sigue el requisito previo anterior, los administradores de Marketo deben aplicar el acceso a usuarios/funciones específicos antes de que los usuarios vean los botones GenAI.

+++Obtenga información sobre cómo configurar permisos

1. En Marketo Engage, haga clic en **Administrador** y seleccione **Usuarios y roles**.

   ![](assets/use-the-ai-assistant-0a.png)

1. En la ficha **Roles**, haga doble clic en el rol que desee.

   ![](assets/use-the-ai-assistant-0b.png)

1. En _Access Design Studio_, active la casilla de verificación **Acceder al asistente de IA** y haga clic en **Guardar**.

   ![](assets/use-the-ai-assistant-0c.png)

1. Haga clic en la pestaña Usuarios y seleccione el usuario al que desee proporcionar acceso.

   ![](assets/use-the-ai-assistant-0d.png)

1. Seleccione la función elegida en el paso 3 y el espacio de trabajo deseado (si corresponde). Haga clic en **Guardar**.

   ![](assets/use-the-ai-assistant-0e.png)

+++

## Casos de uso {#use-cases}

Hay algunos casos de uso principales para el asistente de IA:

* [Cree una línea de asunto o un encabezado previo](#create-a-subject-line-preheader) para su correo electrónico
* [Crea contenido para una sección específica](#create-content-for-a-specific-section) de tu correo electrónico
* [Crear un correo electrónico completo](#create-an-entire-email) a partir de una plantilla seleccionada

## Creación de una línea de asunto/encabezado previo {#create-a-subject-line-preheader}

Puede utilizar el asistente de IA para crear una línea de asunto, un encabezado previo o ambos.

![](assets/use-the-ai-assistant-1.png)

El ejemplo siguiente ilustra la línea de asunto. Para un preencabezado, se pueden seguir los mismos pasos haciendo clic en la casilla de verificación _Preheader_ (que se ve en la imagen anterior).

Cuando se cree un correo electrónico con la Nueva Designer de correo electrónico, introduzca una línea de asunto temporal.

Una vez creado el correo electrónico, la línea de asunto se encuentra en la columna _Detalles_, a la derecha. Haga clic en el botón del asistente de IA ( ![Icono de filtro](assets/icon-ai-assistant.png) ) que se encuentra junto a él para obtener ayuda con la creación de una nueva línea de asunto mediante la funcionalidad de IA general.

![](assets/use-the-ai-assistant-2.png)

Habilite la opción **Usar contenido de referencia** para el asistente de IA a fin de personalizar el nuevo contenido en función del contenido seleccionado.

Introduzca el mensaje para personalizar la línea de asunto. Introduzca la configuración de texto relevante y cargue cualquier recurso de marca que desee utilizar como referencia para crear una línea de asunto adecuada.

![](assets/use-the-ai-assistant-3.png)

La configuración de texto incluye:

<table><tbody>
  <tr>
    <td style="width:25%"><b>Grupo de compras</b></td>
    <td>Grupo de compra específico al que se dirige (por ejemplo, Profesional, Influencer, Responsable de la toma de decisiones).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Fase de Recorrido de marketing</b></td>
    <td>Destinatarios en una fase de recorrido de marketing determinada (por ejemplo, Discover, Evaluar, Comprometer).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Estrategia de comunicación</b></td>
    <td>El objetivo de la comunicación (por ejemplo, urgente, prueba social, informativa).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Idioma</b></td>
    <td>Idioma en el que desea que se genere la línea de asunto.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Tono</b></td>
    <td>Tono en el que desea que se genere el contenido (por ejemplo, Inspiracional, Emocionante, Humorístico).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Emojis</b></td>
    <td>Permite incluir emojis en el contenido generado.</td>
  </tr>
</tbody>
</table>

Al hacer clic en **Generar**, aparecen ejemplos para que usted elija entre:

![](assets/use-the-ai-assistant-4.png)

También puede cargar un recurso de marca para utilizar contenido dentro del recurso como referencia para crear la línea de asunto.

![](assets/use-the-ai-assistant-5.png)

Para elegir una variación, seleccione su casilla de verificación y haga clic en **Seleccionar**. También puede modificarlo si hace clic en **Refinar**. Además, puede proporcionar comentarios haciendo clic en el icono de pulgares hacia arriba o hacia abajo para que la tecnología Gen-AI conozca sus preferencias.

Después de realizar la selección, la línea de asunto se rellena en los detalles del correo electrónico.

![](assets/use-the-ai-assistant-6.png)

## Creación de contenido para una sección específica del correo electrónico {#create-content-for-a-specific-section}

Una vez creado el correo electrónico, tiene la opción de modificar determinadas secciones, imágenes o texto.

![](assets/use-the-ai-assistant-7.png)

En este ejemplo, utilizamos una plantilla financiera. Si una o más de las imágenes existentes no satisfacen sus necesidades, puede indicar al asistente de IA que cree una nueva imagen basada en la descripción. Seleccione la imagen que desee y haga clic en el icono Asistente de IA.

![](assets/use-the-ai-assistant-8.png)

Introduzca los detalles relevantes en el mensaje, como, &quot;Un banquero sentado en su escritorio con pilas de dinero en efectivo&quot;. También puede utilizar la biblioteca de mensajes (a la derecha del mensaje) si no está seguro de qué escribir. Haga clic en **Configuración de imagen**.

![](assets/use-the-ai-assistant-9.png)

Haga clic en el botón de alternancia para habilitar _Generar imágenes con IA_ y, a continuación, cambie la configuración deseada, incluido el modelo que se va a utilizar (Adobe Firefly o Gemini 2.5 Nano Banana). Cuando termine, haga clic en **Generar**.

![](assets/use-the-ai-assistant-10.png)

Se crean varias variantes. Elige tu favorito y haz clic en **Aplicar**.

![](assets/use-the-ai-assistant-11.png)

>[!NOTE]
>
>Si ninguna de las imágenes cumple con sus necesidades, vuelva a hacer clic en **Generar** para crear nuevas versiones.

De forma similar a la imagen, también se pueden modificar las partes de texto del correo electrónico.

## Crear un correo electrónico completo a partir de una plantilla seleccionada {#create-an-entire-email}

Esta opción solo está disponible si el correo electrónico se crea con una plantilla existente. Puede ser una plantilla estándar proporcionada por el Designer de correo electrónico, una plantilla guardada que ya haya creado o una plantilla importada mediante la opción Importar HTML. Esta opción no está disponible si elige [Diseño desde cero](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#design-from-scratch) para el correo electrónico.

Seleccione una plantilla sin seleccionar ningún componente y haga clic en el botón Asistente de IA en el Designer de correo electrónico.

![](assets/use-the-ai-assistant-12.png)

Introduzca el mensaje correspondiente y elija la configuración de texto, los recursos de marca y cualquier configuración de imagen que desee para el correo electrónico.

![](assets/use-the-ai-assistant-13.png)

Si desea generar imágenes con Firefly, seleccione la opción Configuración de imagen y seleccione la opción para **Generar imágenes con IA**.

![](assets/use-the-ai-assistant-14.png)

Seleccione el _Tipo de contenido_, _Color y tono_, _Iluminación_ y _Composición_ deseados para crear imágenes de IA general para su correo electrónico. Haga clic en **Generar** cuando haya terminado.

![](assets/use-the-ai-assistant-15.png)

Vea el aspecto que tendrá una variación en su correo electrónico al hacer clic en **Vista previa**. Elija una variación haciendo clic en **Aplicar**.
