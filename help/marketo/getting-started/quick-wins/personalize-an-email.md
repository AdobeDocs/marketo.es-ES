---
unique-page-id: 2359422
description: Personalización de un correo electrónico - Documentos de marketing - Documentación del producto
title: Personalización de un correo electrónico
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Personalización de un correo electrónico {#personalize-an-email}

## Misión: Personalice sus correos electrónicos agregando tokens de datos {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar y Añadir una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Enviar una explosión de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Perforación, Perforación, Nurtura](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Paso 1: Seleccionar un correo electrónico para personalizar {#step-select-an-email-to-personalize}

1. Seleccione uno de los correos electrónicos de formación creados en la [anterior victoria](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) rápida y haga clic en **Editar borrador**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Esto crea una copia del correo electrónico como borrador. Debe aprobar el borrador para que los cambios se activen.

Si no ha habilitado un bloqueador de elementos emergentes, el editor de correo electrónico se abrirá en una nueva ficha o ventana. De lo contrario, haga clic en **Editar borrador** dos veces.

## Paso 2: Convertir al vendedor en el remitente {#step-make-the-salesperson-the-sender}

1. Seleccione el campo **Desde** , resalte y **elimine** el nombre actual.

   ![](assets/two-5.png)

1. Haga clic en el icono **Token** a la derecha del campo **Desde** .

   ![](assets/three-4.png)

1. Busque y seleccione el **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Escriba el nombre de la compañía y un guión para el valor **** predeterminado para asegurarse de que se muestra algo en caso de que el nombre del representante de venta no esté disponible. Haga clic en **Insertar**.

   ![](assets/five-4.png)

1. Pulse la barra espaciadora del campo **Desde** , asegurándose de que el cursor parpadea un espacio después del token que acaba de insertar. A continuación, vuelva a hacer clic en el icono **Token** .

   ![](assets/six-4.png)

1. Busque y seleccione el **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Escriba &quot;Ventas&quot; para el Valor **** predeterminado y haga clic en **Insertar**.

   ![](assets/eight-3.png)

## Paso 3: Añadir el nombre del posible cliente en el correo electrónico {#step-add-the-leads-name-to-the-email}

1. Seleccione la sección editable superior, haga clic en el icono de engranaje y seleccione **Editar**.

   ![](assets/nine-2.png)

1. Añada un espacio después de &quot;Hola&quot; y coloque el cursor delante de la coma y, a continuación, haga clic en el icono **Insertar token** .

   ![](assets/ten-4.png)

1. Busque y seleccione el **`{{lead.First Name}}`** token.

   ![](assets/eleven-4.png)

1. Escriba &quot;Amigo&quot; (o cualquier etiqueta que desee) en el campo Valor **** predeterminado y haga clic en **Insertar**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Incluya siempre un valor predeterminado para los tokens; esto garantiza que el valor predeterminado se mostrará en el correo electrónico si falta alguna parte de la información personal.

1. Haga clic en **Guardar**.

   ![](assets/thirteen-3.png)

1. Cierre la ficha o ventana del editor de correo electrónico.

   ![](assets/fourteen-3.png)

1. En Acciones **de** correo electrónico, seleccione **Aprobar borrador**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>¿Necesita un repaso rápido sobre cómo enviarse el correo electrónico? Consulte [Enviar una explosión](/help/marketo/getting-started/quick-wins/send-an-email.md)de correo electrónico.

### Misión completada {#mission-complete}

¡Felicitaciones, has personalizado tu correo electrónico!

<br> 

[◄ Misión 6: Perforación, Perforación, Nurtura](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Misión 8: Alerta al representante de ventas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
