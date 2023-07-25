---
unique-page-id: 11385053
description: 'Implementación de JavaScript para la inteligencia artificial aplicada al contenido: documentos de Marketo, documentación del producto'
title: Implementación de JavaScript para la inteligencia artificial aplicada al contenido
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Implementación de JavaScript para la inteligencia artificial aplicada al contenido {#deploy-the-javascript-for-content-ai}

Para utilizar contenido predictivo, debe generar y configurar la etiqueta RTP (Web Personalization).

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de Predictive Content. Ir a **Configuración de cuenta**.

   ![](assets/settings-dropdown-account-hands.png)

1. Entrada **Configuración del dominio**, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/generate-tag.png)

1. Copie y pegue la etiqueta Web Personalization en el HTML del sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de Web Personalization y péguela como el primer script en el encabezado de sus páginas, entre las etiquetas `<head> </head>` etiquetas. Ver más detalles [instrucciones de implementación aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Compruebe que la etiqueta aparece en todas las páginas, incluidas las de aterrizaje y los subdominios. Para comprobarlo, haga clic con el botón derecho en la página del sitio web. Ir a **Ver origen de página** en un explorador web. Buscar: &quot;RTP&quot;.

1. Confirme que la opción Etiqueta esté configurada como. **ACTIVADO**.
