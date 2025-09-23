---
unique-page-id: 10096656
description: Creación de un evento con el adaptador Marketo ON24 - Documentos de Marketo - Documentación del producto
title: Crear un evento con el adaptador Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 6%

---

# Crear un evento con el adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Debe estar familiarizado con los componentes básicos y la secuencia recomendada para crear Eventos en Marketo. También debe tener conocimientos prácticos de los siguientes conceptos de Marketo:

* [Programas de Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}, así como Eventos y las diferencias entre ellos
* [Canales](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Assets local](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campañas secundarias](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} y [Estados de programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Consulte la [Documentación de la API de Marketo](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} para obtener más información sobre las API de Marketo.

## Requisitos previos {#prerequisites}

Se requiere lo siguiente para utilizar la integración de Marketo ON24:

* **Suscripción a transmisiones por Internet ON24**: si no dispone de una suscripción actual, póngase en contacto directamente con ON24. **NOTA**: ON24 Hosted Edition es obligatorio. No se requiere la administración de eventos ON24.

* **Derechos de administrador para ON24**: necesitará esto para usar este conector y crear invitados en el sistema ON24.
* **Credenciales de conexión ON24**: tendrá que introducir esta información en Marketo para habilitar la integración: nombre de usuario, contraseña, ID de cliente y clave de cliente. Póngase en contacto con el administrador de cuentas de ON24 o con la asistencia técnica de ON24 si necesita ayuda con sus credenciales.
* **Formulario de registro**: utilice un formulario de Marketo o uno que no sea de Marketo junto con la API adecuada para asegurarse de que los datos de registro y la información del solicitante se pasan a Marketo.
* **Campaña secundaria de registro**: para que funcione la integración de socios de eventos, debe crearse y configurarse correctamente una campaña secundaria de registro en su evento de Marketo.

## Flujo de proceso {#process-flow}

Siga estos pasos para crear un evento con el adaptador Marketo On24:

1. [Cree su evento de seminario web en ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Configurar la configuración de eventos y sincronizar Marketo con el seminario web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Crear campañas secundarias y Assets local](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Probar la integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Explicación de los estados del programa de seminarios web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Actualizaciones de registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
