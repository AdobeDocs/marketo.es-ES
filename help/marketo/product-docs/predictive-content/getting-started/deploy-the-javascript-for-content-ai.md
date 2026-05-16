---
unique-page-id: 11385053
description: Obtenga información sobre cómo generar y colocar la etiqueta RTP Web Personalization para contenido predictivo. Cópielo en el encabezado de la página, verifique la cobertura y confirme que la opción permanece activada.
title: Implementar JavaScript para Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 7%

---

# Implementar JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

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
