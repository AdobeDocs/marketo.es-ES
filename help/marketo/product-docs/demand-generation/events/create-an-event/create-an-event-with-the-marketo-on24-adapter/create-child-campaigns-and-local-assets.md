---
unique-page-id: 10096675
description: 'Creación de campañas secundarias y Assets local: documentos de Marketo: documentación del producto'
title: Creación de campañas secundarias y Assets local
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Creación de campañas secundarias y Assets local {#create-child-campaigns-and-local-assets}

Cree sus campañas secundarias y recursos locales con Design Studio.

## Página de aterrizaje y formulario {#landing-page-and-form}

Para garantizar que las personas estén correctamente registradas con ON24, se deben incluir los siguientes campos en el formulario de Marketo:

* Nombre
* Apellido
* Correo electrónico

También puede insertar los campos siguientes en ON24:

* Nombre de la empresa
* Cargo

Con el paso de flujo adecuado agregado a la campaña de registro, las personas se transferirán a ON24 y se marcarán como registradas. Puede agregar otros campos al formulario, y la información se capturará en Marketo como parte del registro de detalles de la persona.

>[!CAUTION]
>
>Para una integración correcta, debe utilizar un formulario de Marketo para registrar a sus recursos en el evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketo.

## Correos electrónicos y tokens de URL {#emails-and-url-tokens}

Cree los correos electrónicos de invitación, confirmación, seguimiento y agradecimiento con Marketo.

## Token de correo electrónico y URL de confirmación de Marketo {#marketo-confirmation-email-and-url-token}

Utilice Marketo para enviar el correo electrónico de confirmación del evento. Cuando una persona se registra, recibe una dirección URL única para utilizar y entrar en el evento.

>[!NOTE]
>
>Para rellenar el correo electrónico de confirmación con esta dirección URL única, use el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando envía la URL de confirmación, este token se resuelve automáticamente en la URL de confirmación única de la persona.
>
>Establece el tipo de tu correo electrónico de confirmación en **Operativo** para asegurarte de que las personas que se registren reciban su información de confirmación, incluso si cancelaron su suscripción.

>[!TIP]
>
>Puede configurar ON24 para enviar correos electrónicos de confirmación, recordatorio o seguimiento. Consulte el [Sitio de ayuda ON24](https://www.on24.com/live-webcast-elite/){target="_blank"} para obtener más información.

## Requisitos de la campaña secundaria de registro {#registration-child-campaign-requirements}

Los eventos contienen una o más campañas secundarias que trabajan juntas para mover a las personas a través de los estados del programa y permitirle rastrear el rendimiento del evento.

Algunos ejemplos de campañas secundarias son una campaña de invitación, una campaña de registro y campañas de seguimiento.

>[!CAUTION]
>
>Para que el adaptador realice su trabajo, DEBE crear una campaña de registro. Esta campaña debe activarla la persona que rellene un formulario y el primer paso debe cambiar el estado del programa de la persona a **Registrada**. A continuación, la campaña envía un correo electrónico de confirmación. Consulte el resto de este artículo para obtener más información.

**Registro/Confirmación (Campaña de Déclencheur)**

* Lista inteligente
* Déclencheur basado en **Rellena formulario**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **Agregar restricción**, especialmente si el mismo formulario se utiliza en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de Marketo para registrar a sus personas en el evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketo. Esto es fundamental para el éxito de la integración de su socio de eventos.

>[!NOTE]
>
>Si usas un formulario de Marketo en una página de aterrizaje que no sea de Marketo, el déclencheur será **Rellena el formulario** con el nombre del formulario.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flujo**

* **Cambiar estado del programa** - Definir en seminario web -> Registrado.

Este paso de flujo es necesario como el PRIMER PASO DE FLUJO al configurar la campaña secundaria. Cuando el estado del programa de una persona cambia a Registrado, Marketo envía la información de registro a ON24. Ningún otro estado empujará a la persona.

* **Enviar correo electrónico** - Correo electrónico de confirmación. Establece este correo electrónico en **Operativo** para que las personas que cancelaron su suscripción y se hayan registrado lo sigan recibiendo.

El paso de flujo **Enviar correo electrónico** DEBE ser el segundo paso. El correo electrónico de confirmación contiene `{{member.webinar url}}`, que se rellena con información devuelta a Marketo desde el ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>El orden de estos pasos de flujo es importante debido al orden en que se realizan las acciones en Marketo. El paso **Cambiar estado del programa** envía a la persona a ON24 para que se registre y se genere una dirección URL única. Una vez hecho esto, puede enviar el correo electrónico de confirmación que incluye esta dirección URL única usando el token `{{member.webinar URL}}`.
>
>Si la persona es devuelta con un error de registro, no recibirá la confirmación por correo electrónico.

El siguiente paso es [probar la integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Explicación de los estados del programa de seminarios web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
