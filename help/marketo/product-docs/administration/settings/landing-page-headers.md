---
description: 'Encabezados de página de aterrizaje: documentos de Marketo, documentación del producto'
title: Encabezados de la página de destino
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '131'
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
