---
unique-page-id: 4720125
description: 'Integración de RTP con Google Universal Analytics: documentos de Marketo, documentación del producto'
title: Integración de RTP con Universal Analytics de Google
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Integración de RTP con Universal Analytics de Google {#integrate-rtp-with-google-universal-analytics}

## Introducción {#intro}

Aproveche Google Universal Analytics (GUA) con los datos firmográficos y de personalización de Marketo Real-Time Personalization (RTP) para medir y analizar mejor sus esfuerzos de marketing en línea.

En esta publicación se explica cómo configurar e integrar la plataforma Marketo Real-Time Personalization (RTP) con cuentas de Google Universal Analytics (GUA). Los datos de RTP se pueden anexar a su cuenta de GUA, lo que le permite ver y ver el rendimiento de las organizaciones, industrias, firmográficos y segmentos de RTP que visitan su sitio web.

**Google Universal Analytics**

Los datos de Google Universal Analytics con RTP le permiten comprender mejor cómo los usuarios de B2B interactúan con el contenido en línea, y le ayudan a medir y obtener mejores resultados con sus campañas de personalización. [Más información sobre Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Solo Para Usuarios De Google Tag Manager**
>
>No es necesario realizar ninguna codificación ni configuración especial. Asegúrese de completar la siguiente lista de comprobación:
>
>* Las dimensiones RTP se crean en Google Universal Analytics
>* La etiqueta [RTP está correctamente instalada en Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* La integración de Google Universal Analytics está habilitada en la configuración de cuenta de RTP
>* [La etiqueta de Google Universal Analytics está configurada correctamente en el Administrador de etiquetas de Google](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* La etiqueta [Google Tag Manager está correctamente instalada en su sitio web](https://developers.google.com/tag-manager/quickstart)

## Configuración de Dimension personalizados en GUA {#set-up-custom-dimensions-in-gua}

1. En Google Analytics,

   1. Ir a **Administrador**
   1. Seleccione la **cuenta.**
   1. Seleccione la **propiedad.**
   1. Seleccione **Definiciones personalizadas** y **Dimension personalizados**.

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Añada una nueva dimensión personalizada. Haga clic en **+Nuevo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Agregar los siguientes **Dimension personalizados:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nombre de Dimension personalizado</strong></p></td> 
   <td><p><strong>Ámbito</strong></p></td> 
   <td><p><strong>Activo</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organización</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industria</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Category</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Grupo RTP</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Los nombres de Dimension personalizados** deben ser exactamente como se definen en la tabla anterior (de lo contrario, los paneles e informes personalizados de RTP en GUA no se mostrarán correctamente)

1. Agregar **Nombre**. Seleccione el ámbito como **Sesión**. Haga clic en **Crear**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

La lista de Dimension personalizados debería tener este aspecto.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una vez que haya activado los Dimension personalizados en GUA, vaya a la plataforma RTP para habilitar estas dimensiones dentro de RTP.

## Activación de la integración de GUA en su cuenta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. En la plataforma RTP, vaya a **Configuración de la cuenta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **Configuración de la cuenta**, haga clic en **Dominio**.
1. En **Analytics**, haga clic en **Google Universal Analytics**.
1. Active **1&rbrace; los Dimension personalizados y eventos relevantes para anexar estos datos de RTP a Google Universal Analytics.**
1. Escriba el **número de índice** de la dimensión alineado con el número de índice en GUA.
1. Haga clic en **Guardar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>El número de índice del Dimension personalizado se encuentra en GUA, en Dimension personalizados.
>
>Ejemplo: Número de índice del sector RTP igual a 1, Número de índice de la organización RTP igual a 2.

## Eliminación de paneles antiguos en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En Google Analytics. Ir a **Informes.**
1. Haga clic en **Paneles.**
1. Seleccionar un **panel** (rendimiento de RTP B2B o RTP)
1. Haga clic en **Eliminar panel**.

![](assets/image2014-11-29-11-3a42-3a55.png)
