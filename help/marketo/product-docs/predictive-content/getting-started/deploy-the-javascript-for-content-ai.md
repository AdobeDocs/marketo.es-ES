---
unique-page-id: 11385053
description: Implementar JavaScript para Content-AI - Marketo Docs - Documentación del producto
title: Implementar JavaScript para Content-AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Implementar JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

Para utilizar contenido predictivo, debe generar y configurar la etiqueta RTP (Personalización web).

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de contenido predictivo. Vaya a **Configuración de la cuenta**.

   ![](assets/settings-dropdown-account-hands.png)

1. En **Configuración de dominio**, localice el dominio relevante y haga clic en **Generar etiqueta**.

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta de personalización web en el HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de Personalización web y péguela como la primera secuencia de comandos en el encabezado de las páginas, entre las etiquetas `<head> </head>`. Consulte las [instrucciones de implementación más detalladas aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Para ello, haga clic con el botón derecho en la página del sitio web. Vaya a **Origen de página de Vista** en un explorador Web. Buscar: &quot;RTP&quot;.

1. Confirme que el alternador de etiquetas está establecido en **ON**.
