---
unique-page-id: 4719332
description: Implementación de RTP JavaScript - Documentos de Marketo - Documentación del producto
title: Implementación de RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Implementación de RTP JavaScript {#deploy-the-rtp-javascript}

Para generar y configurar su etiqueta RTP, siga las instrucciones de instalación que se indican a continuación

## Generar etiqueta {#generate-tag}

1. Inicie sesión en su cuenta de RTP. Ir a **Configuración de cuenta**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. Entrada **Dominio** y **Configuración del dominio**, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copie y pegue la etiqueta de personalización web (RTP) en el sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta JavaScript de RTP y péguela como la primera secuencia de comandos en el encabezado de sus páginas, entre las etiquetas `<head> </head>` etiquetas.

   Asegúrese de que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Para comprobarlo, haga clic con el botón derecho en la página del sitio web. Vaya a Ver origen de página en un explorador web. Buscar: &quot;RTP&quot;.

1. Conmutador de etiquetas establecido en **ACTIVADO**.

   Confirme que la opción Etiqueta esté activada. Debería empezar a ver el flujo de datos en la pestaña de la organización.

   Ya está configurado con la etiqueta RTP y listo para iniciarse [creación de segmentos](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) y campañas en tiempo real.

1. Compruebe que la etiqueta está en todas las páginas.
