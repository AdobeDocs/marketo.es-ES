---
description: 'Notas de la versión, agosto de 2021: Documentos de Marketo: documentación del producto'
title: Notas de la versión, agosto de 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Notas de la versión: agosto de 2021 {#release-notes-aug-21}

Las siguientes funciones están incluidas en la versión de agosto de 2021 de. Consulte en la edición de Marketo Engage la disponibilidad de las funciones.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Adobe Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características se lanzarán el **20 de agosto de 2021**.

## Automatización de experiencias {#experience-automation}

* **Autenticación de usuario Marketo Engage mediante identidad de Adobe**: Pronto se incorporarán nuevos usuarios Marketo Engage con paquetes Enterprise mediante las credenciales de usuario Adobe ID. La migración de los usuarios actuales al sistema de identidad integrado no se producirá hasta mediados de 2022 y no se requiere ninguna acción hasta nuevo aviso. La autenticación de usuarios de identidad de Adobe permite a los administradores de TI/seguridad administrar varias instancias de productos de Marketo Engage junto con otras soluciones de Experience Cloud, así como configurar el SSO a través de una consola común. Los administradores pueden administrar de forma práctica los grupos de usuarios y las autorizaciones de usuario en un solo lugar.

* **Anidado de campañas ejecutables**: Las campañas ejecutables ahora también pueden llamar a otras campañas ejecutables, lo que le permite anidarlas hasta en tres niveles. Esto permite una mayor consolidación de los flujos operativos comunes y mejora la administración de campañas inteligentes.

* **Acción de flujo única en la página de detalles de persona** (disponible para el 9 de septiembre): ejecute acciones de flujo como enviar correo electrónico, cambiar el propietario de la persona o cualquier otra acción de campaña inteligente en personas individuales desde la página de detalles de la persona mediante el menú de acciones de flujo sin cambiar a la vista de cuadrícula de la base de datos.

* **[Exportación de actividades personalizadas](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: la exportación de metadatos ahora admite todos los objetos y metadatos respectivos que se pueden usar para compartir, analizar y diseñar el modelo de datos de suscripción.

## Mejoras de API {#api-enhancements}

* **Enviar formulario API**: Cuando una dirección de correo electrónico está duplicada en dos o más registros de posibles clientes, actualizamos el registro &quot;última actualización&quot; en lugar de omitirlo por completo. Proporciona paridad con la API de Forms 2.0.

* **API de correo electrónico**: recupera los recursos de correo electrónico del campeón o aspirante. Recupere recursos de correo electrónico mediante el filtro de intervalo de fechas.

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Visibilidad mejorada de las actividades de cliente potencial, contacto, cuenta y oportunidad para los usuarios de CRM de Salesforce**: la participación con clientes potenciales durante largos ciclos de ventas está más informada debido al mayor número de registros de participación en la perspectiva de ventas. Las pestañas Momentos interesantes, Actividad web, Correo electrónico y Puntuación muestran hasta 400 actividades en los objetos Posible cliente, Contacto, Cuenta y Oportunidad.

## Sales Connect {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Restricción de la conexión de correo electrónico (Beta)**: mejore la capacidad de envío de correo electrónico y escale la comunicación de ventas personalizada con la limitación de la conexión de correo electrónico para Sales Connect. Esta nueva tecnología administra automáticamente el tiempo de envío del correo electrónico para crear experiencias sin problemas para los usuarios de Exchange y Gmail. Reduzca o elimine el uso de aplicaciones de envío masivo de correo electrónico de terceros y envíe todos sus correos electrónicos desde Sales Connect con confianza.

>[!NOTE]
>
>La restricción de correo electrónico ya está disponible en Beta. [Más información](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Perspectivas de actividad de ventas mejoradas**: capture y active la participación personalizada en función de las actividades anteriores de su equipo de ventas. Los nuevos atributos, como el vínculo de registro de llamadas de ventas, el nombre de la campaña de ventas y el asunto del correo electrónico de ventas, se pueden usar en las listas inteligentes de Marketo Engage.  Estas actividades se pueden exportar e informar a través de la API de REST de Marketo Engage o de Exportación masiva y están disponibles en filtros y déclencheur como restricciones adicionales para listas inteligentes.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integración Forms de generación de clientes potenciales de LinkedIn de Bizible**: los especialistas en marketing ahora pueden realizar la atribución de ingresos en las conversiones que se producen cuando LinkedIn captura los formularios que se rellenan a través de sus unidades de anuncios Forms de generación de clientes potenciales. Estas perspectivas se pueden utilizar para optimizar el rendimiento del formulario y las inversiones en medios de pago. LinkedIn Lead Gen Forms es una de las ofertas de medios de pago de más rápido crecimiento de LinkedIn y esta nueva capacidad se incluye con nuestra integración existente de LinkedIn Ads con Bizible.

* **Tablero de velocidad mejorado**: Hemos agregado una nueva métrica de velocidad y un filtro de tablero para obtener información más detallada. Los especialistas en marketing utilizan este tablero para comprender la velocidad de posible cliente y de oportunidad paso a paso y la eficiencia de las diferentes formas de participación de marketing y ventas.

* **Nuevo panel de Recorrido de cascada de cohorte**: esto permitirá a los especialistas en marketing ver la progresión de una cohorte seleccionada a través de un conjunto de etapas de &quot;cascada de demanda&quot; clásica, lo que proporciona una comprensión rápida de las tasas de conversión y la causalidad de conversión de etapa implícita en cada etapa.

## Integración de Bizible con Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Esta sección incluye nuevas funciones para los usuarios de Bizible que han completado su migración a Adobe Identity Management System (IMS). Si ha migrado, verá su nuevo Adobe ID en Configuración de Bizible en la pestaña Adobe ID. Todas las cuentas deberían migrarse para finales de 2021.

* **Integración de Bizible con el Privacy Service de Adobe** (disponible en septiembre de 2021): La integración de Bizible con el Privacy Service de Adobe centraliza el cumplimiento de las regulaciones críticas de privacidad de datos (como el RGPD) en todas las aplicaciones de Adobe Experience Cloud. Ahora puede aprovechar este servicio y administrar todas las solicitudes de privacidad de forma centralizada para que las solicitudes de cambio que llegan a Bizible y otros productos de Adobe se reflejen en todas las aplicaciones.

* **Bizible en la interfaz de Adobe Experience Cloud**: la adopción de la interfaz de Adobe Experience Cloud por parte de Bizible ofrece a los usuarios nuevas funciones que aparecerán en la barra de encabezado de la aplicación Bizible e incluirán un mejor acceso a los recursos de soporte y a la conmutación de aplicaciones. La interfaz de Experience Cloud ayuda a crear una experiencia coherente entre Bizible y otras aplicaciones de Adobe Experience Cloud.

* **Propiedad y autoadministración de dominios de Bizible**: Los usuarios de Bizible pueden aprovechar Adobe Admin Console para administrar los dominios que desean que Bizible rastree. Esto lleva el autoservicio a un proceso anteriormente manual y proporciona una experiencia coherente en la forma en que la propiedad del dominio y el seguimiento se administran en las aplicaciones de Adobe Experience Cloud.

## Anuncios {#announcements}

* **Actualizar la configuración del identificador universal de suscripción**: para admitir la próxima integración de Marketo Engage e identidad de Adobe para los usuarios existentes, todas las suscripciones de Marketo Engage se unificarán para habilitar la compatibilidad con el identificador universal. Encontrará más información [aquí](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de agosto de 2021](https://engage.marketo.com/August21_Release_Webinar.html)
