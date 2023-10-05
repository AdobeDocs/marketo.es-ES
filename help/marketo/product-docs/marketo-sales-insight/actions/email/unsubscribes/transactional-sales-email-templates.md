---
description: Plantillas de correo electrónico de ventas transaccionales - Documentos de Marketo - Documentación del producto
title: Plantillas de correo electrónico de ventas transaccionales
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# Plantillas de correo electrónico de ventas transaccionales {#transactional-sales-email-templates}

Si su equipo envía correos electrónicos transaccionales o no comerciales, puede marcar una plantilla de correo electrónico como no comercial para que pueda evitar las cancelaciones de suscripción.

## Cosas que hay que tener en cuenta {#things-to-note}

* Los correos electrónicos no comerciales evitarán las cancelaciones de suscripción de ventas y [Comprobación de cancelación de suscripción del Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Los mensajes de cancelación de suscripción no se adjuntarán automáticamente a los correos electrónicos no comerciales, aunque la variable [anexar configuración de administración de mensaje de cancelación de suscripción](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} seguirá rellenando el mensaje de cancelación de suscripción de su equipo.

## Configuración de una plantilla de correo electrónico para uso no comercial {#configure-an-email-template-for-non-commercial-use}

1. En el encabezado, haga clic en **Plantillas**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Busque y seleccione la plantilla que desea actualizar.

   ![](assets/transactional-sales-email-templates-2.png)

1. Habilite la opción de correo electrónico no comercial en Configuración de plantilla.

   ![](assets/transactional-sales-email-templates-3.png)

## Enviar un correo electrónico no comercial {#send-a-non-commercial-email}

>[!NOTE]
>
>Cuando se selecciona una persona sin suscribir, aparece resaltada en naranja.

1. En el encabezado, haga clic en **Escribir**. Busque y seleccione la plantilla no comercial que desee.

   ![](assets/transactional-sales-email-templates-4.png)

1. Los usuarios verán un banner que les mostrará que han seleccionado una plantilla de correo electrónico no comercial.

   ![](assets/transactional-sales-email-templates-5.png)

1. Clic **Enviar**.

   ![](assets/transactional-sales-email-templates-6.png)

El correo electrónico se enviará incluso si la persona ha cancelado la suscripción.
