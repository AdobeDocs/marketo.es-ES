---
unique-page-id: 11385020
description: 'Habilitar contenido predictivo en correos electrónicos: documentos de Marketo, documentación del producto'
title: Habilitar el contenido predictivo en correos electrónicos
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

---

# Habilitar el contenido predictivo en correos electrónicos {#enable-predictive-content-in-emails}

Cree una o más imágenes en el correo electrónico predictivas y adapte la experiencia a cada destinatario.

>[!NOTE]
>
>Se recomienda habilitar más de cinco fragmentos de contenido por categoría y por fuente (correo electrónico, medios enriquecidos, barra) antes de probar y utilizar el contenido predictivo. Más contenido le ofrece un mejor resultado predictivo.

>[!PREREQUISITES]
>
>Antes de activar Contenido predictivo, debe:
>
>* **Preparar el contenido predictivo**
>
>   * [Editar contenido predictivo para correos electrónicos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} o
>   * [Editar contenido predictivo para medios enriquecidos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} o
>   * [Editar contenido predictivo para la barra de recomendaciones](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Aprobar un título para contenido predictivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Adición de contenido predictivo mediante el editor de correo electrónico 2.0 {#adding-predictive-content-using-the-email-editor}

1. Haga clic en **[!UICONTROL Actividades de marketing]**.

   ![](assets/one.png)

1. Seleccione su correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/two.png)

1. Haga clic en la imagen que desee convertir en predictiva. Cuando aparezca el icono del engranaje, haga clic en él y seleccione **[!UICONTROL Habilitar ContentAI]** (ContentAI es el nombre anterior de Predictive Content).

   ![](assets/three.png)

1. Para seleccionar una o más categorías, haga clic en la lista desplegable **[!UICONTROL Categorías]**, realice sus selecciones y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Elegir categorías específicas o cambiar el diseño predictivo es opcional.

1. La imagen ahora es predictiva. Repita los pasos 3 y 4 para obtener imágenes adicionales (si lo desea).

   ![](assets/five.png)

1. Para obtener una vista previa del correo electrónico, haz clic en **[!UICONTROL Vista previa]** en la esquina superior derecha.

   ![](assets/six.png)

1. Para ver diferentes imágenes posibles, haga clic en **[!UICONTROL Actualizar]**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >La imagen no se selecciona **_hasta que el destinatario abra el correo electrónico_**. Por lo tanto, lo que se ve en la vista previa es solo un ejemplo y no es necesariamente la imagen que ve el destinatario.

1. Una vez que hayas terminado de obtener una vista previa del correo electrónico, haz clic en la lista desplegable **[!UICONTROL Acciones de vista previa]** y selecciona **[!UICONTROL Aprobar y cerrar]**. O si todavía tiene que editar, haga clic en **[!UICONTROL Editar borrador]** a la derecha.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Al enviar una muestra, se selecciona una imagen aleatoria.

Después de aprobar su correo electrónico, estará equipado con contenido predictivo y listo para enviar.

>[!CAUTION]
>
>Una vez que un destinatario abre el correo electrónico, las imágenes predictivas se bloquean. Si el contenido se elimina posteriormente, los destinatarios verán una imagen rota en la que se ha eliminado el contenido.

## Adición de contenido predictivo cuando no se utiliza el editor de correo electrónico 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Si no usas una plantilla de [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"}, puedes agregar contenido predictivo al correo electrónico simplemente etiquetando una imagen en tu plantilla como un elemento de imagen editable de Marketo.

Obtenga información acerca de la [sintaxis específica de Marketo aquí](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Este es un ejemplo del aspecto que debería tener el código (este es solo un ejemplo, no copie el código siguiente exactamente).

**Ejemplo**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">
<a><img style="border:10px solid red;"></a>
</div>
```
