---
description: Plantillas de correo electrónico de ventas transaccionales - Documentos de Marketo - Documentación del producto
title: Plantillas de correo electrónico de ventas transaccionales
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Plantillas de correo electrónico de ventas transaccionales {#transactional-sales-email-templates}

Si su equipo envía correos electrónicos transaccionales o no comerciales, puede marcar una plantilla de correo electrónico como no comercial para que pueda evitar las cancelaciones de suscripción.

## Cosas que hay que tener en cuenta {#things-to-note}

* Los correos electrónicos no comerciales evitarán las cancelaciones de suscripción de ventas y [Comprobación de cancelación de suscripción del Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Los mensajes de cancelación de suscripción no se adjuntarán automáticamente a los correos electrónicos no comerciales, aunque la variable [anexar configuración de administración de mensaje de cancelación de suscripción](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} seguirá rellenando el mensaje de cancelación de suscripción de su equipo.

## Configuración de una plantilla de correo electrónico para uso no comercial {#configure-an-email-template-for-non-commercial-use}

1. En el encabezado, haga clic en **Plantillas**.

PICC

1. Busque la plantilla que desee actualizar.

PICC

1. Seleccione la plantilla.

PICC

1. Habilite la opción de correo electrónico no comercial en Configuración de plantilla.

PICC

## Enviar un correo electrónico no comercial {#send-a-non-commercial-email}

Cuando se selecciona una persona sin suscribir, aparece resaltada en naranja.

1. En la ventana de composición, seleccione la plantilla no comercial que desee ver.

PICC

1. Los usuarios verán un banner que les mostrará que han seleccionado actualmente una plantilla de correo electrónico no comercial.

PICC

1. Clic **Enviar**.

PICC

El correo electrónico se enviará incluso si la persona ha cancelado la suscripción.
