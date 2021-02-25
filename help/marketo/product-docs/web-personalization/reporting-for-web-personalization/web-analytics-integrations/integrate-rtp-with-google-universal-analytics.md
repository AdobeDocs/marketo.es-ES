---
unique-page-id: 4720125
description: 'Integración de RTP con Google Universal Analytics: documentos de marketing: documentación del producto'
title: Integrar RTP con Google Universal Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# Integrar RTP con Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Aproveche Google Universal Analytics (GUA) con datos de personalización y firmografía de la Personalización en tiempo real (RTP) de Marketo para medir y analizar mejor sus esfuerzos de mercadotecnia en línea.

En este artículo se explica cómo configurar e integrar la plataforma de personalización en tiempo real (RTP) de Marketo con las cuentas de Google Universal Analytics (GUA). Los datos de RTP se pueden anexar a su cuenta de GUA permitiéndole realizar vistas y ver el rendimiento de organizaciones, industrias, firmografías y segmentos de RTP visitando su sitio web.

**Google Universal Analytics**

Google Universal Analytics con los datos de RTP le ofrece una mejor comprensión de cómo los usuarios de B2B interactúan con su contenido en línea y ayuda a medir y obtener mejores resultados con sus campañas de personalización. [Obtenga más información sobre Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Solo para usuarios de Administrador de etiquetas de Google**
>
>No es necesario codificar ni realizar ninguna configuración especial. Asegúrese de completar la siguiente lista de comprobación:
>
>* Las dimensiones RTP se crean en Google Universal Analytics
>* [La etiqueta RTP está instalada correctamente en el Administrador de etiquetas de Google](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* La integración de Google Universal Analytics está habilitada en la configuración de cuenta de RTP
>* [La etiqueta Google Universal Analytics está configurada correctamente en el Administrador de etiquetas de Google](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [La etiqueta del Administrador de etiquetas de Google se ha instalado correctamente en el sitio web](https://developers.google.com/tag-manager/quickstart)


## Configurar Dimension personalizados en GUA {#set-up-custom-dimensions-in-gua}

1. En Google Analytics,

   1. Vaya a **Administración**
   1. Seleccione la **cuenta.**
   1. Seleccione la **propiedad.**
   1. Seleccione **Definiciones personalizadas** y **Dimension personalizados**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Añada una nueva dimensión personalizada. Haga clic en **+Nuevo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Añada los siguientes **Dimension personalizados:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nombre del Dimension personalizado</strong></p></td> 
   <td><p><strong>Ámbito</strong></p></td> 
   <td><p><strong>Activo</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organization</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">xib</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">xib</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Categoría RTP</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">xib</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">xib</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Los** nombres de Dimension personalizados deben ser exactamente los definidos en la tabla anterior (de lo contrario, los informes y paneles RTP personalizados en GUA no se mostrarán correctamente)

1. Añada el **Nombre**. Seleccione el ámbito como **Sesión**. Haga clic en **Crear**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

La lista del Dimension personalizado debería tener este aspecto.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una vez activados los Dimension personalizados en GUA, vaya a la plataforma RTP para habilitar estas dimensiones dentro de RTP.

## Active la integración de GUA en su cuenta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. En la plataforma RTP, vaya a **Configuración de la cuenta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **Configuración de cuenta**, haga clic en **Dominio**.
1. En **Analytics**, haga clic en **Google Universal Analytics**.
1. Active **Los Dimension y Eventos personalizados relevantes para anexar estos datos de RTP a Google Universal Analytics.**
1. Introduzca el **número de índice** de la dimensión alineada con el número de índice en GUA.
1. Haga clic en **Guardar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>El número de índice del Dimension personalizado se encuentra en GUA, en Dimension personalizados.
>
>Ejemplo: El número de índice RTP-Industry es igual a 1, el número de índice de la organización RTP es igual a 2.

## Eliminar Paneles antiguos en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En Google Analytics. Vaya a **Sistema de informes.**
1. Haga clic en **Paneles.**
1. Seleccione un **Panel** (rendimiento RTP B2B o RTP)
1. Haga clic en **Eliminar Panel**.

![](assets/image2014-11-29-11-3a42-3a55.png)
