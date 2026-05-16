---
unique-page-id: 37355602
description: Obtenga información sobre cómo instalar y configurar Marketo Sales Insight en Microsoft Dynamics Online. Configure la solución para Dynamics Online.
title: Instalar y configurar Marketo Sales Insight en Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/ILDX3tNq-X0E6jVl5NY8EHw5lGwFEcgXh5yz4Q7zfhs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 469
ht-degree: 5%

---

# Instalar y configurar [!DNL Marketo Sales Insight] en [!DNL Microsoft Dynamics Online] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

[!DNL Marketo Sales Insight] es una herramienta fantástica para ofrecer a su equipo de ventas una &quot;ventana&quot; sobre la gran cantidad de datos que tiene el equipo de marketing. Así se instala y configura en [!DNL Microsoft Dynamics Online].

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de [!DNL Microsoft Dynamics CRM].

## Importar solución {#import-solution}

>[!NOTE]
>
>Si está usando la interfaz unificada, antes del paso 1 siguiente, haga clic en el icono Configuración en la esquina superior derecha y seleccione **[!UICONTROL Configuración avanzada]**.

1. En Microsoft Dynamics CRM, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. En Configuración, haga clic en **[!UICONTROL Personalizaciones]**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Haga clic en **[!UICONTROL Soluciones]**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado la solución de Marketo antes de continuar.

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. En la nueva ventana, haz clic en **[!UICONTROL Examinar]**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. En el equipo, busque e instale la solución que acaba de descargar.

1. Haga clic en **[!UICONTROL Next]**.

   ![](assets/seven.png)

1. Se cargará la solución. Si lo desea, puede ver el contenido del paquete. Haga clic en **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. No dude en descargar el archivo de registro y, a continuación, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. ¡Fantástico! Debería ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/eleven.png)

1. Haga clic en **[!UICONTROL Personalizar publicación]**.

   >[!NOTE]
   >
   >Asegúrese de habilitar la sincronización global [!DNL MS Dynamics].

## Conectar Marketo y [!DNL Sales Insight] {#connect-marketo-and-sales-insight}

Vinculemos su instancia de Marketo a [!DNL Sales Insight] en [!DNL Dynamics]. A continuación se muestra cómo:

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Inicie sesión en Marketo y vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. En la sección [!UICONTROL Sales Insight], haga clic en **[!UICONTROL Editar configuración de API]**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** y **[!UICONTROL API User Id]** para usarlos en un paso posterior. Escriba una clave secreta de API de su elección y haga clic en **[!UICONTROL Guardar]**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Los campos siguientes se deben sincronizar con Marketo para que _tanto el posible cliente como el contacto_ funcionen para [!DNL Sales Insight]:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. En [!DNL Microsoft Dynamics], ve a **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración de la API de Marketo]**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Escriba la información que tomó de Marketo anteriormente y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Habilitar sincronización {#enable-sync}

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/enable-one.png)

1. En Integración, seleccione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/enable-two.png)

1. Haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-three.png)

1. Haga clic en **[!UICONTROL Editar]** junto a [!UICONTROL Detalles de sincronización de campos].

   ![](assets/enable-four.png)

1. Esto _seleccionará automáticamente_ los campos MSI que anteriormente estaban deshabilitados ([!UICONTROL Urgencia], [!UICONTROL Puntuación relativa] y [!UICONTROL Prioridad]). Simplemente haz clic en **[!UICONTROL Guardar]** en para comenzar a sincronizar los datos.

   ![](assets/enable-five.png)

## Definir acceso de usuario {#set-user-access}

Por último, debe otorgar acceso a usuarios específicos para que utilicen [!DNL Marketo Sales Insight].

1. Vaya a **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vaya a **[!UICONTROL Seguridad]**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Haga clic en **[!UICONTROL Usuarios]**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Seleccione a los usuarios a los que desea otorgar acceso a [!DNL Sales Insight] y haga clic en **[!UICONTROL Administrar roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Seleccione el rol [!DNL Marketo Sales Insight] y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   ¡Y tú deberías haber terminado! Por último, para realizar pruebas, inicie sesión en [!DNL Dynamics] como un usuario que tiene acceso a [!DNL Marketo Sales Insight] y observe a un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
