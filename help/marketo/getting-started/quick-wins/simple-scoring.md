---
unique-page-id: 2359414
description: 'Puntuación simple: Documentos de Marketo: Documentación del producto'
title: Puntuación simple
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Puntuación simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](get-set-up-and-add-a-person.md)
>* [Página de aterrizaje con un formulario](landing-page-with-a-form.md)


## Paso 1: Crear una campaña de puntuación {#step-create-a-scoring-campaign}

1. Vaya al área **Marketing Activities** .

   ![](assets/ma-1.png)

1. Haga clic con el botón derecho en la carpeta **Learning** y haga clic en **New Campaign Folder**.

   ![](assets/two-2.png)

1. Asigne a la carpeta de campañas el nombre &quot;Puntuación&quot;.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Si ya tiene una carpeta de Puntuación, asígnele un nombre diferente a este, como Puntuación 1. Los nombres de carpeta deben ser únicos.

1. A continuación, haga clic con el botón derecho en la nueva carpeta **Scoring** y seleccione **New Smart Campaign**.

   ![](assets/four.png)

1. **** Asigne un nombre a la campaña &quot;Cambiar puntuación&quot; y haga clic en  **Crear**.

   ![](assets/five-1.png)

1. Haga clic en la pestaña **Smart List**.

   ![](assets/six-1.png)

   Queremos que esta campaña se ejecute siempre que una persona rellene su **Formulario de solicitud de prueba**.

1. Busque y arrastre el déclencheur **Rellenar formulario** al lienzo izquierdo.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Seleccione **Mi formulario**.

   >[!NOTE]
   >
   >Si ha completado la [Página de aterrizaje con una victoria rápida de Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md), debe tener el formulario. Si ha utilizado un nombre diferente para el formulario, selecciónelo.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Haga clic en la pestaña **Flow**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Arrastre la acción de flujo **Change Score** al lienzo izquierdo.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Puede escribir cualquier valor que desee añadir a la puntuación de la persona. Vamos a introducir &quot;+5&quot; en el campo **Change**.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Las buenas campañas de puntuación son clave para ofrecer a las ventas personas de alta calidad. Lea [**La Guía definitiva para la puntuación de posibles clientes**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Haga clic en la pestaña **Schedule** y en el botón **Activate**.

   ![](assets/twelve-1.png)

1. Haga clic en **Activate** en la pantalla de confirmación.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>Una vez activa, esta campaña se ejecutará cada vez que una persona rellene el formulario. La campaña seguirá ejecutándose hasta que se desactive.

## Paso 2: Rellene el formulario {#step-fill-out-the-form}

1. Seleccione la página de aterrizaje que ha creado en la [Página de aterrizaje con una victoria rápida de Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/fourteen-1.png)

1. Haga clic en **Ver página aprobada**. La página de aterrizaje se abrirá en una pestaña nueva.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Rellene el formulario con su nombre, apellidos y dirección de correo electrónico y, a continuación, haga clic en **Enviar**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Utilice el mismo nombre y dirección de correo electrónico que utilizó cuando se introdujo por primera vez como persona para aplicar el aumento de puntuación &quot;+5&quot;.

## Paso 3: Ver la información de la persona {#step-view-the-person-info}

1. Vaya al área Base de datos.

   ![](assets/db-2.png)

1. Busque la dirección de correo electrónico que utilizó al rellenar el formulario.

   ![](assets/eighteen.png)

1. Haga doble clic en su persona.

   ![](assets/nineteen.png)

Los detalles de la persona se abrirán en una nueva pestaña o ventana. ¡¿Ver cómo su puntuación aumentó en 5 puntos para rellenar el formulario?!

![](assets/twenty.png)

**¡Felicidades!** Ha creado una campaña de puntuación.
[◄ Misión 2: Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Misión 4: Respuesta automática por correo electrónico ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
