---
unique-page-id: 4719332
description: Implementación de RTP JavaScript - Marketo Docs - Documentación del producto
title: Implementar el JavaScript de RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Implementar el JavaScript de RTP {#deploy-the-rtp-javascript}

Para generar y configurar su etiqueta RTP, siga las instrucciones de instalación a continuación

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta RTP. Vaya a **Configuración de la cuenta**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. En **Dominio** y **Configuración de dominio**, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copie y pegue la etiqueta de personalización web (RTP) en el sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta RTP JavaScript y péguela como el primer script en el encabezado de sus páginas, entre las `<head> </head>` etiquetas.

   Asegúrese de que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Para comprobar esto, haga clic con el botón derecho en la página de su sitio web. Vaya a Ver origen de página en un explorador web. Buscar: &quot;RTP&quot;.

1. Etiqueta de alternancia establecida en **ON**.

   Confirme que la opción Etiqueta está activada. Debería comenzar a ver el flujo de datos en la pestaña Organización.

   Ahora está configurado con la etiqueta RTP y listo para empezar [creación de segmentos](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) y campañas en tiempo real!

1. La etiqueta Verify está en todas las páginas.
