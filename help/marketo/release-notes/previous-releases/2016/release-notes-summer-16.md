---
unique-page-id: 11380218
description: 'Notas de la versión, verano de 2016, documentación de Marketo: documentación del producto'
title: Notas de la versión, verano de 2016
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
feature: Release Information
source-git-commit: 5e2d1979abcafd8e4a37e55b843be932125c954e
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Notas de la versión: Verano de 2016 {#release-notes-summer}

Las siguientes funciones se incluyen en la versión de verano de 16. Compruebe la disponibilidad de las funciones en Marketo Edition. Haga clic en los vínculos del título para ver los artículos detallados de cada función.

## [Marketing basado en cuentas](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

El marketing basado en cuentas de Marketo proporciona todos los elementos esenciales en una sola plataforma:

* **Target** - Descubrimiento de cuentas, coincidencia de clientes potenciales con cuentas y listas de cuentas con nombre
* **Participación** : personalización basada en cuentas, participación en canales múltiples y flujos de trabajo específicos de la cuenta
* **Medida** - Perspectivas a nivel de cuenta y lista, Puntuación de participación en la cuenta e Impacto en la canalización e ingresos

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM está disponible como complemento de su suscripción a Marketo, por lo que debe ponerse en contacto con su representante de ventas para implementarlo.

## [Pista de auditoría](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

La pista de auditoría proporciona un historial completo de los cambios realizados en la suscripción de Marketo. Creará responsabilidad entre usuarios y administradores, ayudará a identificar la causa de comportamientos inesperados y proporcionará la seguridad de saber quién hace qué y cuándo. Esta información estará disponible en cualquier momento y se puede utilizar para responder preguntas como las siguientes:

* ¿Qué ha pasado con este recurso o configuración y quién lo actualizó por última vez?
* ¿Qué ha estado haciendo el usuario X?
* ¿Quién inicia sesión en nuestra cuenta?

![](assets/audit-trail.png)

## [Integración de LaunchPoint de SMS de Marketo-Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Cree fácilmente mensajes SMS dentro de Marketo. Personalice y segmente su mensaje con los datos de Marketo enriquecidos y supervise fácilmente su rendimiento con el panel de mensajes SMS.

>[!NOTE]
>
>Esta función requiere que tenga una cuenta de SMS de Vibes.

![](assets/vibes-sms2.png)

## [Mejoras de Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variables de nivel de módulo**

Anteriormente, todas las variables especificadas en las plantillas de correo electrónico 2.0 tenían un ámbito &quot;global&quot;. Cuando se utilizan variables dentro de los módulos, esto no siempre es deseable si planea utilizar varias instancias del módulo. Con esta versión, las variables ahora se pueden especificar como &quot;nivel de módulo&quot;, lo que le permite indicar que el usuario debe poder establecer valores únicos para cada módulo en el que se utilicen.

![](assets/module-level-variables.png)

**Actualizaciones de sintaxis**

* Ahora puede utilizar &quot;mktoAddByDefault&quot; en los módulos especificados en las plantillas de correo electrónico 2.0 para indicar qué módulos deben mostrarse en los nuevos correos electrónicos de forma predeterminada. Esto resulta mucho más práctico si crea una plantilla de correo electrónico con una gran cantidad de módulos.
* En los elementos de imagen, ahora puede especificar si la variable subyacente `<img>` Las propiedades &quot;height&quot; y &quot;width&quot; del elemento HTML deben estar bloqueadas o ser editables para el usuario final. mktoLockImgSize=&quot;true&quot; hará que el alto/ancho se bloquee (incluso si se cambia la imagen). Del mismo modo, mktoLockImgStyle=&quot;true&quot; hará que la propiedad &quot;style&quot; se bloquee.

**Búsqueda de código**

Utilice la nueva funcionalidad de búsqueda para buscar y reemplazar contenido de forma eficaz dentro del código del correo electrónico. Esta funcionalidad también está disponible en el editor de plantillas de correo electrónico.

![](assets/2nd-screenshot.png)

**Compatibilidad con tokens en elementos de imagen**

Ahora, los tokens se pueden utilizar en el área &quot;URL externa&quot; de la experiencia de inserción de imágenes. Si ha especificado imágenes con `{{my.tokens}}`Ahora puede hacer referencia a estos tokens en el Editor de correo electrónico 2.0. Tenga en cuenta que la imagen seguirá apareciendo rota en el lienzo del Editor de correo electrónico 2.0. Sin embargo, los verá procesados en Vista previa y Enviar muestra antes de enviar el correo electrónico.

## Varios dominios de personalización de marca {#multiple-branding-domains}

Se acabaron los días en que los vínculos de seguimiento de correo electrónico solo se podían añadir a un único dominio de marca. Ahora puede añadir varios dominios de promoción de la marca para inspirar confianza en los consumidores, crear una apariencia más optimizada para centrarse en la marca, mejorar la capacidad de envío de correos electrónicos y elegir, por correo electrónico, el dominio de promoción de la marca que se utilizará para los vínculos de seguimiento de cada correo electrónico.

![](assets/multiple-branding-domains.png)

## [Tokens de programa](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Hemos creado un nuevo tipo de token para los programas. Ahora puede procesar Nombre, Descripción e ID del programa en los pasos de flujo de recursos y campañas inteligentes.

![](assets/program-tokens.png)

## [Clave de empresa](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Requerir que cada persona de su equipo de ventas instale nuestro complemento de perspectiva de ventas para Outlook puede ser tedioso. Hemos introducido una nueva forma de instalar el complemento para Outlook de forma remota mediante una clave empresarial. Envíe a su equipo de TI la clave única que se encuentra en la sección de Perspectivas de ventas de Marketo de Admin y déjeles hacer el resto.

![](assets/enterprise-key.png)

## [Campañas de personalización web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Especifique un retraso para que las campañas web reaccionen en el sitio web.

![](assets/dialog-campaign-delay.png)

## [Exportación de análisis de contenido y Recommendations](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Ver datos de análisis de contenido y recomendaciones sin conexión.

## [Compatibilidad con API para el editor de correo electrónico 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Las API de recursos preexistentes, que anteriormente solo eran compatibles con las plantillas y los correos electrónicos de la versión 1.0, ahora están habilitadas para los recursos de correo electrónico de la versión 2.0.

## [Sitio para desarrolladores de Marketo](https://developers.marketo.com/) {#marketo-developers-site}

Nuevo y mejorado

## [Configuración de privacidad](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Los especialistas en marketing pueden utilizar la configuración de privacidad para decidir si desean rastrear o no a los visitantes mediante las funciones de Munchkin y Personalización web. El nivel de seguimiento se controla mediante la configuración No rastrear del explorador, una cookie de exclusión o una IP no específica. Estos métodos pueden afectar al valor y la funcionalidad de Marketo en áreas específicas, pero si el experto en marketing no cambia nada, la funcionalidad de Marketo permanece igual.

Esta función se lanzará gradualmente a los clientes durante un periodo de seis semanas. Si lo necesita de inmediato, póngase en contacto con el Soporte técnico de Marketo.
