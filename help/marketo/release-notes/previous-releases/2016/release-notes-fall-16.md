---
unique-page-id: 11384018
description: 'Notas De La Versión, Otoño De 2016: Documentos De Marketo: Documentación Del Producto'
title: Notas de la versión, otoño de 2016
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 2b72932606a93d061eb2f57c0ff3256b94a0c20c
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Notas de la versión: otoño de 2016 {#release-notes-fall}

Las siguientes funciones se incluyen en la versión de otoño de 1616. Compruebe la disponibilidad de las funciones en Marketo Edition. Haga clic en los vínculos del título para ver los artículos detallados de cada función.

## [!UICONTROL Contenido predictivo] en el correo electrónico {#predictive-content-in-email}

Hay una nueva experiencia de usuario para nuestra aplicación [!UICONTROL Contenido predictivo] que permite rastrear, administrar y recomendar su contenido a través de nuestro aprendizaje automático y algoritmos predictivos en los canales web y de correo electrónico.

>[!NOTE]
>
>Todos los clientes con el módulo Predictive estarán habilitados el 10 de enero.

![](assets/shafe.png)

Ahora puede añadir contenido predictivo al correo electrónico. Cuando se abre el correo electrónico, el destinatario recibe automáticamente contenido relevante recomendado que ayuda a aumentar la participación y las conversiones del contenido.

![](assets/predictive.png)

## [Conversiones de Facebook sin conexión](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Con la integración de [!DNL Facebook] conversiones sin conexión, los datos de conversión en Marketo (para posibles clientes con publicidad) se envían automáticamente de vuelta a [!DNL Facebook] para que su equipo de publicidad pueda optimizar mejor su gasto en publicidad. En este informe de administrador de anuncios [!DNL Facebook], se resaltan las conversiones sin conexión.

![](assets/facebook.png)

## [Id. universal](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un ID universal le permite acceder a varias suscripciones de Marketo con un solo inicio de sesión y cambiar entre suscripciones rápidamente. Puede utilizar un único perfil de comunidad para todas las suscripciones.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Póngase en contacto con el Soporte técnico de Marketo para habilitar esta función.

## Mejoras de marketing basado en cuentas de Marketo {#marketo-account-based-marketing-enhancements}

Ahora puede asignar equipos de cuentas a cuentas con nombre en Marketing basado en cuentas (ABM), por ejemplo, propietario de cuenta, representante de desarrollo de ventas, representante de desarrollo empresarial y administrador de éxito de clientes. También puede crear listas de cuentas específicas del propietario de la cuenta y enviar informes personalizados de ABM semanales al equipo de la cuenta.

![](assets/account-team-11-15-16.png)

**API DE REST**

Esta versión también le permite administrar atributos de cuenta con nombre y puntuaciones de cuentas en ABM mediante la API de REST de Marketo. Para obtener más información sobre las operaciones de la API, visite el [sitio web de desarrolladores de Marketo](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Mejoras en la pista de auditoría](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

La pista de auditoría proporciona un historial completo de los cambios realizados en la suscripción de Marketo. Hemos agregado funcionalidades de seguimiento adicionales para programas, así como detalles importantes sobre cambios para campañas inteligentes, listas inteligentes y cambios realizados en usuarios y funciones.

## Nuevos permisos

**Poner el correo electrónico en funcionamiento**

Se acabaron los días en los que tenía que preocuparse por los usuarios que enviaban correos electrónicos transaccionales a personas de la base de datos que habían cancelado la suscripción. Ahora puede especificar qué usuarios pueden hacer que un correo electrónico sea operativo o editar correos electrónicos operativos.

**Editar restricciones de campaña**

¿Por qué establecer [restricciones de campaña](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) si no puede aplicarlas? Cuando establece la Configuración de límite de campaña para restringir el número de personas en la base de datos a las que se puede dirigir con una sola campaña, ahora puede restringir qué usuarios pueden anular esta configuración al programar una campaña.

## [Sonido para notificaciones push móviles](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Aporte mayor riqueza a las notificaciones push de iOS habilitando el sonido. Esta nueva función le permite almacenar en déclencheur un sonido cuando las notificaciones push se muestran en el dispositivo móvil.

>[!NOTE]
>
>* Los propietarios de dispositivos pueden optar por evitar que los sonidos se reproduzcan en la configuración del dispositivo, y los desarrolladores de aplicaciones pueden proporcionar a los propietarios de dispositivos opciones dentro de la aplicación para evitar que se reproduzcan sonidos.
>* Los sonidos se reproducen automáticamente cuando se muestra una notificación push en un dispositivo Android.

![](assets/sound-for-push-notifications.png)

## [Insight de ventas compatible con Salesforce Encryption](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market [!DNL Sales Insight] ahora es compatible con cifrado de escudo [!DNL Salesforce]. Todos los clientes de [!DNL Sales Insight] deben actualizar a este último paquete administrado (versión 1.4359.2), que está [disponible en el [!DNL Appexchange]](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API de cuentas con nombre](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Con esta versión, los usuarios de Marketo ABM pueden administrar cuentas con nombre a través de la API de Cuentas con nombre. Los usuarios pueden crear, actualizar y eliminar cuentas con nombre, así como leer y actualizar las puntuaciones de cuentas con nombre de ABM.

## [Compatibilidad con la API del Editor de correo electrónico v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Administre variables y módulos para correos electrónicos en formato v2.0 mediante la API de REST de Marketo.

## [Cambios en la sincronización de Marketo Salesforce](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

La integración de [!DNL Salesforce] de Marketo está evolucionando para mejorar la forma en que los campos de Marketo se sincronizan con [!DNL Salesforce]. Ahora, en lugar de tener que sincronizar un grupo grande de campos que puede que necesite o no, puede elegir qué campos desea incluir. Consulte nuestra documentación aquí para obtener más información: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
