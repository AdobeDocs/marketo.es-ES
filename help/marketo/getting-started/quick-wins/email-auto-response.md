---
unique-page-id: 2359416
description: 'Respuesta automática por correo electrónico: Documentos de Marketo: Documentación del producto'
title: Respuesta automática de correo electrónico
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Respuesta automática de correo electrónico {#email-auto-response}

## Misión: Enviar un correo electrónico de agradecimiento cuando una persona rellene un formulario {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Paso 1: Crear un correo electrónico {#step-create-an-email}

1. Vaya al área Actividades de marketing .

   ![](assets/one-2.png)

1. Seleccione Mi programa en el menú de la izquierda, haga clic en la lista desplegable Nuevo y seleccione Nuevo recurso local.

   ![](assets/two-3.png)

1. Hacer clic en el email.

   ![](assets/three-2.png)

1. Asigne un nombre al correo electrónico &quot;Correo electrónico de respuesta automática&quot;, elija una plantilla y haga clic en Crear.

   ![](assets/four-1.png)

   Se abrirá un editor de correo electrónico en una nueva ventana o pestaña. Si las ventanas emergentes están bloqueadas, haga clic en **Editar borrador** en la página de resumen de recursos para acceder al correo electrónico.

1. Introduzca una línea de asunto y, a continuación, haga doble clic en el área editable del correo electrónico.

   ![](assets/five-2.png)

   _Se abrirá un editor de texto enriquecido sobre el editor de correo electrónico._

1. Resalte el contenido de correo electrónico existente.

   ![](assets/six-2.png)

1. Escriba el contenido del correo electrónico y haga clic en Guardar.

   ![](assets/seven-2.png)

1. Los cambios se guardan automáticamente. Cierre la pestaña o ventana del editor de correo electrónico.

   ![](assets/eight-1.png)

1. Seleccione el nuevo correo electrónico. En Acciones de correo electrónico, haga clic en Aprobar.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Paso 2: Creación de una campaña inteligente {#step-create-a-smart-campaign}

1. Clic con el botón derecho **Mi programa** y haga clic en **Nueva campaña inteligente**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Nombre** su campaña inteligente &quot;Campaña de respuesta automática&quot; y haga clic en **Crear**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Vaya a la **Lista inteligente** pestaña .

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Estamos configurando esta campaña para que se ejecute siempre que una persona rellene el formulario que ha creado en [**Página de aterrizaje con un formulario**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Busque y arrastre el **Rellena el formulario** déclencheur al lienzo izquierdo.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Select **Mi formulario** en la lista desplegable . Haga clic en el **Flujo** pestaña .

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Arrastre el **Enviar correo electrónico** acción de flujo al lienzo izquierdo.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Seleccione su **Correo electrónico de respuesta automática** y vaya a **Programación** pestaña .

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Haga clic en **Editar**.

   ![](assets/8.png)

1. Select **cada vez** y haga clic en **Guardar**.

   ![](assets/9.png)

1. Haga clic en **Activar**.

   ![](assets/10.png)

1. Haga clic en **Activar** en la pantalla de confirmación.

   ![](assets/11.png)

>[!NOTE]
>
>Una vez activa, esta campaña se ejecutará cada vez que una persona rellene el formulario especificado. La campaña seguirá ejecutándose hasta que se desactive.

## Paso 3: Rellenar el formulario {#step-fill-out-the-form}

1. Select **Mi página**. Se creó en la variable [Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} victoria rápida.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Haga clic en **Ver página aprobada**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   La página de aterrizaje &quot;Prueba gratuita&quot; se abrirá en una pestaña nueva.

1. Rellene el formulario con su nombre, apellidos y dirección de correo electrónico y, a continuación, haga clic en **Submit**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Asegúrese de utilizar su dirección de correo electrónico real para obtener el correo electrónico.

## Misión finalizada {#mission-complete}

En solo unos minutos debería ver el correo electrónico de respuesta automática en su bandeja de entrada. ¡bueno trabajo!

<br> 

[◄ Misión 3: Puntuación simple](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Misión 5: Importar una lista de personas ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
