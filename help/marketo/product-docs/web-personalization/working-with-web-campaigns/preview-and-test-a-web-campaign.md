---
unique-page-id: 10092925
description: Previsualización y prueba de una Campaña Web - Documentos de marketing - Documentación del producto
title: Previsualización y prueba de una Campaña Web
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Previsualización y prueba de una Campaña Web {#preview-and-test-a-web-campaign}

Este artículo muestra diferentes formas de previsualización de una campaña web y también cómo probarla con un segmento de simulación de pruebas en directo en el sitio web.

## Previsualización de una Campaña Web en la página de creación {#preview-a-web-campaign-on-the-creation-page}

1. Vaya a **Web** **Campañas**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Haga clic en** Crear nueva Campaña web******* o en el icono para editar una campaña existente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. En Previsualización en el sitio, agregue la dirección URL de la página y haga clic en **Previsualización**. Se abre una nueva ventana/ficha que muestra la previsualización de campaña.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Haga clic en **Compartir** para abrir un correo electrónico con una dirección URL fija de la previsualización de campaña.

   >[!NOTE]
   >
   >También tiene la opción de instalar un complemento de explorador (ya sea [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [Firefox](https://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi)) para obtener la mejor experiencia de vista previa de la campaña. Consulte la sección siguiente.

## Previsualización de una Campaña Web en la página de creación mediante el complemento del explorador {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Siga los pasos 1 y 2 desde `section above`.
1. Haga clic en el vínculo al complemento del navegador (en este caso, estamos utilizando Chrome).

   ![](assets/4-1.png)

1. Se abre una nueva ventana o ficha. Haga clic en **Añadir a Chrome**.

   ![](assets/five.png)

1. Haga clic en **Añadir extensión**.

   ![](assets/six.png)

1. Vuelve a Marketo. Añada la dirección URL de la página y haga clic en **Previsualización**.

   ![](assets/seven.png)

1. Se abre una nueva ventana/ficha que le permite previsualización de cómo se ve la campaña en un equipo de escritorio, un teléfono o una tablet.

   ![](assets/campaign-preview.png)

## Previsualización de una Campaña Web en la página de Campañas Web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Mientras observa la lista de sus campañas web, simplemente elija una campaña y haga clic en el icono **Previsualización**.

   ![](assets/web-campaigns-1-preview-hand.png)

   ¡Fácil!

## Previsualización de una Campaña Web en su sitio Web {#preview-a-web-campaign-on-your-website}

Cree un segmento de simulación de pruebas y una campaña.

1. Vaya a **Segmentos**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Haga clic en **Crear nuevo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Asigne un nombre al segmento.
1. En Comportamiento, arrastre Incluir páginas al lienzo. Añada el valor *sandbox=1*. Haga clic en Guardar y definir Campaña.

   ![](assets/segment.png)

1. En la página Establecer Campaña web, cambie el segmento de Destinatario al segmento de simulación de pruebas seleccionándolo en la lista.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Complete el elemento creativo de la campaña y haga clic en **Iniciar**.\
   ![](assets/click-launch.jpg)

1. Vaya a su sitio web, agregue el parámetro de URL &quot;?sandbox=1&quot; al final de la dirección URL. Ejemplo: [www.marketo.com?sandbox=1](https://www.marketo.com/?sandbox=1)
1. Consulte las reacciones de la campaña en su sitio web.

>[!NOTE]
>
>Las campañas solo reaccionan una vez durante una sesión de visitante. Para volver a ver la campaña, borre las cookies del explorador.

>[!NOTE]
>
>No se puede obtener una vista previa de las campañas de redireccionamiento. La única manera de probarlos es mediante un segmento de simulación de pruebas (que destinatario por páginas específicas - *sandbox=redirect*)

