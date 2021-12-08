---
description: Razones de la llamada de registro y resultados de la llamada a Salesforce - Marketo Docs - Documentación del producto
title: Razones de la llamada de registro y resultados de la llamada a Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Razones de la llamada de registro y resultados de la llamada a Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Si desea registrar los resultados de las llamadas y llamar a Salesforce por motivos de informes o visibilidad, puede crear un campo de actividad personalizado para cada uno. Cada campo debe utilizar un nombre de API específico.

* Nombre de la API de resultados de la llamada: mktosales_call_result
* Nombre de la API de motivos de la llamada: mktosales_call_reason

Para utilizar estos campos, primero debe crear el campo como campo de actividad personalizado. Para que los usuarios puedan verlo, deberá agregarlo al diseño de página del objeto de tarea.

## Crear campo de actividad personalizado en Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. En Salesforce, vaya a Configuración.

PICC

1. Introduzca &quot;Actividades&quot; en el cuadro Búsqueda rápida.

PICC

1. Haga clic en **Campos personalizados de actividad**.

PICC

1. Haga clic en **Nuevo**.

PICC

## Crear campo de actividad personalizado en el relámpago de Salesforce {#create-custom-activity-field-in-salesforce-lightning}

1. En Salesforce, haga clic en el icono del engranaje en la parte superior derecha.

PICC

1. Haga clic en **Configuración**.

PICC

1. Haga clic en **Administrador de objetos**.

PICC

1. Introduzca Actividad en el cuadro Búsqueda rápida y haga clic en la etiqueta Actividad para abrir la configuración del objeto.

PICC

1. En el lado izquierdo, haga clic en **Campos y relaciones**.

PICC

1. Haga clic en **Nuevo**.

PICC

## Agregar campo de actividad personalizado al diseño de página de tarea en Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

PASOS

## Agregar campo de actividad personalizado al diseño de página de tarea en el relámpago de Salesforce {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

PASOS

>[!MORELIKETHIS]
>
>[Instalar campos de evento de conexión de ventas en el historial de actividades](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
