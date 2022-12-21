---
unique-page-id: 11385053
description: 'Implementación de JavaScript para contenido-IA: Marketo Docs: documentación del producto'
title: Implementación de JavaScript para Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Implementación de JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

Para utilizar contenido predictivo, debe generar y configurar la etiqueta RTP (personalización web).

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de contenido predictivo. Vaya a **Configuración de la cuenta**.

   ![](assets/settings-dropdown-account-hands.png)

1. En **Configuración de dominio**, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta Personalización web en el HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de personalización web y péguela como el primer script en el encabezado de sus páginas, entre las `<head> </head>` etiquetas. Consulte más información [instrucciones de implementación aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Para comprobar esto, haga clic con el botón derecho en la página de su sitio web. Vaya a **Ver origen de página** en un explorador web. Buscar: &quot;RTP&quot;.

1. Confirme que la opción Etiqueta está establecida en **ON**.
