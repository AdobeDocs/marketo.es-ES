---
description: 'Creación de un mensaje SMS de vibraciones: documentos de Marketo, documentación del producto'
title: Crear un mensaje SMS de Vibes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Crear un mensaje SMS de Vibes {#create-a-vibes-sms-message}

A continuación se muestra cómo crear un mensaje SMS de Vibes.

>[!AVAILABILITY]
>
>Esta función está disponible como complemento para su cuenta de Adobe Marketo Engage. Para que se pueda aprovisionar correctamente, debe adquirirse a través del Adobe. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

1. Ir a **Actividades de marketing**.

   ![](assets/mobile-right-click-hand.jpg)

1. Haga clic con el botón derecho en un programa y seleccione **Nuevo recurso local**.

   ![](assets/mobile-right-click-hand.jpg)

1. Clic **Nuevo recurso local**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >También puede hacer clic en el botón **Nuevo** menú desplegable.

1. Clic **Mensaje SMS**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. Introduzca un nombre y una descripción opcional para el nuevo mensaje SMS y haga clic en **Crear**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. Clic **Editar borrador**.

   ![](assets/edit-draft-hand.jpg)

1. En el editor de mensajes, haga clic dentro de la burbuja azul y empiece a introducir texto.

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >El límite de caracteres de un mensaje SMS es de 160 caracteres con el conjunto de caracteres ASCII estándar. Si supera los 160 caracteres, el mensaje se dividirá en función del recuento total de caracteres.

1. Clic **Token** en el menú Insertar para agregar un token al mensaje.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >Si se añade un token, el mensaje puede superar el límite de caracteres. A continuación, el mensaje se divide, lo que da como resultado mensajes adicionales.

   >[!IMPORTANT]
   >
   >Cumplimiento de SMS: todos los mensajes SMS salientes deben incluir el nombre de la marca o la descripción del programa. Las instrucciones HELP y STOP deben proporcionarse al menos una vez al mes por suscriptor para programas de mensajes recurrentes.

   ?????? El uso del acortador de URL de Marketo hará que se utilicen caracteres X en el ?????? del mensaje

1. Clic **Vínculo** en el menú Insertar para añadir un vínculo al mensaje.

   ![](assets/full-message-link-hand.jpg)

1. Seleccione un tipo de vínculo. La página de aterrizaje de Marketo es la predeterminada. Si va con eso, debe seleccionar la página de aterrizaje de la lista desplegable y hacer clic en **Insertar**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >* Los dos vínculos de seguimiento están seleccionados de forma predeterminada.
   >* El uso del acortador de URL de Marketo dará como resultado que se utilicen caracteres X en el mensaje.??????????????????

1. Si desea utilizar una dirección URL externa en su lugar, haga clic en **URL externa** e introduzca la dirección URL en el campo URL. Clic **Insertar**.

   ![](assets/insert-link-url-hands.jpg)

   >[!CAUTION]
   >
   >Se recomienda lo siguiente _no_ utilice acortadores de URL (por ejemplo, Bitly), ya que los operadores pueden marcar el mensaje como correo no deseado.

1. El vínculo se muestra en el mensaje.

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo muestra una vista previa de vínculo del dominio de seguimiento marcado. Si desactiva la casilla de verificación del vínculo mkt_tok, se cambia el vínculo. Desactive también la casilla Rastrear vínculo y la dirección URL se acortará a su longitud básica (por ejemplo, www.mygooglepage.com).

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >El recuento de caracteres refleja solo los caracteres contenidos en el mensaje más bajo.

Si inserta más mensajes que el límite de EE. UU., el editor divide el mensaje en secciones. Hay un límite total absoluto de 900 caracteres. Después de alcanzar ese límite, el mensaje se trunca automáticamente cuando se envía a su audiencia.

LÍMITE DE EE. UU????????
