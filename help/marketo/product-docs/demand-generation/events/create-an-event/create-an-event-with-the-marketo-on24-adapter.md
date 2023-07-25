---
unique-page-id: 10096656
description: Creación de un evento con el adaptador Marketo ON24 - Documentos de Marketo - Documentación del producto
title: Creación de un evento con el adaptador Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Creación de un evento con el adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Debe estar familiarizado con los componentes básicos y la secuencia recomendada para crear Eventos en Marketo. También debe tener conocimientos prácticos de los siguientes conceptos de Marketo:

* [Programas de Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} así como los Eventos y las diferencias entre ellos
* [Canales](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Recursos locales](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campañas secundarias](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} and [Program Statuses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Consulte la [Documentación de API de Marketo](https://developers.marketo.com/documentation/rest/){target="_blank"} para obtener más información sobre las API de Marketo.

## Requisitos previos {#prerequisites}

Se requiere lo siguiente para utilizar la integración de Marketo ON24:

* **Suscripción a transmisiones por Internet ON24** - Si no tiene una suscripción actual, póngase en contacto directamente con ON24. **NOTA**: se requiere ON24 Hosted Edition. No se requiere la administración de eventos ON24.

* **Derechos de administrador para ON24** - Necesitarás esto para usar este conector y crear invitados en el sistema ON24.
* **Credenciales de conexión ON24** : Debe introducir esta información en Marketo para habilitar la integración: nombre de usuario, contraseña, ID de cliente y clave de cliente. Póngase en contacto con el administrador de cuentas de ON24 o con la asistencia técnica de ON24 si necesita ayuda con sus credenciales.
* **Formulario de registro** : utilice un formulario de Marketo o un formulario que no sea de Marketo junto con la API adecuada para garantizar que los datos de registro y la información del registrante se pasen a Marketo.
* **Campaña secundaria de registro** : Se debe crear y configurar correctamente una campaña secundaria de registro en el evento de Marketo para que funcione la integración de socios de evento.

## Flujo de proceso {#process-flow}

Siga estos pasos para crear un evento con el adaptador Marketo On24:

1. [Cree su evento de seminario web en ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Configuración de eventos y sincronización de Marketo con el seminario web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Creación de campañas secundarias y recursos locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Prueba de la integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Explicación de los estados del programa seminario web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Actualizaciones de registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
