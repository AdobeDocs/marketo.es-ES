---
unique-page-id: 12983280
description: Notas de la versión - Otoño '17 - Documentos de marketing - Documentación del producto
title: Notas de la versión - Otoño de 2017
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---


# Notas de la versión: Otoño &#39;17 {#release-notes-fall}

Las siguientes funciones se incluyen en la versión del 17 de otoño. Compruebe la disponibilidad de las funciones en la edición de marketing.

Haga clic en los vínculos de título para vista de artículos detallados para cada función. Nota: Algunas de las funciones incluidas en esta versión no tienen artículos asociados. Si un tema tiene varios subtítulos, los vínculos se colocan allí.

## Fiabilidad del sistema {#system-reliability}

Hemos realizado mejoras en la infraestructura central de Marketing, incluyendo mejor secuenciación, menos desajustes y una mejor estabilidad de Munchkin.

## Rendimiento de sincronización de SFDC {#sfdc-sync-performance}

Aproveche una sincronización más rápida y enriquecida entre Marketing y Salesforce. Los cambios de datos que requieren actualizaciones masivas en cuentas o posibles clientes pueden dividirse en colas paralelas para evitar los retrasos. Los eventos y tareas ahora también se sincronizan hasta un 50 % más rápido.

## Mejoras en el rendimiento de Analytics {#analytics-performance-improvements}

La oferta de las mejoras recientes en la infraestructura ha aumentado el tiempo de actividad y la estabilidad dentro de las herramientas de análisis y sistema de informes de marketing, lo que le permite crear informes ad hoc con mayor rapidez.

## [Huso horario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Con esta nueva función, ahora puede mantener y enviar correos electrónicos según los husos horarios locales. Los programas de correo electrónico y participación se pueden configurar para que se entreguen en las zonas horarias de los destinatarios, lo que elimina la necesidad de crear varios programas: enviar una vez y Marketo retendrá automáticamente el correo electrónico hasta la hora local correcta. Alza las métricas de correo electrónico, observa las prácticas locales y ahorra tiempo usando un solo programa globalmente.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si todavía no puede activar el huso horario de Destinatario en sus programas de correo electrónico y participación, no se asuste. Esta función se está activando gradualmente para todos los clientes.

## [Revisar correos electrónicos de muestra por segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo tiene una nueva opción para elegir un segmento al enviar correos electrónicos de muestra para su revisión. Ya no es necesario determinar manualmente a qué segmento pertenece un posible cliente, lo que facilita el envío de correos electrónicos que contengan contenido dinámico a diferentes segmentos.

## [Preguntas personalizadas sobre LinkedIn Lead Gen](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalice los formularios de generación de posibles clientes de LinkedIn para recopilar atributos de posibles clientes personalizados. Ahora puede hacer hasta tres preguntas personalizadas por formulario, elegir entre una entrada de texto de una sola línea o preguntas de opción múltiple, y volver a asignar a los campos de posibles clientes de Marketing to.

## [Integración de Slack](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Hemos lanzado dos funciones como parte de nuestra nueva integración de Slack:

* Notificaciones del sistema: Reciba notificaciones de Slack sobre eventos importantes en la instancia de Marketing, como alertas sobre estados de campaña actuales y cualquier problema que requiera atención inmediata.
* Momentos interesantes: Cuando una perspectiva de marketing se activa por un individuo conocido desde una cuenta de ventas, los propietarios de clientes potenciales pueden recibir una notificación por medio de un Slack. Las notificaciones incluyen información sobre los posibles clientes, así como detalles sobre la cuenta de ventas.

## Mejoras de ABM {#abm-enhancements}

**[Mostrar cuentas sin contactos](https://docs.marketo.com/x/fKCt)**

Marketo ABM ahora sincroniza y muestra cuentas CRM sin contactos. Incluya nuevas cuentas sin ventas ni historiales de marketing anteriores y rastree el progreso haciendo coincidir los posibles clientes subsiguientes con las cuentas.

## ContentAI Analytics {#contentai-analytics}

**[Nuevo filtro de Lista de cuenta ABM](https://docs.marketo.com/x/1BPG)**

Vista y compare el rendimiento del contenido en las Listas de cuentas ABM para optimizar el contenido existente. ContentAI le muestra:

* contenido más visto
* contenido convertido principal
* Contenido sugerido por AI para actividades de marketing

## Mejoras en la personalización de Web {#web-personalization-enhancements}

**[Tokens para Campañas web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Los tokens ahora están disponibles para su uso en campañas web. Aproveche los tokens para ofrecer contenido y mensajes personalizados a fin de aumentar la participación en sus campañas web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Diseño de imágenes de Studio en el Editor de Campañas web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Ahorre tiempo reutilizando elementos creativos e imágenes en varios canales de Marketing.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integración {#integration}

**[API de Previsualización de correo electrónico](https://developers.marketo.com/rest-api/assets/emails/)**

Ahora puede realizar la previsualización remota del correo electrónico fuera de Marketing, lo que simplifica el proceso de localización del contenido del correo electrónico y reduce los errores.

**[Reemplazar API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Los desarrolladores pueden actualizar el contenido HTML de los recursos de correo electrónico de forma remota, lo que les permite trabajar en un único sistema para mantener los recursos.
