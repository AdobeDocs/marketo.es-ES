---
unique-page-id: 11385053
description: Implementar JavaScript para Content-AI - Marketo Docs - Documentación del producto
title: Implementar JavaScript para Content-AI
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Implementar JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>Según la fecha de compra, la suscripción de marketing puede incluir Contenido predictivo de marketing o Contenido`<sup>AI</sup>`. Para aquellos que utilizan contenido predictivo, Marketing está activando las funciones de análisis de contenido`<sup>AI</sup>` hasta el 30 de abril de 2018. Para mantener estas funciones más allá de esa fecha, póngase en contacto con el administrador de éxito del cliente de Marketing to para actualizar a Contenido de marketing`<sup>AI</sup>`.

Para utilizar contenido predictivo, debe generar y configurar el RTP (Personalización Web) `tag.`

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de contenido predictivo. Vaya a **Configuración de la cuenta**.

   ![](assets/settings-dropdown-account-hands.png)

1. En **Configuración de dominio**, localice el dominio relevante y haga clic en **Generar etiqueta.**

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta de personalización web en el HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de Personalización web y péguela como la primera secuencia de comandos en el encabezado de las páginas, entre las etiquetas `<head> </head>`. Consulte las [instrucciones de implementación más detalladas aquí](https://docs.marketo.com/display/docs/rtp+tag+implementation) [.](https://pages2.marketo.com/rtp-implementation.html)

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Marque esto haciendo clic con el botón derecho en su página `website’s`. Vaya a **Origen de página de Vista** en un explorador Web. Buscar: &quot;RTP&quot;.
1. Confirme que el alternador de etiquetas está establecido en **ON**.

