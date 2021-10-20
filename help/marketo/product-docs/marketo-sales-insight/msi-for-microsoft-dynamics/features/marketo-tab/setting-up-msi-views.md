---
description: 'Configuración de vistas MSI: documentos de Marketo: documentación del producto'
title: Configuración de vistas MSI
hide: true
hidefromtoc: true
source-git-commit: 42ddb44100a041a09ff4a68c02ccf6aabb2d953e
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configuración de vistas MSI {#setting-up-msi-views}

Al instalar el complemento de perspectiva de ventas en Dynamics, se añaden automáticamente las mejores apuestas y los paneles relacionados en el mapa del sitio. Si, por alguna razón, no se agregan los tableros, así es como se los agregan manualmente.

1. En Dynamics, haga clic en el icono de engranaje y seleccione **Configuración avanzada** en la lista desplegable .

1. En la parte superior izquierda de la pantalla, haga clic en **Configuración**. En Personalización , elija **Personalizaciones**.

1. Haga clic en **Personalizar el sistema**.

1. En el árbol de la izquierda, haga clic en **Extensiones de cliente** y doble clic **Mapa del sitio**.

1. Haga clic en la flecha derecha para ir a la página siguiente. En Ventas, debería ver Marketo. Si no es así, asegúrese de que ha importado el paquete correctamente.

   >[!NOTE]
   >
   >En Marketo debe tener: Mejores apuestas, Mi correo electrónico, Actividad web y Actividad web anónima. Si falta alguno de esos tableros, haga clic en el signo + situado encima de Ventas y agréguelos como una subzona.

1. Haga clic en un tablero para seleccionarlo. En la columna de la derecha, introduzca la información correspondiente a continuación para cada una de ellas. Puede ignorar cualquier categoría que no aparezca en la lista.

   **Mejores apuestas**</br>
URL: MainviewBestbets.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Título: Mejores apuestas

   **Mi correo electrónico**</br>
URL: mkt_/MainViewMyEmail.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketing_myemail</br>
Título: Mi correo electrónico

   **Actividad web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Título: Actividad web

   **Actividad web anónima**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Título: Actividad web anónima

1. Haga clic en **Guardar** cuando haya terminado.
