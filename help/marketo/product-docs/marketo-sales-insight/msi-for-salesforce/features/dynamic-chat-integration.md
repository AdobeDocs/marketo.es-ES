---
description: Integración de Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Integración de Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 6e81a8891f7d6e5916549d453a694b42e08cd496
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# Integración de Dynamic Chat {#dynamic-chat-integration}

Obtenga más información sobre la integración de Dynamic Chat con Sales Insight.

>[!PREREQUISITES]
>
>* El paquete de SFDC de Sales Insight debe ser una versión [2.4.0 o superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Debe tener el [Integración de Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} configurar
>
>* Asegúrese de que su perspectiva de ventas [Configuración operativa](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}, you have the "API Secret Key" field populated. If you don't, learn how to retrieve it [here](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Pestaña Configuración de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Siga los pasos a continuación para habilitar la integración de Dynamic Chat.

1. Inicie sesión en su cuenta de Salesforce, haga clic en + al final de la barra de pestañas y luego en **Configuración de Marketo Sales Insight**.

1. Haga clic para desplegar el &quot;Panel de fuerza visual&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleccione el **Habilitar datos del Dynamic Chat** casilla de verificación

   ![](assets/dynamic-chat-integration-2.png)

## Descripción general de funciones {#feature-overview}

Los usuarios de Sales Insight pueden aprovechar las siguientes actividades de Dynamic Chat...

Diálogo comprometido: Ha iniciado sesión en Marketo y se ha completado en Sales Insight cuando un visitante hace clic en un bot de chat e interactúa con el diálogo.

* Nombre del cuadro de diálogo
* URL de la página
* Estado (Iniciado/Descartado/Completado)

Cita programada: se ha iniciado sesión en Marketo y se ha completado en Sales Insight cuando un visitante programa correctamente una cita a través del bot de chat.

* Nombre del cuadro de diálogo
* Agente
* URL de la página
* Programado el (insertar marca de fecha y hora)
* Estado (Programado, Reprogramado, Cancelado)

Meta alcanzada: Se ha iniciado sesión en Marketo y se ha completado en Información de ventas cuando un visitante alcanza una meta en cualquier flujo de diálogo.

* Nombre del cuadro de diálogo
* Nombre de meta
* URL de la página

Interactuó con el documento: ha iniciado sesión en Marketo y se rellena en Sales Insight cuando un visitante interactúa con un documento compartido mediante el bot de chat.

* Nombre del cuadro de diálogo
* Documento
* Estado

Las actividades de chat están disponibles en el panel de perspectivas.

![](assets/dynamic-chat-integration-3.png)

Hay una pestaña de chat disponible en los paneles Posible cliente y Contacto. Incluye las columnas Tipo de actividad, Nombre del cuadro de diálogo y Fecha.

![](assets/dynamic-chat-integration-4.png)

Para obtener más información sobre un tipo de actividad, haga clic en él.

![](assets/dynamic-chat-integration-5.png)

Del mismo modo, los paneles Cuenta y Oportunidad incluyen las columnas Nombre, Tipo de actividad, Nombre del cuadro de diálogo y Fecha.

![](assets/dynamic-chat-integration-6.png)

La pestaña Chat también se incluye en la pestaña Global Marketo. Incluye tres tipos de actividades (diálogo comprometido, cita programada, objetivo alcanzado), junto con las siguientes columnas:

* Persona
* Cuenta
* Tipo de actividad (cuadro de diálogo con participación, cita programada, meta alcanzada)
* Nombre del cuadro de diálogo
* Marca de fecha y hora

De nuevo, puede obtener más información sobre un tipo de actividad haciendo clic en él.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Si la casilla &quot;Habilitar datos del Dynamic Chat&quot; está desactivada, se desactivarán las siguientes funciones:
>
>* Fila con actividades de chat en el panel de perspectivas (cuadrícula inteligente y vista de lista semanal)
>* Pestaña Chat en los paneles Posible cliente, Contacto, Cuenta y Oportunidad
>* Pestaña Chat en la pestaña Global Marketo
>
>No es posible desactivar solo una de estas funciones.

