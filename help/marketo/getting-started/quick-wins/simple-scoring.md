---
unique-page-id: 2359414
description: 'Puntuación simple: Documentos de Marketo: Documentación del producto'
title: Puntuación simple
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 10637f7853c5b0f8a076779d95b8163b2de8abcb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Puntuación simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Paso 1: Creación de una campaña de puntuación {#step-create-a-scoring-campaign}

1. Vaya a la **Actividades de marketing** .

   ![](assets/simple-scoring-1.png)

1. Haga clic con el botón derecho en su **Aprendizaje** carpeta y haga clic en **Nueva carpeta de campañas**.

   ![](assets/simple-scoring-2.png)

1. Asigne a la carpeta de campañas el nombre &quot;Puntuación&quot; y haga clic en **Crear**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Si ya tiene una carpeta de Puntuación, asígnele un nombre diferente a este, como Puntuación 1. Los nombres de carpeta deben ser únicos.

1. Haga clic con el botón derecho en su **Puntuación** carpeta y seleccione **Nueva campaña inteligente**.

   ![](assets/simple-scoring-4.png)

1. Asigne a la campaña el nombre &quot;Cambiar puntuación&quot; y haga clic en **Crear**.

   ![](assets/simple-scoring-5.png)

1. Haga clic en el **Lista inteligente** pestaña .

   ![](assets/simple-scoring-6.png)

   Queremos que esta campaña se ejecute siempre que una persona rellene su **Formulario de solicitud de prueba**.

1. Busque y arrastre el **Rellena el formulario** déclencheur en el lienzo izquierdo.

   ![](assets/simple-scoring-7.png)

1. Select **Mi formulario**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Si ha completado el [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} victoria rápida, debería tener el formulario . Si ha utilizado un nombre diferente para el formulario, selecciónelo.

1. Haga clic en el **Flujo** pestaña .

   ![](assets/simple-scoring-9.png)

1. Arrastre el **Cambiar puntuación** en el lienzo izquierdo.

   ![](assets/simple-scoring-10.png)

1. Puede escribir cualquier valor que desee añadir a la puntuación de la persona. Introduzcamos &quot;+5&quot; en la **Cambiar** campo .

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Las buenas campañas de puntuación son clave para ofrecer a las ventas personas de alta calidad. Lectura [**La Guía definitiva para la puntuación de posibles clientes**](https://www.marketo.com/definitive-guides/lead-scoring/){target=&quot;_blank&quot;}.

1. Haga clic en el **Programación** y **Activar** botón.

   ![](assets/simple-scoring-12.png)

1. Haga clic en **Activar** en la pantalla de confirmación.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Una vez activa, esta campaña se ejecutará cada vez que una persona rellene el formulario. La campaña seguirá ejecutándose hasta que se desactive.

## Paso 2: Rellenar el formulario {#step-fill-out-the-form}

1. Seleccione la página de aterrizaje que ha creado en la [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} victoria rápida.

   ![](assets/simple-scoring-14.png)

1. Haga clic en **Vista previa**. La página de aterrizaje se abrirá en una pestaña nueva.

   ![](assets/simple-scoring-15.png)

1. Rellene el formulario con su nombre, apellidos y dirección de correo electrónico y, a continuación, haga clic en **Submit**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Utilice el mismo nombre y dirección de correo electrónico que utilizó cuando se introdujo por primera vez como persona para aplicar el aumento de puntuación &quot;+5&quot;.

## Paso 3: Ver la información de la persona {#step-view-the-person-info}

1. Vaya al área Base de datos.

   ![](assets/simple-scoring-17.png)

1. Busque la dirección de correo electrónico que utilizó al rellenar el formulario.

   ![](assets/simple-scoring-18.png)

1. Haga doble clic en su persona.

   ![](assets/simple-scoring-19.png)

Los detalles de la persona se abrirán en una nueva pestaña o ventana. ¿Ver cómo su puntuación aumentó en 5 puntos para rellenar el formulario?

![](assets/simple-scoring-20.png)

## ¡Misión finalizada! {#mission-complete}

<br> 

[◄ Misión 2: Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Misión 4: Respuesta automática por correo electrónico ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
