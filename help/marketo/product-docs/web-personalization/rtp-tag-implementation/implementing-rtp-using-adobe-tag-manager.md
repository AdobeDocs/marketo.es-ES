---
unique-page-id: 4720218
description: Obtenga información acerca de la implementación de rtp con el administrador de etiquetas de Adobe en Marketo Engage, incluida la implementación de rtp con etiquetas de Adobe. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP mediante Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/aIrAA9GHOTh0EkaSgVYq4veUQH-0uNbIfUvWfV825fQ
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 5%

---

# Implementación de RTP mediante Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Inicie sesión en su cuenta de RTP.

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. En [!UICONTROL Dominio], busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Inicie sesión en su cuenta de [!DNL Dynamic Tag Manager] ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Ir a **[!UICONTROL Tablero].** Haga clic en la propiedad web correspondiente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vaya a **[!UICONTROL Reglas]** y haga clic en **[!UICONTROL Crear nueva regla]**.

1. Complete lo siguiente

   1. [!UICONTROL Nombre]: **Marketo RTP**
   1. [!UICONTROL Condiciones] (contraer) : regla de Déclencheur en - **[!UICONTROL Parte superior de la página]**
   1. [!UICONTROL Javascript] (contraer): haga clic en **[!UICONTROL Agregar nuevo script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Llame a la nueva etiqueta: **Marketo RTP Tag**

1. Quite el siguiente código de la [!UICONTROL etiqueta RTP]

   * `<script type='text/javascript'>`
   * `</script>`

1. Pegue la etiqueta RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Asegúrese de quitar todas las etiquetas y dejar solamente el script en sí (no `<script type='text/javascript'>` , `</script>` )

1. Haga clic en **[!UICONTROL Guardar código]** en el editor de scripts y en **[!UICONTROL Guardar regla]** en el editor de reglas.

1. En el panel Reglas, busque la regla de carga de página RTP de Marketo y, en la lista desplegable **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Activar reglas]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Compruebe]** que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Puede hacerlo haciendo clic con el botón derecho en las páginas del sitio web. Vaya a **[!UICONTROL Inspeccionar elemento]**, haga clic en **[!UICONTROL Red]**, Buscar: **RTP**.
