---
description: Configuración de una zona protegida de acciones de información de ventas - Documentos de Marketo - Documentación del producto
title: Configuración de una zona protegida de acciones de perspectiva de ventas
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Configuración de una zona protegida de acciones de perspectiva de ventas {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions es una aplicación basada en web que se integra exclusivamente con Salesforce CRM mediante el [paquete de Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. A veces se denomina &quot;Ventas Marketo&quot; o simplemente &quot;Acciones&quot;.

Si tiene una zona protegida de Marketo, puede habilitar una instancia de acciones para utilizarla con fines de prueba.

Al configurar una instancia de acciones, debe decidir si se configura para que funcione con la zona protegida de Salesforce o con la producción de Salesforce. Esto se debe a que Salesforce utiliza diferentes puntos de conexión para cada uno y Actions utiliza la conexión con Salesforce para activar y autenticar a los usuarios.

Siga los pasos a continuación para configurar una instancia de acciones para que funcione con la instancia de zona protegida de Salesforce.

>[!NOTE]
>
>Puede obtener más información sobre cómo [activarán el puesto de acciones](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. También puede obtener información sobre cómo se autenticarán los usuarios [con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Además, si prefiere que los usuarios se autentiquen con correo electrónico y contraseña, puede obtener más información al respecto en nuestro [artículo de configuración de administración de inicio de sesión](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Solicite que se aprovisione una instancia de acciones a su zona protegida de Marketo {#request=an-actions-instance}

Acciones de perspectiva de ventas no está habilitado para instancias de zona protegida de Marketo a menos que se solicite. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para enviar una solicitud.

## Aprovisionar la cuenta de acciones para la zona protegida de Marketo {#provision-your-actions-account}

Una vez que Actions esté habilitada para tu zona protegida de Marketo, deberás seguir los pasos a continuación para activar tu nueva instancia.

1. Inicie sesión en la instancia de zona protegida de Marketo.

1. Vaya a **Administrador**.

1. Seleccione **Perspectiva de ventas**.

1. Seleccione **Configuración de acciones**.

   >[!IMPORTANT]
   >
   >Una dirección de correo electrónico solo se puede utilizar para una instancia de acciones en las instancias Sandbox y Production. Si es un administrador que necesitará acceso a varias instancias en Producción y Zona protegida, debe utilizar una dirección de correo electrónico diferente para cada una.

1. En la tarjeta de aprovisionamiento, seleccione el usuario al que desee invitar a su instancia de acciones de información de ventas.

## Activar la instancia de acciones {#activate-your-actions-instance}

La instancia de acciones deberá activarse con una cuenta de producción de Salesforce. Una vez activado, se puede cambiar a una cuenta de zona protegida de Salesforce.

1. Busque la invitación enviada.

1. Haga clic en el vínculo **Introducción**.

1. Actívelo con su instancia de Producción de Salesforce.

1. Siga las indicaciones para configurar la cuenta. Para obtener una descripción detallada, consulte nuestro [artículo de incorporación de usuarios](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Prepare la instancia de acciones para que sea compatible con la instancia de zona protegida de Salesforce {#prepare-your-actions-instance}

Las acciones requieren que active primero una nueva instancia con un usuario de producción de Salesforce. Una vez activada, puede seguir los siguientes pasos para preparar su instancia para que sea compatible con la zona protegida de Salesforce.

1. Actualice la configuración de inicio de sesión a &quot;Todos los métodos de inicio de sesión&quot;, para que pueda iniciar sesión con un nombre de usuario y una contraseña si es necesario. Si se prefiere, se puede volver a cambiar a &quot;Solo Salesforce&quot; después de configurar todo. [Vea cómo hacer esto aquí](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Desconéctese de Salesforce Production y conéctese a su zona protegida de Salesforce. [Vea cómo conectarse aquí](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. En el paso 3, seleccione &quot;Entorno aislado&quot; en lugar de &quot;Salesforce&quot;. Si ya está conectado, debería ver una opción para desconectarse en la pestaña Conexiones y personalizaciones de Salesforce.

>[!NOTE]
>
>Si tiene un dominio personalizado para la instancia de Salesforce, le recomendamos que inicie sesión en la instancia de Salesforce antes de conectarse a Salesforce o iniciar sesión en Actions.

## Solicite la conversión de la instancia de acciones para que sea compatible con la zona protegida de Salesforce {#request-your-actions-instance-be-converted}

1. Póngase en contacto con el [Soporte técnico del Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para solicitar que su nueva instancia de acciones de información de ventas se configure para que sea compatible con la zona protegida de Salesforce.

1. Pruebe que todo está configurado correctamente intentando iniciar sesión con el botón &quot;Iniciar sesión con Salesforce&quot; de la página toutapp.com/login.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Si tiene algún problema en este momento, puede solicitar un restablecimiento de contraseña y usar una contraseña para recuperar el acceso a su cuenta.

Ahora la instancia está lista para utilizarse con la instancia de zona protegida de Salesforce. Si quieres usar [Inicio de sesión automático de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} desde Salesforce, puedes volver a cambiar a &quot;Solo Salesforce&quot; en tu [configuración de Administración de inicio de sesión](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Conecte su cuenta de acciones de información de ventas a Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Guía de incorporación del usuario de acciones de Sales Insight](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Inicio de sesión automático desde Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Configuración de administración de inicio de sesión](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
