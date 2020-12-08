---
unique-page-id: 11385053
description: Implementar JavaScript para Content-AI - Marketo Docs - Documentación del producto
title: Implementar JavaScript para Content-AI
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Implementar JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>Según la fecha de compra, la suscripción de marketing puede incluir Contenido`<sup>AI</sup>`predictivo de marketing o Contenido. Para aquellos que utilizan contenido predictivo, Marketing`<sup>AI</sup>` está activando las funciones de Content Analytics hasta el 30 de abril de 2018. Para mantener estas funciones más allá de esa fecha, póngase en contacto con el administrador de éxito del cliente de Marketing to para actualizar a Contenido`<sup>AI</sup>`de marketing.

Para utilizar contenido predictivo, debe generar y configurar el RTP (Personalización web) `tag.`

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de contenido predictivo. Vaya a Configuración **de cuenta**.

   ![](assets/settings-dropdown-account-hands.png)

1. En Configuración **** de dominio, localice el dominio relevante y haga clic en **Generar etiqueta.**

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta de personalización web en el HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de Personalización web y péguela como la primera secuencia de comandos en el encabezado de las páginas, entre las `<head> </head>` etiquetas. Consulte las instrucciones [de implementación más detalladas aquí](http://docs.marketo.com/display/docs/rtp+tag+implementation) [.](http://pages2.marketo.com/rtp-implementation.html)

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Marque esta opción haciendo clic con el botón secundario en la `website’s` página. Vaya a Origen **de página de** Vista en un explorador Web. Buscar: &quot;RTP&quot;.
1. Confirme que la opción de alternancia de etiquetas está **activada**.

