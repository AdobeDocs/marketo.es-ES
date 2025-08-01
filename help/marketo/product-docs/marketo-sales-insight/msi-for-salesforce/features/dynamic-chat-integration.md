---
description: 'Integración de Dynamic Chat: documentos de Marketo, documentación del producto'
title: Integración del Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# Integración del Dynamic Chat {#dynamic-chat-integration}

Obtenga más información sobre la integración de Dynamic Chat con Sales Insight.

>[!PREREQUISITES]
>
>* Su paquete de Sales Insight SFDC debe ser de la versión [2.4.0 o superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Debe tener configurada la [integración de Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Compruebe que en su [Configuración operativa](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} de Sales Insight haya rellenado el campo &quot;Clave secreta de API&quot;. Si no lo hace, aprenda a recuperarlo [aquí](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## [!DNL Marketo Sales Insight] ficha de configuración {#marketo-sales-insight-configuration-tab}

Siga los pasos a continuación para habilitar la integración de [!DNL Dynamic Chat].

1. Inicie sesión en su cuenta de [!DNL Salesforce], haga clic en + al final de la barra de fichas y luego en **[!DNL Marketo Sales Insight Config]**.

1. Haga clic para desplegar el &quot;[!UICONTROL Panel Visualforce]&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleccione la casilla de verificación **[!UICONTROL Habilitar datos de Dynamic Chat]**.

   ![](assets/dynamic-chat-integration-2.png)

## Descripción general de funciones {#feature-overview}

[!DNL Dynamic Chat] usuarios pueden aprovechar las siguientes [!DNL Sales Insight] actividades...

Diálogo comprometido: Se ha iniciado sesión en Marketo y se ha completado en [!DNL Sales Insight] cuando un visitante hace clic en un bot de chat e interactúa con el cuadro de diálogo.

* Nombre del diálogo
* URL de página
* Estado (Iniciado/Descartado/Completado)

Cita programada: se inició sesión en Marketo y se completó en [!DNL Sales Insight] cuando un visitante programa correctamente una cita a través del bot de chat.

* Nombre del diálogo
* Agente
* URL de página
* Programado el (insertar marca de fecha y hora)
* Estado (Programado, Reprogramado, Cancelado)

Meta alcanzada: Se inició sesión en Marketo y se completó en [!DNL Sales Insight] cuando un visitante alcanza una meta en cualquier flujo de diálogo.

* Nombre del diálogo
* Nombre del objetivo
* URL de página

Se interactuó con el documento: se inició sesión en Marketo y se rellenó en [!DNL Sales Insight] cuando un visitante interactúa con un documento compartido a través del bot de chat.

* Nombre del diálogo
* Documento
* Estado

Las actividades de chat están disponibles en el panel de perspectivas.

![](assets/dynamic-chat-integration-3.png)

Hay una pestaña de chat disponible en los paneles Posible cliente y Contacto. Incluye las columnas [!UICONTROL Tipo de actividad], [!UICONTROL Nombre del cuadro de diálogo] y [!UICONTROL Fecha].

![](assets/dynamic-chat-integration-4.png)

Para obtener más información sobre un tipo de actividad, haga clic en él.

![](assets/dynamic-chat-integration-5.png)

Del mismo modo, los paneles Cuenta y Oportunidad incluyen las columnas [!UICONTROL Nombre], [!UICONTROL Tipo de actividad], [!UICONTROL Nombre del cuadro de diálogo] y [!UICONTROL Fecha].

![](assets/dynamic-chat-integration-6.png)

La pestaña Chat también se incluye en la pestaña Global Marketo. Incluye tres tipos de actividades ([!UICONTROL Diálogo comprometido], [!UICONTROL Cita programada], [!UICONTROL Objetivo alcanzado]), junto con las siguientes columnas:

* [!UICONTROL Persona]
* [!UICONTROL Cuenta]
* [!UICONTROL Tipo de actividad] ([!UICONTROL Diálogo con participación], [!UICONTROL Cita programada], [!UICONTROL Objetivo alcanzado])
* [!UICONTROL Nombre del cuadro de diálogo]
* [!UICONTROL Fecha]

De nuevo, puede obtener más información sobre un tipo de actividad haciendo clic en él.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Si la casilla de verificación &quot;[!UICONTROL Habilitar datos de Dynamic Chat]&quot; está deshabilitada, se deshabilitarán las siguientes características:
>
>* Fila con actividades de chat en el panel de perspectivas (cuadrícula inteligente y vista de lista semanal)
>* Pestaña Chat en los paneles Posible cliente, Contacto, Cuenta y Oportunidad
>* Pestaña Chat en la pestaña Global Marketo
>
>No es posible desactivar solo una de estas funciones.
