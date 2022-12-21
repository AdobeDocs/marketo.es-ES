---
unique-page-id: 11384018
description: Notas de la versión - Otoño del 16 - Documentos de Marketo - Documentación del producto
title: Notas de la versión - Otoño del 2016
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Notas de la versión: Otoño del 16 {#release-notes-fall}

Las siguientes funciones están incluidas en la versión del 16 de otoño. Compruebe la disponibilidad de las funciones en su edición de Marketo. Haga clic en los vínculos de título para ver los artículos detallados de cada función.

## Contenido predictivo en correo electrónico {#predictive-content-in-email}

Hay una nueva experiencia de usuario para que nuestra aplicación de contenido predictivo rastree, administre y recomiende su contenido a través de nuestro aprendizaje automático y algoritmos predictivos en la web y los canales de correo electrónico.

>[!NOTE]
>
>Todos los clientes con el módulo Predictive estarán habilitados para el 10 de enero.

![](assets/shafe.png)

Ahora puede añadir contenido predictivo al correo electrónico. Cuando se abre el correo electrónico, el destinatario recibe automáticamente el contenido relevante y recomendado que ayuda a aumentar la participación en el contenido y las conversiones.

![](assets/predictive.png)

## [Conversiones sin conexión de facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Con la integración de conversiones sin conexión de Facebook, los datos de conversión en Marketo (para posibles clientes de anuncios de posibles clientes) se envían automáticamente a Facebook para que su equipo de publicidad pueda optimizar mejor su gasto en publicidad. En este informe de Facebook Ad Manager, se resaltan las conversiones sin conexión.

![](assets/facebook.png)

## [ID universal](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un ID universal le permite acceder a varias suscripciones a Marketo con un solo inicio de sesión y cambiar rápidamente entre suscripciones. Puede utilizar un solo perfil de comunidad para todas sus suscripciones.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Póngase en contacto con el servicio de asistencia técnica de Marketo para habilitar esta función.

## Mejoras de marketing basadas en cuentas de Marketo {#marketo-account-based-marketing-enhancements}

Ahora, puede asignar equipos de cuenta a cuentas con nombre en Marketing basado en cuentas (ABM), por ejemplo, propietario de cuenta, representante de desarrollo de ventas, representante de desarrollo empresarial y administrador de éxito de clientes. También puede crear listas de cuentas específicas del propietario de la cuenta y enviar informes ABM semanales personalizados al equipo de la cuenta.

![](assets/account-team-11-15-16.png)

**API de REST**

Esta versión también le permite administrar atributos de cuenta con nombre y puntuaciones de cuentas en ABM mediante la API de REST de Marketo. Para obtener más información sobre las operaciones de la API, visite [Sitio web de desarrolladores de Marketo](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Mejoras en la pista de auditoría](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

La pista de auditoría ofrece un historial completo de los cambios realizados en la suscripción a Marketo. Hemos añadido funciones de seguimiento adicionales para programas, así como detalles importantes sobre cambios para campañas inteligentes, listas inteligentes y cambios realizados a usuarios y funciones.

## [Nuevos permisos](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**Hacer operativo el correo electrónico**

Atrás quedaron los días en los que tuvo que preocuparse de que los usuarios enviaran correos electrónicos transaccionales a personas de la base de datos que han cancelado la suscripción. Ahora puede especificar qué usuarios pueden hacer que un correo electrónico sea operativo o editar los correos electrónicos operativos.

**Editar restricciones de campaña**

Por qué establecer [restricciones de campaña](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) ¿si no puede aplicarlos? Al establecer la configuración de límites de campaña para restringir el número de personas de la base de datos que pueden ser objetivo de una sola campaña, ahora puede restringir qué usuarios pueden anular esta configuración al programar una campaña.

## [Sonido para notificaciones push móviles](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Añada riqueza a la notificación push de iOS al habilitar el sonido. Esta nueva función le permite almacenar en déclencheur un sonido cuando se muestra la notificación push en el dispositivo móvil.

>[!NOTE]
>
>* Los propietarios de dispositivos pueden optar por evitar que se reproduzcan sonidos en la configuración del dispositivo, y los desarrolladores de aplicaciones pueden ofrecer a los propietarios de dispositivos opciones dentro de la aplicación para evitar que se reproduzcan sonidos.
>* Los sonidos se reproducen automáticamente cuando se muestra una notificación push en un dispositivo Android.


![](assets/sound-for-push-notifications.png)

## [Perspectiva de ventas compatible con el cifrado de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Ahora, Market Sales Insight es compatible con Salesforce Shield Encryption. Todos los clientes de Sales Insight deben actualizar a este último paquete administrado (versión 1.4359.2), que es [disponible en Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API de cuentas con nombre](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Con esta versión, los usuarios de ABM de Marketo pueden administrar cuentas con nombre a través de la API de cuentas con nombre. Los usuarios pueden crear, actualizar y eliminar cuentas con nombre, así como leer y actualizar las puntuaciones de cuenta con nombre ABM.

## [Compatibilidad con la API del Editor de correo electrónico v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Administre variables y módulos para correos electrónicos en formato v2.0 mediante la API de REST de Marketo.

## [Cambios en Marketo Salesforce Sync](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

La integración de Salesforce de Marketo está evolucionando para mejorar la forma en que los campos de Marketo se sincronizan con Salesforce. Ahora, en lugar de tener que sincronizar un grupo grande de campos que puede que necesite o no, puede elegir qué campos desea incluir. Consulte nuestra documentación aquí para obtener más información: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
