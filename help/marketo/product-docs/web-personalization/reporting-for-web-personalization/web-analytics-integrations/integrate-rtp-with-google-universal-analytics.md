---
unique-page-id: 4720125
description: 'Integración de RTP con Google Universal Analytics: Marketo Docs: documentación del producto'
title: Integración de RTP con Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Integración de RTP con Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introducción {#intro}

Aproveche Google Universal Analytics (GUA) con los datos de personalización y firmografía de la personalización en tiempo real (RTP) de Marketo para medir y analizar mejor sus esfuerzos de marketing en línea.

En este artículo se explica cómo configurar e integrar la plataforma de personalización en tiempo real (RTP) de Marketo con cuentas de Google Universal Analytics (GUA). Los datos de RTP se pueden anexar a su cuenta de GUA, lo que le permite ver y ver el rendimiento de las organizaciones, industrias, firmografías y segmentos de RTP que visitan su sitio web.

**Google Universal Analytics**

Google Universal Analytics con los datos de RTP le permite comprender mejor cómo interactúan los usuarios de B2B con el contenido en línea y ayudarle a medir y obtener mejores resultados de sus campañas de personalización. [Más información sobre Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

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
>* [La etiqueta Administrador de etiquetas de Google está instalada correctamente en el sitio web](https://developers.google.com/tag-manager/quickstart)


## Configuración de Dimension personalizados en GUA {#set-up-custom-dimensions-in-gua}

1. En los Google Analytics,

   1. Vaya a **Administrador**
   1. Seleccione el **Cuenta.**
   1. Seleccione el **Propiedad.**
   1. Select **Definiciones personalizadas** y **Dimension personalizados**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Añada una nueva dimensión personalizada. Haga clic en **+Nuevo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Agregue lo siguiente **Dimension personalizados:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nombre de Dimension personalizado</strong></p></td> 
   <td><p><strong>Ámbito</strong></p></td> 
   <td><p><strong>Activo</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Organización RTP</strong></p></td> 
   <td><p>Sesión</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
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
>**Nombres de Dimension personalizados** debe ser exactamente como se define en la tabla anterior (de lo contrario, los paneles RTP personalizados y los informes en GUA no se mostrarán correctamente)

1. Agregue la variable **Nombre**. Seleccione el ámbito como **Sesión**. Haga clic en **Crear**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

La lista de Dimension personalizados debería tener este aspecto.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una vez que haya activado los Dimension personalizados en GUA, vaya a la plataforma RTP para habilitar estas dimensiones dentro de RTP.

## Active la integración de GUA en su cuenta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. En la plataforma RTP, vaya a **Configuración de la cuenta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **Configuración de la cuenta**, haga clic en **Dominio**.
1. En **Analytics**, haga clic en **Google Universal Analytics**.
1. Turn **Activado** los Dimension y eventos personalizados relevantes para anexar estos datos de RTP a Google Universal Analytics.
1. Introduzca la variable **Número de índice** de la dimensión alineada con el número de índice en GUA.
1. Haga clic en **Guardar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>El número de índice del Dimension personalizado se puede encontrar en GUA en Dimension personalizados.
>
>Ejemplo: El número de índice RTP-Industry es igual a 1, el número de índice RTP-Organization es igual a 2.

## Eliminar tableros antiguos en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En los Google Analytics. Vaya a **Informes.**
1. Haga clic en **Tableros.**
1. Seleccione un **Panel** (Rendimiento RTP B2B o RTP)
1. Haga clic en **Eliminar tablero**.

![](assets/image2014-11-29-11-3a42-3a55.png)
