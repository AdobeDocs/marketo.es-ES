---
unique-page-id: 10096675
description: Crear Campañas secundarias y recursos locales - Documentos de marketing - Documentación del producto
title: Crear Campañas secundarias y recursos locales
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Crear Campañas secundarias y recursos locales {#create-child-campaigns-and-local-assets}

Cree sus campañas secundarias y recursos locales con Design Studio.

## página de aterrizaje y formulario {#landing-page-and-form}

Para asegurarse de que las personas están registradas correctamente con ON24, se deben incluir los siguientes campos en el formulario de marketing:

* Nombre
* Apellido
* Dirección de correo electrónico

También puede insertar los siguientes campos en ON24:

* Nombre de compañía
* Puesto de trabajo

Con el paso de flujo adecuado añadido a la campaña de registro, la gente será empujada a ON24 y será marcada como registrada. Puede agregar otros campos al formulario y la información se capturará en Marketing como parte del registro de detalles de la persona.

>[!CAUTION]
>
>Para lograr una integración correcta, debe utilizar un formulario de Marketo para registrar a sus usuarios para el Evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketing.

## Mensajes de correo electrónico y tokens de URL {#emails-and-url-tokens}

Cree los mensajes de correo electrónico de invitación, confirmación, seguimiento y agradecimiento mediante MarketingTo.

## Autentificador de URL y correo electrónico de confirmación de marketing {#marketo-confirmation-email-and-url-token}

Utilice Marketing para enviar el correo electrónico de confirmación de su evento. Cuando una persona se registra, recibe una dirección URL única para entrar en el evento.

>[!NOTE]
>
>**Recordatorio**
>
>Para completar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Al enviar la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
>
>Establezca el tipo de correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren reciban la información de confirmación, incluso si se cancelan las suscripciones.

>[!TIP]
>
>Puede configurar ON24 para enviar correos electrónicos de confirmación, recordatorio o seguimiento. Consulte el [sitio](http://webcastelitehelp.on24.com) de ayuda de ON24 para obtener más información.

## Requisitos de Campaña secundaria de registro {#registration-child-campaign-requirements}

Los eventos contienen una o más campañas secundarias que funcionan todas juntas para mover personas a través de los estados de programa y permitirle rastrear el rendimiento del evento.

Ejemplos de campañas infantiles son una campaña de invitación, una campaña de registro y campañas de seguimiento.

>[!CAUTION]
>
>Para que el adaptador pueda realizar su trabajo, debe crear una campaña de registro. Esta campaña debe activarla la persona que rellena un formulario y el primer paso debe cambiar el estado de programa de la persona a **Registrada**. A continuación, la campaña envía un correo electrónico de confirmación. Consulte el resto de este artículo para obtener más información.

**Registro/Confirmación (Campaña desencadenadora)**

* Lista inteligente
* Activador basado en **Rellenar formulario**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **Añadir restricción**, especialmente si se utiliza el mismo formulario en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de marketing para registrar a las personas para el evento o un formulario que no sea de marketing con la integración de API adecuada para insertar los datos de registro en Marketing. Esto es fundamental para el éxito de la integración de socios de evento.

>[!NOTE]
>
>Si está utilizando un formulario de marketing en una página de aterrizaje que no sea de marketing, el activador será **Rellenar formulario** con el nombre del formulario.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flujo**

* **Cambiar estado** de Programa - Establecer como seminario web -> Registrado.

Este paso de flujo es necesario como PRIMER PASO DE FLUJO al configurar la campaña infantil. Cuando el estado de programa de una persona cambia a Registrado, Marketo coloca la información de registro en ON24. Ningún otro estado empujará a la persona.

* **Enviar correo electrónico** : correo electrónico de confirmación. Establezca este mensaje de correo electrónico en **Operativo** para que las personas que se han registrado aún lo reciban.

El paso **Enviar correo electrónico** DEBE ser el segundo paso. El mensaje de correo electrónico de confirmación contiene el `{{member.webinar url}}`, que se rellena con la información que se devuelve a Marketing desde ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>El orden de estos pasos de flujo es importante debido al orden en que se realizan las acciones en Marketing. El paso **Cambiar estado** de Programa envía a la persona a ON24 para registrarse y se genera una dirección URL única. Después de esto, puede enviar el correo electrónico de confirmación que incluye esta dirección URL única mediante el `{{member.webinar URL}}` token.
>
>Si la persona es devuelta con un error de registro, no recibirá la confirmación por correo electrónico.

El siguiente paso es [probar la integración](test-your-on24-event-integration.md)de evento ON24.

>[!MORELIKETHIS]
>
>* [Explicación de los Eventos del adaptador de Marketo ON24](understanding-marketo-on24-adapter-events.md)
>* [Ejemplo de integración de Evento ON24](example-on24-event-integration.md)
>* [Explicación de los estados de Programa de seminario web](understanding-webinar-program-statuses.md)
>* [Probar la integración del Evento ON24](test-your-on24-event-integration.md)

>



