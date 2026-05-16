---
description: Obtenga información sobre cómo configurar vistas de MSI en Microsoft Dynamics. Configure las fichas y los datos de Marketo Sales Insight que aparecerán para los usuarios.
title: Configuración de las vistas de MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/PylFEW3pRnOwoIVF8hG2pKcFix5DO7ynWomXOfvy1e0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 264
ht-degree: 4%

---

# Configuración de las vistas de MSI {#setting-up-msi-views}

Al instalar el complemento [!DNL Sales Insight] en Dynamics, se agregan automáticamente [!DNL Best Bets] y los paneles relacionados en el mapa del sitio. Si, por alguna razón, no se agregan los paneles, así es como se agregan manualmente.

1. En Dynamics, haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración avanzada]** en la lista desplegable.

1. En la parte superior izquierda de la pantalla, haga clic en **[!UICONTROL Configuración]**. En Personalización elija **[!UICONTROL Personalizaciones]**.

1. Haga clic en **[!UICONTROL Personalizar el sistema]**.

1. En el árbol de la izquierda, haga clic en **[!UICONTROL Extensiones de cliente]** y haga doble clic en **[!UICONTROL Mapa del sitio]**.

1. Haga clic en la flecha derecha para ir a la página siguiente. En Ventas debería ver Marketo. Si no lo tiene, asegúrese de importar el paquete correctamente.

   >[!NOTE]
   >
   >En Marketo, debería tener: Lo más probable, Mi correo electrónico, Actividad web y Actividad web anónima. Si falta alguno de estos tableros, haga clic en el signo + situado encima de Ventas y agréguelo como Subárea.

1. Haga clic en un tablero para seleccionarlo. En la columna de la derecha, introduzca la información correspondiente a cada uno de ellos. Puede ignorar cualquier categoría que no esté en la lista.

   **resultados más probables**</br>
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

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.
