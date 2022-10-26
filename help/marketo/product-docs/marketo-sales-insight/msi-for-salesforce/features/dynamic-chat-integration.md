---
description: 'Integración de Dynamic Chat: Marketo Docs: Documentación del producto'
title: Integración de Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 9d5c941dc4869b03787a6135550a133ce12b365b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 5%

---

# Integración de Dynamic Chat {#dynamic-chat-integration}

Obtenga más información sobre la integración de Dynamic Chat con la perspectiva de ventas.

>[!PREREQUISITES]
>
>* El paquete de SFDC de Sales Insight debe ser de versión [1.9 o superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Debe tener la variable [Integración con Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} configurado


## Ficha Configuración de la perspectiva de ventas de Marketo {#marketo-sales-insight-configuration-tab}

Siga los pasos a continuación para habilitar la integración de Dynamic Chat.

1. Inicie sesión en su cuenta de Salesforce, haga clic en + al final de la barra de pestañas y haga clic en **Configuración de perspectiva de ventas de Marketo**.

1. Haga clic en para desplegar el &quot;Panel de fuerza visual&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleccione el **Habilitar datos de chat dinámico** casilla de verificación.

   ![](assets/dynamic-chat-integration-2.png)

## Descripción general de características {#feature-overview}

Los usuarios de Sales Insight pueden aprovechar las siguientes actividades de Dynamic Chat...

Diálogo comprometido: Inició sesión en Marketo y se rellena en Perspectiva de ventas cuando un visitante hace clic en un bot de chat y participa en el Diálogo.

* Nombre del cuadro de diálogo
* URL de la página
* Estado (iniciado/descartado/completado)

Cita programada: Inició sesión en Marketo y se rellena en Perspectiva de ventas cuando un visitante programa correctamente una cita a través del bot de chat.

* Nombre del cuadro de diálogo
* Agente
* URL de la página
* Programado el (insertar fecha y hora)
* Estado (programado, reprogramado, cancelado)

Objetivo alcanzado: Inició sesión en Marketo y se rellena en Perspectiva de ventas cuando un visitante alcanza un objetivo en cualquier flujo de diálogos.

* Nombre del cuadro de diálogo
* Nombre del objetivo
* URL de la página

Interactuado con el documento: Inició sesión en Marketo y se rellena en Perspectiva de ventas cuando un visitante interactúa con un documento compartido a través del bot de chat.

* Nombre del cuadro de diálogo
* Documento
* Estado

Las actividades de chat están disponibles en el panel de perspectivas.

![](assets/dynamic-chat-integration-3.png)

Hay una pestaña Chat disponible en los paneles Posibles clientes y Contacto . Incluye las columnas Tipo de actividad, Nombre del cuadro de diálogo y Fecha.

![](assets/dynamic-chat-integration-4.png)

Para obtener más información sobre un tipo de actividad, haga clic en él.

![](assets/dynamic-chat-integration-5.png)

Del mismo modo, los paneles Cuenta y Oportunidad incluyen las columnas Nombre, Tipo de actividad, Nombre del cuadro de diálogo y Fecha.

![](assets/dynamic-chat-integration-6.png)

La pestaña Chat también está incluida en su pestaña Marketo global. Incluye tres tipos de actividades (Diálogo con participación, Nombramiento programado, Objetivo alcanzado), junto con las siguientes columnas:

* Persona
* Cuenta
* Tipo de actividad (cuadro de diálogo con participación, cita programada, objetivo alcanzado)
* Nombre del cuadro de diálogo
* Marca de fecha y hora

De nuevo, puede obtener más información sobre un tipo de actividad haciendo clic en él.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Si la casilla &quot;Habilitar datos de chat dinámico&quot; está desactivada, se deshabilitarán las siguientes funciones:
>
>* Fila con actividades de chat en el panel de perspectivas (cuadrícula inteligente y vista de lista semanal)
>* Ficha Chat de los paneles Posible cliente, Contacto, Cuenta y Oportunidad
>* Pestaña Chat de la pestaña Marketo Global
>
>No es posible desactivar solo una de estas funciones.

