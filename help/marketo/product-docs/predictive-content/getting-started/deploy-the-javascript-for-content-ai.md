---
unique-page-id: 11385053
description: 'Implementación de JavaScript para la inteligencia artificial aplicada al contenido: documentos de Marketo, documentación del producto'
title: Implementación de JavaScript para la inteligencia artificial aplicada al contenido
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Implementación de JavaScript para la inteligencia artificial aplicada al contenido {#deploy-the-javascript-for-content-ai}

Para utilizar contenido predictivo, debe generar y configurar la etiqueta RTP (Web Personalization).

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de Predictive Content. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   ![](assets/settings-dropdown-account-hands.png)

1. En **[!UICONTROL Configuración del dominio]**, busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta Web Personalization en la HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de Web Personalization y péguela como el primer script en el encabezado de sus páginas, entre las etiquetas `<head> </head>`. Vea [instrucciones de implementación más detalladas aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las de aterrizaje y los subdominios. Para comprobarlo, haga clic con el botón derecho en la página del sitio web. Vaya a **[!UICONTROL Ver página Source]** en un navegador web. Buscar: &quot;RTP&quot;.

1. Confirme que la opción Etiqueta esté establecida en **[!UICONTROL ON]**.
