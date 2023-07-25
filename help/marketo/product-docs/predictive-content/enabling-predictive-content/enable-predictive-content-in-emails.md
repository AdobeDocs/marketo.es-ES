---
unique-page-id: 11385020
description: 'Habilitar contenido predictivo en correos electrónicos: documentos de Marketo, documentación del producto'
title: Habilitar contenido predictivo en correos electrónicos
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Habilitar contenido predictivo en correos electrónicos {#enable-predictive-content-in-emails}

Cree una o más imágenes en el correo electrónico predictivas y adapte la experiencia a cada destinatario.

>[!NOTE]
>
>Se recomienda habilitar más de cinco fragmentos de contenido por categoría y por fuente (correo electrónico, medios enriquecidos, barra) antes de probar y utilizar el contenido predictivo. Más contenido le ofrece un mejor resultado predictivo.

>[!PREREQUISITES]
>
>Antes de activar Contenido predictivo, debe:
>
>* **Preparación del contenido predictivo**
>
>   * [Editar contenido predictivo para correos electrónicos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} o
>   * [Editar contenido predictivo para medios enriquecidos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} o
>   * [Editar contenido predictivo para la barra de recomendaciones](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Aprobar un título para contenido predictivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Adición de contenido predictivo mediante el editor de correo electrónico 2.0 {#adding-predictive-content-using-the-email-editor}

1. Clic **Actividades de marketing**.

   ![](assets/one.png)

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/two.png)

1. Haga clic en la imagen que desee convertir en predictiva. Cuando aparezca el icono del engranaje, haga clic en él y seleccione **Habilitar ContentAI** (ContentAI es el nombre anterior de Predictive Content).

   ![](assets/three.png)

1. Para seleccionar una o varias categorías, haga clic en el icono **Categorías** , realice sus selecciones y haga clic en. **Aplicar**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Elegir categorías específicas o cambiar el diseño predictivo es opcional.

1. La imagen ahora es predictiva. Repita los pasos 3 y 4 para obtener imágenes adicionales (si lo desea).

   ![](assets/five.png)

1. Para previsualizar el correo electrónico, haga clic en **Previsualizar** en la esquina superior derecha.

   ![](assets/six.png)

1. Para ver diferentes imágenes posibles, haga clic en **Actualizar**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >La imagen no está seleccionada **_hasta que el destinatario abra el correo electrónico_**. Por lo tanto, lo que se ve en la vista previa es solo un ejemplo y no es necesariamente la imagen que ve el destinatario.

1. Una vez que haya terminado de previsualizar el correo electrónico, haga clic en **Previsualizar acciones** y seleccione. **Aprobar y cerrar**. O si todavía tiene que editar, haga clic en **Editar borrador** a la derecha.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Al enviar una muestra, se selecciona una imagen aleatoria.

Después de aprobar su correo electrónico, estará equipado con contenido predictivo y listo para enviar.

>[!CAUTION]
>
>Una vez que un destinatario abre el correo electrónico, las imágenes predictivas se bloquean. Si el contenido se elimina posteriormente, los destinatarios verán una imagen rota en la que se ha eliminado el contenido.

## Adición de contenido predictivo cuando no se utiliza el editor de correo electrónico 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Si no está utilizando un [Correo electrónico 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"} , añadir contenido predictivo al correo electrónico se puede hacer simplemente etiquetando una imagen en la plantilla como un elemento de imagen editable de Marketo.

Obtenga información acerca de [Sintaxis específica de Marketo aquí](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Este es un ejemplo del aspecto que debería tener el código (este es solo un ejemplo, no copie el código siguiente exactamente).

**Ejemplo**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
