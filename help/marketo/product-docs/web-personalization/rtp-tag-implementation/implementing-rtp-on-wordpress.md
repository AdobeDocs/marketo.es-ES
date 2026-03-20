---
unique-page-id: 4720149
description: Obtenga información acerca de la implementación de rtp en wordpress en Marketo Engage, incluida la implementación de rtp en dnl wordpress. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP en Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 2%

---

# Implementando RTP en [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Para implementar su [!UICONTROL etiqueta RTP], siga las instrucciones de instalación a continuación:

1. Abra el archivo **header.php** de su **[!DNL WordPress]tema**.

   Puede usar un cliente FTP para acceder al servidor o editar los archivos de tema directamente desde el panel [!DNL WordPress]. El editor de archivos se encuentra en la ficha **[!UICONTROL Aspecto]** del menú de la barra lateral.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. En la lista de archivos de plantilla a la derecha del editor de texto, busque **header.php** y ábralo.

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. En [!UICONTROL Dominio], busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copie la etiqueta RTP JavaScript y péguela en las plantillas de sitio web.

   a. Asegúrese de que sea el primer script en el encabezado de la página, entre las etiquetas **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Haz clic en **[!UICONTROL Actualizar archivo]** para el archivo header.php.

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   a. Puede hacerlo haciendo clic con el botón derecho en la página del sitio web. Vaya a **[!UICONTROL Ver página Source].** busque **RTP** para encontrar la etiqueta.
