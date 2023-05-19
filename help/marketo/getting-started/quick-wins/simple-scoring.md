---
unique-page-id: 2359414
description: 'Puntuación simple: Documentos de Marketo: documentación del producto'
title: Puntuación simple
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 74da8ebbd564b11e2795da31321ca47493135f48
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Puntuación simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configuración y adición de una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}


## Paso 1: Crear una campaña de puntuación {#step-create-a-scoring-campaign}

1. Vaya a la **[!UICONTROL Actividades de marketing]** área.

   ![](assets/simple-scoring-1.png)

1. Haga clic con el botón derecho **Aprendizaje** y haga clic en **[!UICONTROL Nueva carpeta de campaña]**.

   ![](assets/simple-scoring-2.png)

1. Asigne a la carpeta de campaña el nombre &quot;Puntuación&quot; y haga clic en **[!UICONTROL Crear]**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Si ya tiene una carpeta Puntuación, póngale otro nombre, como Puntuación 1. Los nombres de las carpetas deben ser únicos.

1. Haga clic con el botón derecho **Puntuación** carpeta y seleccione **[!UICONTROL Nueva campaña inteligente]**.

   ![](assets/simple-scoring-4.png)

1. Asigne a la campaña el nombre &quot;Cambiar puntuación&quot; y haga clic en **[!UICONTROL Crear]**.

   ![](assets/simple-scoring-5.png)

1. Haga clic en **[!UICONTROL Lista inteligente]** pestaña.

   ![](assets/simple-scoring-6.png)

   Queremos que esta campaña se ejecute cada vez que una persona rellene su **Formulario de solicitud de prueba**.

1. Busque y arrastre el **[!UICONTROL Rellena el formulario]** déclencheur en el lienzo izquierdo.

   ![](assets/simple-scoring-7.png)

1. Seleccionar **Mi formulario**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Si ha completado la [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} ganancia rápida, deberías tener el formulario. Si ha utilizado un nombre diferente para el formulario, selecciónelo.

1. Haga clic en **[!UICONTROL Flujo]** pestaña.

   ![](assets/simple-scoring-9.png)

1. Arrastre el **Cambiar puntuación** acción de flujo en el lienzo izquierdo.

   ![](assets/simple-scoring-10.png)

1. Puede escribir cualquier valor para añadirlo a la puntuación de la persona. Vamos a introducir &quot;+5&quot; en **[!UICONTROL Cambiar]** field.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Las buenas campañas de puntuación son clave para ofrecer personas de alta calidad a Ventas. Leer [**La guía definitiva para la puntuación de posibles clientes**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}.

1. Haga clic en **[!UICONTROL Programación]** y la pestaña **[!UICONTROL Activar]** botón.

   ![](assets/simple-scoring-12.png)

1. Clic **[!UICONTROL Activar]** en la pantalla de confirmación.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Una vez activa, esta campaña se ejecutará cada vez que una persona rellene el formulario. La campaña se seguirá ejecutando hasta que se desactive.

## Paso 2: Rellenar el formulario {#step-fill-out-the-form}

1. Seleccione la página de aterrizaje que creó en la [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} ganancia rápida.

   ![](assets/simple-scoring-14.png)

1. Clic **[!UICONTROL Previsualizar]**. La página de aterrizaje se abrirá en una nueva pestaña.

   ![](assets/simple-scoring-15.png)

1. Rellene el formulario con su nombre, apellidos y dirección de correo electrónico y, a continuación, haga clic en **[!UICONTROL Enviar]**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Utilice el mismo nombre y dirección de correo electrónico que utilizó cuando se introdujo por primera vez como persona para aplicar el aumento de puntuación &quot;+5&quot;.

## Paso 3: Ver la información de la persona {#step-view-the-person-info}

1. Vaya a la **[!UICONTROL Base de datos]** área.

   ![](assets/simple-scoring-17.png)

1. Busque la dirección de correo electrónico que utilizó al rellenar el formulario.

   ![](assets/simple-scoring-18.png)

1. Haga doble clic en la persona.

   ![](assets/simple-scoring-19.png)

Los detalles de su persona se abrirán en una nueva pestaña o ventana. ¿Ve cómo su puntuación aumentó en 5 puntos por rellenar el formulario?

![](assets/simple-scoring-20.png)

## ¡Misión completa! {#mission-complete}

<br> 

[◄ Misión 2: Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Misión 4: ► de respuesta automática de correo electrónico](/help/marketo/getting-started/quick-wins/email-auto-response.md)
