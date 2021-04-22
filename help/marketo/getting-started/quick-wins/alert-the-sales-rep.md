---
unique-page-id: 2359424
description: Alerta al representante de ventas - Documentos de Marketo - Documentación del producto
title: Alerta al representante de ventas
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Alerta al representante de ventas {#alert-the-sales-rep}

## Misión: Alerta al representante de ventas cuando una persona rellene un formulario en su sitio web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Para enviar automáticamente correos electrónicos de alerta a los representantes de ventas, todo lo que necesita es un correo electrónico de alerta y una campaña de correo electrónico. Así es como hacerlo.

>[!PREREQUISITES]
>
>[Página de aterrizaje con un formulario](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Paso 1: Crear un correo electrónico de alerta {#step-create-an-alert-email}

1. Vaya al área **Marketing Activities** .

   ![](assets/one-5.png)

1. Seleccione **My Program** que creó en la [Página de aterrizaje con una victoria rápida de Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) y, en **Nuevo**, haga clic en **Nuevo recurso local**.

   ![](assets/two-6.png)

1. Haga clic en **Email**.

   ![](assets/three-5.png)

1. **** Asigne un nombre al correo electrónico &quot;Mi alerta de correo electrónico&quot;, seleccione una plantilla y haga clic en  **Crear**.

   ![](assets/four-4.png)

1. Introduzca los **Desde Nombre**, **Desde Correo electrónico**, **Respuesta a** y **Asunto** que desea que vea su equipo de ventas.

   ![](assets/five-5.png)

1. Haga doble clic para editar el texto del correo electrónico.

   ![](assets/six-5.png)

1. Escriba el contenido del correo electrónico.

   ![](assets/seven-6.png)

1. Coloque el cursor donde desee insertar la información de contacto de la persona y haga clic en el icono **Insertar token**.

   ![](assets/eight-4.png)

1. Busque y seleccione el `{{SP_Send_Alert_Info}}` **Token** y haga clic en **Insertar**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} es un token especial para los correos electrónicos de alerta. Consulte [Usar el token de información de alerta de envío](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) para obtener más información.

1. Haga clic en **Guardar**.

   ![](assets/ten-5.png)

1. Cierre la pestaña o ventana del editor de correo electrónico.

   ![](assets/eleven-5.png)

1. En **Acciones de correo electrónico** haga clic en **Aprobar**.

   ![](assets/twelve-4.png)

## Paso 2: Crear una campaña de Déclencheur de alertas {#step-create-an-alert-trigger-campaign}

1. Seleccione **My Program** creado anteriormente y, en **New**, haga clic en **New Smart Campaign**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **** Asigne un nombre a la campaña &quot;Mi campaña de alertas&quot; y haga clic en  **Crear**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. En la pestaña **Smart List**, busque y arrastre el déclencheur **Rellenar formulario** al lienzo.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Seleccione el formulario que hemos creado anteriormente.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. En la pestaña **Flow**, busque y arrastre la acción de flujo **Send Alert** al lienzo.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Seleccione **My Alert Email** creado anteriormente y deje **Send To** como **Sales Owner**.

   ![](assets/eighteen-1.png)

1. Escriba su dirección de correo electrónico en el campo **To Other Emails**.

   ![](assets/nineteen-2.png)

1. Vaya a la pestaña **Schedule** y haga clic en el botón **Activate**.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Establezca **Qualification Rules** en **cada vez** (editando la campaña inteligente) para permitir que la misma persona déclencheur alertas varias veces.

1. Haga clic en **Activate** en la pantalla de confirmación.

   ![](assets/twenty-one-1.png)

## Paso 3: ¡Pruébelo! {#step-test-it-out}

1. Seleccione la página de aterrizaje y haga clic en **Ver página aprobada**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >No olvide aprobar páginas de aterrizaje; no se activan hasta que se aprueban.

1. Complete el formulario y haga clic en **Submit**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Debería recibir su correo electrónico en breve. Una vez que haya verificado que todo funciona como debería, elimine su dirección de correo electrónico del flujo Enviar alerta (consulte el paso 2.7 anterior).

   >[!NOTE]
   >
   >Haga clic en la pestaña **Información de persona** en Marketo para ver la información de contacto.

## ¡Misión finalizada! {#mission-complete}

<br> 

[◄ Misión 7: Personalización de un correo electrónico](personalize-an-email.md)

[Misión 9: Actualizar datos de posibles clientes ►](update-person-data.md)
