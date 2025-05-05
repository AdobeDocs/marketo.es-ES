---
unique-page-id: 12983280
description: 'Notas De La Versión, Otoño De 2017: Documentos De Marketo: Documentación Del Producto'
title: Notas de la versión, otoño de 2017
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---

# Notas de la versión: otoño de 2017 {#release-notes-fall}

Las siguientes funciones se incluyen en la versión de otoño de 1717. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos del título para ver los artículos detallados de cada función. Nota: Algunas de las funciones incluidas en esta versión no tienen artículos asociados. Si un tema tiene varios subencabezados, los vínculos se colocan allí.

## Fiabilidad del sistema {#system-reliability}

Hemos realizado más mejoras en la infraestructura principal de Marketo, incluida una mejor secuenciación, menos discrepancias y una mayor estabilidad en Munchkin.

## Rendimiento de sincronización de SFDC {#sfdc-sync-performance}

Aproveche la sincronización más rica y rápida entre Marketo y Salesforce. Los cambios de datos que requieren actualizaciones masivas en cuentas o posibles clientes se pueden dividir en colas paralelas para evitar atrasos. Los eventos y las tareas ahora también se sincronizan hasta un 50 % más rápido.

## Mejoras de rendimiento de Analytics {#analytics-performance-improvements}

Las mejoras recientes de la infraestructura ofrecen un mayor tiempo de actividad y estabilidad dentro de las herramientas de análisis e informes de Marketo, lo que le permite crear informes ad hoc más rápidamente.

## [Zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Con esta nueva función, ahora puede retener y enviar correos electrónicos según las zonas horarias locales. Los programas de correo electrónico y participación se pueden configurar para que se entreguen en los husos horarios de los destinatarios, lo que elimina la necesidad de crear varios programas: enviar una vez y Marketo retendrá automáticamente el correo electrónico hasta la hora local correcta. Levante las métricas de correo electrónico, observe las prácticas locales y ahorre tiempo gracias al uso de un solo programa a nivel global.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si todavía no puedes habilitar la Zona horaria del destinatario en tus programas de correo electrónico y participación, ¡no te asustes! Estamos habilitando gradualmente esta función para todos los clientes.

## [Revisar correos electrónicos de muestra por segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo tiene una nueva opción para elegir un segmento al enviar correos electrónicos de muestra para su revisión. Ya no es necesario determinar manualmente a qué segmento pertenece un posible cliente, lo que facilita el envío de correos electrónicos con contenido dinámico a diferentes segmentos.

## [Preguntas personalizadas de LinkedIn Lead Gen](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalice los formularios de LinkedIn Lead Gen para recopilar atributos de posibles clientes personalizados. Ahora puede hacer hasta tres preguntas personalizadas por formulario, elegir entre preguntas de una sola línea o de opción múltiple y volver a asignar a los campos de posible cliente de Marketo.

## Integración de Slack {#slack-integration}

Hemos lanzado dos funciones como parte de nuestra nueva integración de Slack:

* Notificaciones del sistema: obtenga notificaciones del Slack sobre eventos importantes en su instancia de Marketo, como alertas sobre estados de campañas actuales y cualquier problema que requiera atención inmediata.
* Momentos interesantes: Cuando una persona conocida activa una perspectiva de Marketo desde una cuenta de ventas, los propietarios del posible cliente pueden recibir notificaciones a través del Slack. Las notificaciones incluyen información sobre posibles clientes y sobre la cuenta de ventas.

## Mejoras de ABM {#abm-enhancements}

**[Mostrar cuentas sin contactos](https://docs.marketo.com/x/fKCt)**

Marketo ABM ahora sincroniza y muestra cuentas de CRM sin contactos. Incluya nuevas cuentas sin historial de ventas o marketing anterior y rastree el progreso haciendo coincidir los posibles clientes subsiguientes con las cuentas.

## ContentAI Analytics {#contentai-analytics}

**[Nuevo filtro de lista de cuenta ABM](https://docs.marketo.com/x/1BPG)**

Vea y compare el rendimiento del contenido en las listas de cuentas de ABM para optimizar el contenido existente. ContentAI le muestra:

* contenido principal visualizado
* contenido convertido superior
* Contenido sugerido con tecnología de IA para actividades de marketing

## Mejoras de Web Personalization {#web-personalization-enhancements}

**[Tokens para campañas web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Los tokens ya están disponibles para su uso en campañas web. Aproveche los tokens para ofrecer mensajes y contenido personalizados y aumentar la participación en sus campañas web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Imágenes de Design Studio en el editor de campañas web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Ahorre tiempo reutilizando recursos e imágenes creativos en varios canales dentro de Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integración  {#integration}

**[API de vista previa de correo electrónico](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/email-scripting)**

Ahora puede previsualizar de forma remota el correo electrónico fuera de Marketo, lo que simplifica el proceso de localización del contenido del correo electrónico y reduce los errores.

**[Reemplazar API de HTML](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/email-scripting)**

Los desarrolladores pueden actualizar el contenido de los recursos de correo electrónico del HTML de forma remota, lo que les permite trabajar dentro de un solo sistema para mantener los recursos.
