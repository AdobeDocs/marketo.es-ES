---
unique-page-id: 10096675
description: Creación de campañas secundarias y recursos locales - Documentos de Marketo - Documentación del producto
title: Creación de campañas secundarias y recursos locales
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 1%

---

# Creación de campañas secundarias y recursos locales {#create-child-campaigns-and-local-assets}

Cree sus campañas secundarias y recursos locales mediante Design Studio.

## Página de aterrizaje y formulario {#landing-page-and-form}

Para garantizar que las personas estén correctamente registradas con ON24, se deben incluir los siguientes campos en el formulario de Marketo:

* Nombre
* Apellido
* Dirección de email

También puede insertar los campos siguientes en ON24:

* Nombre de la compañía
* Cargo

Con el paso de flujo adecuado añadido a la campaña de registro, la gente será empujada a ON24 y será marcada como registrada. Puede agregar otros campos al formulario y la información se capturará en Marketo como parte del registro de detalles de la persona.

>[!CAUTION]
>
>Para que la integración sea correcta, debe utilizar un formulario de Marketo para registrar a las personas para el evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketo.

## Correos electrónicos y tokens de URL {#emails-and-url-tokens}

Cree la invitación, la confirmación, el seguimiento y los correos electrónicos de agradecimiento mediante Marketo.

## Token de URL y correo electrónico de confirmación de Marketo {#marketo-confirmation-email-and-url-token}

Utilice Marketo para enviar el correo electrónico de confirmación del evento. Cuando una persona se registra, recibe una dirección URL única que se utiliza para entrar en el evento.

>[!NOTE]
>
>Para rellenar el correo electrónico de confirmación con esta dirección URL única, utilice el token siguiente en el correo electrónico: `{{member.webinar url}}`. Cuando envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
>
>Establezca el tipo de correo electrónico de confirmación en **Operativo** para garantizar que las personas que se registren reciban su información de confirmación, incluso si se dan de baja.

>[!TIP]
>
>Puede configurar ON24 para enviar correos electrónicos de confirmación, recordatorio o seguimiento. Consulte la [Sitio de ayuda de ON24](https://www.on24.com/live-webcast-elite/){target=&quot;_blank&quot;} para obtener más información.

## Requisitos de la campaña secundaria de registro {#registration-child-campaign-requirements}

Los eventos contienen una o más campañas secundarias que funcionan todas juntas para mover personas a través de los estados del programa y permiten rastrear el rendimiento del evento.

Algunos ejemplos de campañas secundarias son una campaña de invitación, una campaña de registro y campañas de seguimiento.

>[!CAUTION]
>
>Para que el adaptador haga su trabajo, DEBE crear una campaña de registro. Esta campaña debe ser activada por la persona que rellene un formulario y el primer paso debe cambiar el estado del programa de la persona a **Registrados**. A continuación, la campaña envía un correo electrónico de confirmación. Consulte el resto de este artículo para obtener más información.

**Registro/Confirmación (Campaña de Déclencheur)**

* Lista inteligente
* Déclencheur basado en **Rellena el formulario**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **Agregar restricción**, especialmente si se utiliza el mismo formulario en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de Marketo para registrar a las personas para el evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketo. Esto es fundamental para el éxito de la integración de socios de evento.

>[!NOTE]
>
>Si utiliza un formulario de Marketo en una página de aterrizaje que no sea de Marketo, el déclencheur será **Rellena el formulario** con el nombre del formulario.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flujo**

* **Cambiar estado del programa** - Se establece en Seminario web -> Registrado.

Este paso de flujo es necesario como PRIMER PASO DE FLUJO al configurar la campaña secundaria. Cuando el estado del programa de una persona cambia a Registrada, Marketo envía la información de registro a ON24. Ningún otro estado empuja a la persona.

* **Enviar correo electrónico** - Correo electrónico de confirmación. Establezca este correo electrónico en **Operativo** de modo que las personas que se hayan dado de baja de suscripción y se hayan registrado sigan recibiendo dicha asistencia.

La variable **Enviar correo electrónico** paso de flujo DEBE ser el segundo paso. El correo electrónico de confirmación contiene la variable `{{member.webinar url}}`, que se rellena con información devuelta a Marketo desde ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>El orden de estos pasos de flujo es importante debido al orden en que se realizan las acciones en Marketo. La variable **Cambiar estado del programa** step envía a la persona a ON24 para que se registre y se genera una URL única. Una vez hecho esto, puede enviar el correo electrónico de confirmación que incluya esta dirección URL única usando la variable `{{member.webinar URL}}` token.
>
>Si la persona es devuelta con un error de registro, no recibirá la confirmación por correo electrónico.

El siguiente paso es [probar la integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}.

>[!MORELIKETHIS]
>
>* [Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
>* [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [Explicación de los estados del programa de los seminarios web](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}

