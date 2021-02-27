---
unique-page-id: 11380218
description: Notas de la versión - Verano 16 - Documentos de marketing - Documentación del producto
title: Notas de la versión - Verano 2016
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---


# Notas de la versión: Verano &#39;16 {#release-notes-summer}

Las siguientes funciones se incluyen en la versión del verano de 2016. Compruebe la disponibilidad de las funciones en la edición de marketing. Haga clic en los vínculos de título para vista de artículos detallados para cada función.

## [Mercadotecnia basada en cuenta](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

La mercadotecnia basada en cuentas de marketing proporciona todos los elementos esenciales en una plataforma unificada:

* **Destinatario** : detección de cuentas, coincidencia de posibles clientes con cuentas y Listas de cuentas con nombre
* **Participación** : Personalización basada en cuentas, participación en varios canales y Flujos de trabajo específicos de la cuenta
* **Medición** : perspectivas de nivel de cuenta y Lista, puntuación de participación en la cuenta e impacto en la canalización y los ingresos

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM está disponible como complemento a su suscripción de Marketing, por lo que póngase en contacto con su representante de ventas para que la implemente.

## [Pista de auditoría](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

La pista de auditoría proporciona un historial completo de los cambios realizados en la suscripción de marketing. Creará responsabilidad entre usuarios y administradores, ayudará a identificar la causa de un comportamiento inesperado y garantizará la seguridad de saber quién está haciendo qué y cuándo. Esta información estará disponible en cualquier momento y puede utilizarse para responder preguntas como:

* ¿Qué ha pasado con este recurso o configuración y quién lo actualizó por última vez?
* ¿Qué ha estado haciendo el usuario X?
* ¿Quién está iniciando sesión en nuestra cuenta?

![](assets/audit-trail.png)

## [Integración de LaunchPoint de SMS de Marketo-Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Cree fácilmente mensajes SMS dentro de Marketing. Personalice y destinatario su mensaje con sus datos enriquecidos de Marketing y supervise fácilmente su rendimiento mediante el panel de mensajes SMS.

>[!NOTE]
>
>Esta función requiere que tenga una cuenta de Vibes SMS existente.

![](assets/vibes-sms2.png)

## [Mejoras en Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variables de nivel de módulo**

Anteriormente, todas las variables especificadas en las plantillas de correo electrónico 2.0 tenían un alcance &quot;global&quot;. Cuando se utilizan variables dentro de módulos, esto no siempre es deseable si se planea utilizar varias instancias del módulo. Con esta versión, las variables ahora se pueden especificar como &quot;nivel de módulo&quot;, lo que le permite indicar que el usuario debe poder establecer valores únicos para cada módulo en el que se utilizan.

![](assets/module-level-variables.png)

**Actualizaciones de sintaxis**

* Ahora puede utilizar &quot;mktoAddByDefault&quot; en los módulos especificados en las plantillas de correo electrónico 2.0 para indicar qué módulos deben mostrarse en los nuevos correos electrónicos de forma predeterminada. Esto resulta mucho más práctico si está creando una plantilla de correo electrónico con grandes cantidades de módulos.
* En los elementos de imagen, ahora puede especificar si las propiedades &quot;height&quot; y &quot;width&quot; del elemento HTML subyacente deben bloquearse o editarse para el usuario final. `<img>` mktoLockImgSize=&quot;true&quot; bloqueará la altura y la anchura (incluso si se cambia la imagen). Del mismo modo, mktoLockImgStyle=&quot;true&quot; bloqueará la propiedad &quot;style&quot;.

**Búsqueda de código**

Utilice la nueva funcionalidad de búsqueda para buscar y reemplazar de forma eficaz el contenido del código de correo electrónico. Esta funcionalidad también está disponible en el editor de plantillas de correo electrónico.

![](assets/2nd-screenshot.png)

**Compatibilidad con tokens en elementos de imagen**

Los tokens ahora se pueden usar en el área &quot;URL externa&quot; de la experiencia de inserción de imágenes. Si ha especificado imágenes con `{{my.tokens}}`, ahora puede hacer referencia a estos tokens en el Editor de correo electrónico 2.0. Tenga en cuenta que la imagen seguirá apareciendo rota en el lienzo del Editor de correo electrónico 2.0. Sin embargo, los verá procesados en Previsualización y Enviar muestra antes de enviar su correo electrónico.

## Varios dominios de marca {#multiple-branding-domains}

Atrás quedaron los días en los que los vínculos de seguimiento del correo electrónico solo podían marcarse con un único dominio de marca. Ahora puede agregar varios dominios de marca para inspirar confianza del consumidor, crear un aspecto más optimizado para centrarse en la marca, mejorar la entrega por correo electrónico y elegir, por correo electrónico, qué dominio de marca utilizar para los vínculos de seguimiento de cada correo electrónico.

![](assets/multiple-branding-domains.png)

## [Tokens de programa](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Hemos creado un nuevo tipo de token para programas. Ahora puede procesar Nombre de Programa, Descripción e ID en los recursos y en los pasos del flujo de campaña inteligente.

![](assets/program-tokens.png)

## [Clave de empresa](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Exigir a cada persona del equipo de ventas que instale nuestro complemento de perspectiva de ventas para Outlook puede resultar tedioso. Hemos introducido una nueva forma de instalar el complemento para Outlook de forma remota mediante una clave de empresa. Envíe a su equipo de TI la clave única que encontró en la sección Perspectiva de ventas de marketing de Administración y déjeles hacer el resto.

![](assets/enterprise-key.png)

## [Campañas de personalización web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Especifique un tiempo de espera para que las campañas web reaccionen en el sitio web.

![](assets/dialog-campaign-delay.png)

## [Content Analytics y Recommendations Export](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Datos de recomendaciones y análisis de contenido de vista sin conexión.

## [Compatibilidad de API con el Editor de correo electrónico 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Las API de recursos preexistentes, que anteriormente solo eran compatibles con plantillas y correos electrónicos v1.0, ahora están activadas para los recursos de correo electrónico v2.0.

## [Sitio para desarrolladores de marketing](https://developers.marketo.com/) {#marketo-developers-site}

¡Nuevo y mejorado!

## [Configuración de privacidad](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Los especialistas en marketing pueden utilizar la configuración de privacidad para decidir si rastrear visitantes utilizando las funciones de Munchkin y Personalización web. El nivel de seguimiento se controla mediante la configuración No rastrear del explorador, una cookie de exclusión o una IP no específica. Estos métodos pueden afectar al valor y la funcionalidad de Marketing en áreas específicas, pero si el especialista en mercadotecnia no cambia nada, la funcionalidad de Marketing sigue siendo la misma.

Esta función se lanzará gradualmente a los clientes durante un período de seis semanas. Si lo necesita de inmediato, póngase en contacto con la asistencia técnica de marketing.
