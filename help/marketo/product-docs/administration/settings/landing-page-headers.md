---
description: Cómo personalizar encabezados HTTP para dominios de páginas de aterrizaje, incluidos Strict-Transport-Security y X-Frame-Options.
title: Encabezados de la página de destino
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 147
ht-degree: 4%

---

# Encabezados de la página de destino {#landing-page-headers}

Siga los pasos a continuación para personalizar algunos de los encabezados HTTP de los dominios de la página de aterrizaje.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/landing-page-headers-1.png)

1. Haga clic en **[!UICONTROL Páginas de aterrizaje]**.

   ![](assets/landing-page-headers-2.png)

1. Haga clic en **[!UICONTROL Editar]** junto a los encabezados HTTP de la página de aterrizaje.

   ![](assets/landing-page-headers-3.png)

1. Elija la configuración que desee y haga clic en **[!UICONTROL Guardar]** cuando haya terminado.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Utilice esto para garantizar que las conexiones a las páginas de destino siempre se proporcionen a través de HTTPS (solo debe configurarse para suscripciones con páginas de destino protegidas por SSL)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Permite definir si los recursos alojados por Marketo Engage se pueden incrustar o no en páginas web externas</td>
 </tr>
</table>

>[!CAUTION]
>
>Es importante revisar esta configuración con su equipo de TI para determinar en qué política de su organización debe configurarse. Una configuración incorrecta puede impedir que algunos visitantes accedan a sus páginas de aterrizaje.
