---
unique-page-id: 10092925
description: 'Previsualización y prueba de una campaña web: documentos de Marketo, documentación del producto'
title: Previsualización y prueba de una campaña web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Previsualización y prueba de una campaña web {#preview-and-test-a-web-campaign}

Este artículo muestra diferentes formas de previsualizar una campaña web y también cómo probarla con un segmento de zona protegida activo en el sitio web.

>[!NOTE]
>
>La vista previa solo muestra el aspecto que tendrá la campaña en el sitio elegido. Los vínculos y widgets no funcionarán para evitar clics o vistas erróneos en el análisis.

## Vista previa de una campaña web en la página de creación {#preview-a-web-campaign-on-the-creation-page}

1. Ir a **Campañas web**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Clic **Creación de una nueva campaña web** o el icono para editar una campaña existente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. En Vista previa en el sitio, agregue la dirección URL de la página y haga clic en **Previsualizar**. Se abre una nueva ventana/pestaña con la vista previa de la campaña.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Clic **Compartir** para abrir un correo electrónico con una dirección URL fija de la vista previa de la campaña.

   >[!NOTE]
   >
   >También tiene la opción de instalar un complemento del explorador (ya sea [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) para obtener la mejor experiencia al previsualizar la campaña. Consulte la sección siguiente.

## Vista previa de una campaña web en la página de creación mediante el complemento del explorador {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Siga los pasos 1 y 2 de la sección anterior.

1. Haga clic en el vínculo al complemento del explorador (en este caso se utiliza Chrome).

   ![](assets/4-1.png)

1. Se abre una nueva ventana/pestaña. Clic **Añadir a Chrome**.

   ![](assets/five.png)

1. Clic **Añadir extensión**.

   ![](assets/six.png)

1. Vuelva a Marketo. Añada la dirección URL de la página y haga clic en **Previsualizar**.

   ![](assets/seven.png)

1. Se abre una nueva ventana o pestaña que le permite obtener una vista previa del aspecto de la campaña en un escritorio, un teléfono o una tableta.

   ![](assets/campaign-preview.png)

## Vista previa de una campaña web en la página de campañas web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Al ver la lista de sus campañas web, simplemente elija una campaña y haga clic en **Previsualizar** icono.

   ![](assets/web-campaigns-1-preview-hand.png)

   ¡Tranquilo!

## Vista previa de una campaña web en el sitio web {#preview-a-web-campaign-on-your-website}

Cree un segmento y una campaña de zona protegida.

1. Ir a **Segmentos**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Clic **Crear nuevo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Asigne un nombre al segmento.

1. En Comportamiento, arrastre Incluir páginas al lienzo. Añada el valor &#42;sandbox=1&#42;. Clic **Guardar y definir la campaña**.

   ![](assets/segment.png)

1. En la página Definir campaña web, cambie el segmento de Target al segmento de zona protegida seleccionándolo en la lista.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Complete el elemento creativo de la campaña y haga clic **Launch**.

   ![](assets/click-launch.jpg)

1. Vaya al sitio web y añada el parámetro de URL &quot;?sandbox=1&quot; al final de la dirección URL. Ejemplo: `www.marketo.com?sandbox=1`.

1. Consulte la reacción de la campaña en el sitio web.

>[!NOTE]
>
>Las campañas reaccionan solo una vez durante una sesión del visitante. Para volver a ver la campaña, borre las cookies del explorador.

>[!NOTE]
>
>No se pueden previsualizar las campañas de redireccionamiento. La única manera de probarlos es usando un segmento de zona protegida (segmentado por páginas específicas: &#42;sandbox=redirect&#42;)
