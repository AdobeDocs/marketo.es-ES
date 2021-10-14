---
unique-page-id: 10092925
description: Vista previa y prueba de una campaña web - Documentos de Marketo - Documentación del producto
title: Vista previa y prueba de una campaña web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Vista previa y prueba de una campaña web {#preview-and-test-a-web-campaign}

Este artículo muestra distintas formas de obtener una vista previa de una campaña web y también cómo probarla con un segmento de simulación de pruebas en directo en el sitio web.

>[!NOTE]
>
>La vista previa solo muestra el aspecto que tendrá la campaña en el sitio elegido. Los vínculos y las utilidades no funcionarán como para evitar clics o vistas incorrectas en Analytics.

## Vista preliminar de una campaña web en la página de creación {#preview-a-web-campaign-on-the-creation-page}

1. Vaya a **Campañas web**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Haga clic en **Crear nueva campaña web** o en el icono para editar una campaña existente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. En Vista previa en el sitio, añada la dirección URL de la página y haga clic en **Vista previa**. Se abre una nueva ventana o pestaña que muestra la vista previa de la campaña.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Haga clic en **Compartir** para abrir un correo electrónico con una dirección URL fija de la vista previa de la campaña.

   >[!NOTE]
   >
   >También tiene la opción de instalar un complemento del explorador ([Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) para obtener la mejor experiencia y obtener una vista previa de la campaña. Consulte la siguiente sección.

## Vista preliminar de una campaña web en la página de creación mediante el complemento del explorador {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Siga los pasos 1 y 2 de la sección anterior.

1. Haga clic en el vínculo al complemento del explorador (en este caso, estamos usando Chrome).

   ![](assets/4-1.png)

1. Se abre una nueva ventana o pestaña. Haga clic en **Agregar a Chrome**.

   ![](assets/five.png)

1. Haga clic en **Agregar extensión**.

   ![](assets/six.png)

1. Vuelva a Marketo. Añada la dirección URL de la página y haga clic en **Preview**.

   ![](assets/seven.png)

1. Se abre una nueva ventana o pestaña que permite obtener una vista previa del aspecto de la campaña en un escritorio, teléfono o tableta.

   ![](assets/campaign-preview.png)

## Vista preliminar de una campaña web en la página Campañas web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Al consultar la lista de sus campañas web, simplemente elija una campaña y haga clic en el icono **Preview**.

   ![](assets/web-campaigns-1-preview-hand.png)

   ¡Fácil!

## Vista preliminar de una campaña web en el sitio web {#preview-a-web-campaign-on-your-website}

Cree un segmento y una campaña de entorno limitado.

1. Vaya a **Segments**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Haga clic en **Crear nuevo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Asigne un nombre al segmento.

1. En Comportamiento, arrastre Incluir páginas al lienzo. Agregue el valor *sandbox=1*. Haga clic en **Guardar y definir campaña**.

   ![](assets/segment.png)

1. En la página Definir campaña web , cambie el segmento de destino al segmento de entorno limitado seleccionándolo en la lista.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Complete el elemento creativo de la campaña y haga clic en **Launch**.

   ![](assets/click-launch.jpg)

1. Vaya a su sitio web, añada el parámetro de URL &quot;?sandbox=1&quot; al final de la dirección URL. Ejemplo: `www.marketo.com?sandbox=1`.

1. Consulte la reacción de la campaña en su sitio web.

>[!NOTE]
>
>Las campañas solo reaccionan una vez durante una sesión de visitante. Para volver a ver la campaña, borre las cookies del explorador.

>[!NOTE]
>
>No se puede obtener una vista previa de las campañas de redireccionamiento. La única forma de probarlos es mediante un segmento de simulación de pruebas (que se orienta a páginas específicas: *sandbox=redirect*)
