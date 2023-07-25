---
description: Configuración de vistas MSI - Documentos de Marketo - Documentación del producto
title: Configurar vistas de MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configurar vistas de MSI {#setting-up-msi-views}

Al instalar el complemento de perspectiva de ventas en Dynamics, se agregan automáticamente los resultados más probables y los paneles relacionados en el mapa del sitio. Si, por alguna razón, no se agregan los paneles, así es como se agregan manualmente.

1. En Dynamics, haga clic en el icono de engranaje y seleccione **Configuración avanzada** de la lista desplegable.

1. En la parte superior izquierda de la pantalla, haga clic en **Configuración**. En Personalización, elija **Personalizaciones**.

1. Clic **Personalizar el sistema**.

1. En el árbol de la izquierda, haga clic en **Extensiones de cliente** y haga doble clic **Mapa del sitio**.

1. Haga clic en la flecha derecha para ir a la página siguiente. En Ventas debería ver Marketo. Si no lo tiene, asegúrese de importar el paquete correctamente.

   >[!NOTE]
   >
   >En Marketo, debería tener: Lo más probable, Mi correo electrónico, Actividad web y Actividad web anónima. Si falta alguno de estos tableros, haga clic en el signo + situado encima de Ventas y agréguelo como Subárea.

1. Haga clic en un tablero para seleccionarlo. En la columna de la derecha, introduzca la información correspondiente a cada uno de ellos. Puede ignorar cualquier categoría que no esté en la lista.

   **Recomendaciones**</br>
URL: MainviewBest.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Título: Resultados más probables

   **Mi correo electrónico**</br>
URL: mkt_/MainViewMyEmail.html</br>
Icono: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
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

1. Clic **Guardar** cuando termine.
