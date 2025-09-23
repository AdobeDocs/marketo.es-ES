---
unique-page-id: 4720125
description: 'Integración de RTP con Google Universal Analytics: documentos de Marketo, documentación del producto'
title: Integración de RTP con Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 4%

---

# Integrar RTP con [!DNL Google Universal Analytics] {#integrate-rtp-with-google-universal-analytics}

## Introducción {#intro}

Aproveche [!DNL Google Universal Analytics] (GUA) con los datos firmográficos y de personalización de [!DNL Marketo Real-Time Personalization] (RTP) para medir y analizar mejor sus esfuerzos de marketing en línea.

En esta publicación se explica cómo configurar e integrar la plataforma [!DNL Marketo Real-Time Personalization] (RTP) con cuentas de [!DNL Google Universal Analytics] (GUA). Los datos de RTP se pueden anexar a su cuenta de GUA, lo que le permite ver y ver el rendimiento de las organizaciones, industrias, firmográficos y segmentos de RTP que visitan su sitio web.

**[!DNL Google Universal Analytics]**

[!DNL Google Universal Analytics] con los datos de RTP le ofrece una mejor comprensión de cómo los usuarios B2B interactúan con el contenido en línea y ayuda a medir y obtener mejores resultados con sus campañas de personalización. [Más información sobre [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1).

>[!NOTE]
>
>**Solo Para Usuarios De Google Tag Manager**
>
>No es necesario realizar ninguna codificación ni configuración especial. Asegúrese de completar la siguiente lista de comprobación:
>
>* Las dimensiones RTP se han creado en [!DNL Google Universal Analytics]
>* La etiqueta [RTP está correctamente instalada en Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* La integración de [!DNL Google Universal Analytics] está habilitada en la configuración de cuenta de RTP
>* [[!DNL Google Universal Analytics] la etiqueta está configurada correctamente en Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* La etiqueta [Google Tag Manager está correctamente instalada en su sitio web](https://developers.google.com/tag-manager/quickstart)

## Configuración de dimensiones personalizadas en GUA {#set-up-custom-dimensions-in-gua}

1. En Google Analytics,

   1. Ir a **[!UICONTROL Administrador]**
   1. Seleccione la **[!UICONTROL cuenta].**
   1. Seleccione la **[!UICONTROL propiedad].**
   1. Seleccione **[!UICONTROL definiciones personalizadas]** y **[!UICONTROL dimensiones personalizadas]**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Añada una nueva dimensión personalizada. Haga clic en **[!UICONTROL +Nuevo Dimension personalizado]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Agregar las **[!UICONTROL dimensiones personalizadas] siguientes:**

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
>**Los nombres personalizados de Dimension** deben ser exactamente como se definen en la tabla anterior (de lo contrario, los paneles e informes personalizados de RTP en GUA no se mostrarán correctamente)

1. Agregar **[!UICONTROL Nombre]**. Seleccione el ámbito como **[!UICONTROL Sesión]**. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

La lista de Dimension personalizados debería tener este aspecto.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una vez que haya activado las dimensiones personalizadas en GUA, vaya a la plataforma RTP para habilitar estas dimensiones dentro de RTP.

## Activación de la integración de GUA en su cuenta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. En la plataforma RTP, vaya a **[!UICONTROL Configuración de la cuenta].**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **[!UICONTROL Configuración de la cuenta]**, haga clic en **[!UICONTROL Dominio]**.
1. En **[!UICONTROL Analytics]**, haga clic en **[!UICONTROL Google Universal Analytics]**.
1. Active **[!UICONTROL 1} las dimensiones y eventos personalizados relevantes para anexar estos datos de RTP a]**.[!DNL Google Universal Analytics]
1. Escriba el **[!UICONTROL número de índice]** de la dimensión alineado con el número de índice en GUA.
1. Haga clic en **[!UICONTROL Guardar]**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>El número de índice del Dimension personalizado se encuentra en GUA, en Dimensiones personalizadas.
>
>Ejemplo: Número de índice del sector RTP igual a 1, Número de índice de la organización RTP igual a 2.

## Eliminación de paneles antiguos en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En Google Analytics. Ir a **[!UICONTROL Informes].**
1. Haga clic en **[!UICONTROL Paneles].**
1. Seleccionar un **[!UICONTROL panel]** (rendimiento de RTP B2B o RTP)
1. Haga clic en **[!UICONTROL Eliminar panel]**.

![](assets/image2014-11-29-11-3a42-3a55.png)
