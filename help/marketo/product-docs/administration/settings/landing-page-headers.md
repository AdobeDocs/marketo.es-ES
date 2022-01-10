---
description: 'Encabezados de página de aterrizaje: Documentos de Marketo: Documentación del producto'
title: Encabezados de página de aterrizaje
hide: true
hidefromtoc: true
source-git-commit: 921c3279b53bc18ac753b1e3f0672a70fe11abe7
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Landing Page Headers {#landing-page-headers}

Siga los pasos a continuación para personalizar algunos de los encabezados HTTP de los dominios de la página de aterrizaje.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/landing-page-headers-1.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/landing-page-headers-2.png)

1. Haga clic en **Editar** junto a Encabezados HTTP de la página de aterrizaje.

   ![](assets/landing-page-headers-3.png)

1. Elija la configuración que desee y haga clic en **Guardar** cuando haya terminado.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Utilice esto para garantizar que las conexiones a las páginas de aterrizaje siempre se proporcionen a través de HTTPS (solo debe establecerse para suscripciones con páginas de aterrizaje seguras mediante SSL)</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>Lets you define whether or not Marketo Engage hosted assets can be embedded in external web pages</td>
 </tr>
</table>

>[!CAUTION]
>
>Es importante revisar esta configuración con su equipo de TI para determinar en qué debe configurarse la política de su organización. Incorrect settings can prevent some visitors from accessing your Landing Pages.
