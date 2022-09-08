---
unique-page-id: 10096656
description: Creación de un evento con el adaptador Marketo ON24 - Marketo Docs - Documentación del producto
title: Crear un evento con el adaptador Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Crear un evento con el adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

>[!IMPORTANT]
>
>A partir de agosto de 2022, ON24 ya no es compatible con las nuevas integraciones de Marketo. La información de este artículo solo se aplica a los usuarios existentes.

Debe conocer los componentes básicos y la secuencia recomendada para crear eventos en Marketo. También debe tener conocimientos prácticos de los siguientes conceptos de Marketo:

* [Programas de Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) , así como eventos y las diferencias entre ellos
* [Canales](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Recursos locales](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Campañas secundarias](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) y [Estados del programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Consulte la [Documentación de la API de Marketo](https://developers.marketo.com/documentation/rest/) para obtener más información sobre las API de Marketo.

## Requisitos previos {#prerequisites}

Para utilizar la integración Marketo ON24, es necesario lo siguiente:

* **Suscripción a las transmisiones web ON24** - Si no tiene una suscripción actual, póngase en contacto directamente con ON24. **NOTA**: Se requiere ON24 Hosted Edition. No se requiere la administración de eventos ON24.

* **Derechos de administrador a ON24** - Necesitará esto para utilizar este conector y crear invitados en el sistema ON24.
* **Credenciales de conexión ON24** : Deberá introducir esta información en Marketo para habilitar la integración: Nombre de usuario, Contraseña, ID de cliente y Clave de cliente. Póngase en contacto con el administrador de cuentas de ON24 o con la asistencia de ON24 si necesita ayuda con sus credenciales.
* **Formulario de registro** - Utilice un formulario de Marketo o un formulario que no sea de Marketo junto con la API adecuada para garantizar que los datos de registro y la información de registro se pasen a Marketo.
* **Campaña secundaria de registro** - Se debe crear y configurar correctamente una campaña secundaria de registro en el Evento de Marketo para que funcione la integración de Socios de evento.

## Flujo de proceso {#process-flow}

Siga estos pasos para crear un evento con el adaptador Marketo On24:

1. [Crear el evento de seminario web en ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Configuración de eventos y sincronización de Marketo con el seminario web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Creación de campañas secundarias y recursos locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Probar la integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Explicación de los estados del programa de los seminarios web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Actualizaciones de registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
