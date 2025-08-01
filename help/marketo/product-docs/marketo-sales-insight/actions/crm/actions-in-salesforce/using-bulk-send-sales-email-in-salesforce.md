---
description: Uso del envío masivo de correo electrónico de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Uso del envío masivo de correo electrónico de ventas en Salesforce
exl-id: 4886109d-c2b8-4186-922b-8a15cf1e742e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Uso del envío masivo de correo electrónico de ventas en Salesforce {#using-bulk-send-sales-email-in-salesforce}

Aprenda a enviar correos electrónicos masivos en Salesforce para escalar la comunicación saliente mediante acciones de ventas.

>[!NOTE]
>
>Salesforce aplica un límite de 200 registros que se pueden seleccionar a la vez.

>[!PREREQUISITES]
>
>Asegúrese de que ha instalado el [último paquete de Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} en su instancia de Salesforce y de que ha configurado los [botones de acción](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} en las vistas de contactos y listas de posibles clientes en Salesforce.

## Envío de correo electrónico masivo en Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. En Salesforce, vaya a la página de inicio de los posibles clientes o contactos haciendo clic en la ficha **Posibles clientes o contactos**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. En la lista desplegable Ver, seleccione la vista que desee de los posibles clientes/contactos que desee enviar por correo electrónico.

   >[!TIP]
   >
   >Para crear una vista nueva, haz clic en el icono de engranaje a la derecha y selecciona **Nuevo**. Una vez que le haya dado a la vista un nuevo nombre y lo haya guardado, puede hacer clic en el icono de filtro de la derecha para ayudar a filtrar hasta el conjunto deseado de posibles clientes/contactos que desee enviar por correo electrónico.

1. Elige el posible cliente o la lista de contactos que desees y haz clic en el botón **Enviar correo electrónico de ventas**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Se abrirá la ventana de composición Acciones, en la que se añadirán las personas seleccionadas.

1. Seleccione la plantilla que desee insertar en el editor de la ventana de composición Acciones o escriba un correo electrónico personalizado.

   >[!TIP]
   >
   >Use [Categorías ancladas](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} para facilitar el acceso a sus plantillas de correo electrónico favoritas.

   **PASO OPCIONAL**: Obtenga una vista previa de cualquier personalización de campos dinámicos haciendo clic en el botón **Vista previa de campos dinámicos**.

   >[!TIP]
   >
   >Si desea personalizar una plantilla para todos los destinatarios, hacer clic en la opción Todos los destinatarios en la barra lateral de composición masiva le permite realizar ediciones en todos los correos electrónicos de los destinatarios al mismo tiempo. Si desea realizar un cambio en un correo electrónico específico, haga clic en el nombre del destinatario o en el correo electrónico en la barra lateral de composición en lote. Tenga en cuenta que si realiza cambios en un correo electrónico individual y luego realiza cambios al seleccionar Todos los destinatarios, los cambios realizados en Todos los destinatarios sobrescribirán los cambios realizados en el correo electrónico individual.

1. Seleccione **Enviar** para enviar el correo electrónico inmediatamente o **Establecer horario** para establecer una fecha y hora para el correo electrónico que se enviará.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Envío de correo electrónico masivo en Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. En Salesforce, haga clic en la ficha **Posibles clientes/contactos**.

1. En el menú desplegable Ver, selecciona la vista que desees de los posibles clientes o contactos que deseas enviar por correo electrónico y haz clic en **Ir**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Para crear una nueva vista, haga clic en Crear nueva vista y configure los filtros disponibles para reducir la lista de usuarios que añade a una campaña de ventas.

1. Elige la lista de contactos o posibles clientes que desees y haz clic en el botón **Enviar correo electrónico de ventas**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. Se abrirá la ventana de composición Acciones (Actions) con los destinatarios seleccionados en la ventana de composición.

1. Seleccione la plantilla que desee insertar en el editor de la ventana de composición Acciones o escriba un correo electrónico personalizado.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Use [Categorías ancladas](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} para facilitar el acceso a sus plantillas de correo electrónico favoritas.

   **PASO OPCIONAL**: Obtenga una vista previa de cualquier personalización de campos dinámicos haciendo clic en el botón **Vista previa de campos dinámicos**.

   >[!TIP]
   >
   >Si desea personalizar una plantilla para todos los destinatarios, hacer clic en la opción Todos los destinatarios en la barra lateral de composición masiva le permite realizar ediciones en todos los correos electrónicos de los destinatarios al mismo tiempo. Si desea realizar un cambio en un correo electrónico específico, haga clic en el nombre del destinatario o en el correo electrónico en la barra lateral de composición en lote. Tenga en cuenta que si realiza cambios en un correo electrónico individual y luego realiza cambios al seleccionar Todos los destinatarios, los cambios realizados en Todos los destinatarios sobrescribirán los cambios realizados en el correo electrónico individual.

1. Seleccione **Enviar** para enviar el correo electrónico inmediatamente o **Establecer horario** para establecer una fecha y hora para el correo electrónico que se enviará.
