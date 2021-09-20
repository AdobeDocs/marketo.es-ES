---
description: Notas de la versión actuales - Documentos de Marketo - Documentación del producto
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: c6713c972603ab9528a66e908e47e4c187b86c0c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Notas de la versión: Agosto de 2021 {#release-notes-aug-21}

Las siguientes funciones están incluidas en la versión del 21 de agosto. Consulte la edición para su Marketo Engage si hay disponibilidad de funcionalidades.

>[!AVAILABILITY]
>
>Las funciones denotadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage del Adobe para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán el **20 de agosto de 2021**.

## Automatización de la experiencia {#experience-automation}

* **Autenticación de usuario Marketo Engage mediante identidad** de Adobe: Pronto, los nuevos usuarios Marketo Engage con paquetes empresariales se incorporarán mediante las credenciales de usuario de Adobe ID. La migración de los usuarios actuales al sistema de identidad integrado no se producirá hasta mediados de 2022 y no se requiere ninguna acción hasta nuevo aviso. La autenticación de usuarios de identidad de Adobe permite a los administradores de TI/seguridad administrar varias instancias de producto de Marketo Engage junto con otras soluciones de Experience Cloud, así como configurar SSO a través de una consola común. Los administradores pueden administrar fácilmente los grupos de usuarios y las autorizaciones de usuario en un solo lugar.

* **Anidado** de campaña ejecutable: Ahora, las campañas ejecutables también pueden llamar a otras campañas ejecutables, lo que le permite anidarlas hasta con tres niveles de profundidad. Esto permite una mayor consolidación de los flujos operativos comunes y mejora la administración de Smart Campaign.

* **Acción de flujo único en la página de detalles de la persona**  (disponible antes del 9 de septiembre): Ejecute acciones de flujo como enviar correo electrónico, cambiar propietario de persona o cualquier otra acción de campaña inteligente en personas individuales desde la página de detalles de persona mediante el menú de acción de flujo sin cambiar a la vista de cuadrícula de la base de datos.

* **[Exportación](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)** de actividades personalizadas: La exportación de metadatos ahora es compatible con todos los objetos y metadatos respectivos que se pueden utilizar para compartir, analizar y diseñar el modelo de datos de suscripción.

## Mejoras de API {#api-enhancements}

* **Enviar API** de formulario: Cuando una dirección de correo electrónico está duplicada en dos o más registros de posible cliente, actualizamos el registro &quot;última actualización&quot; en lugar de omitirlo por completo. Proporciona paridad con la API de Forms 2.0.

* **API** de correo electrónico: Recupere los recursos de correo electrónico de campeón o aspirante. Recupere los recursos de correo electrónico mediante el filtro de intervalo de fechas.

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Conocimiento de ventas {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Visibilidad mejorada de las actividades de posible cliente, contacto, cuenta y oportunidad para los usuarios** de Salesforce CRM: La participación con los posibles clientes durante los ciclos de ventas largos está más informada debido al aumento del número de registros de participación en la perspectiva de ventas. Momentos interesantes, actividad web, correo electrónico y pestañas de puntuación muestran hasta 400 actividades en los objetos Posibles clientes, Contacto, Cuenta y Oportunidad.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Restricción de la conexión del correo electrónico (Beta)**: Mejore la capacidad de envío de correo electrónico y escale la comunicación de ventas personalizada con la regulación de la conexión de correo electrónico para Sales Connect. Esta nueva tecnología administra automáticamente el tiempo de envío de correo electrónico para crear experiencias sin problemas para los usuarios de Exchange y Gmail. Reduzca o elimine el uso de las aplicaciones de envío masivo de correo electrónico de terceros y envíe todos sus correos electrónicos desde Sales Connect con confianza.

>[!NOTE]
>
>La restricción de correo electrónico ya está disponible en versión beta. [Obtenga más información](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Perspectivas** de actividad de ventas mejoradas: Capture y active la participación personalizada en función de las actividades anteriores del equipo de ventas. En las listas inteligentes del Marketo Engage se pueden utilizar nuevos atributos, como el vínculo de grabación de llamadas de venta, el nombre de campaña de ventas y el asunto del correo electrónico de ventas.  Estas actividades se pueden exportar e informar a través de la API de REST del Marketo Engage o la exportación masiva, y están disponibles en filtros y déclencheur como restricciones adicionales para listas inteligentes.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integración** con Bizible LinkedIn Lead Gen Forms: Los especialistas en marketing ahora pueden realizar la atribución de ingresos en conversiones que se producen cuando LinkedIn captura los rellenos de formulario a través de sus unidades de anuncios de Forms de Generación de posibles clientes. Estas perspectivas se pueden utilizar para optimizar el rendimiento del formulario y las inversiones de medios de pago. linkedIn Lead Gen Forms es una de las ofertas de medios de pago de más rápido crecimiento de LinkedIn y esta nueva funcionalidad se incluye con nuestra integración de LinkedIn Ads con Bizible. 
 
* **Panel de Velocity** mejorado: Hemos agregado una nueva métrica de velocidad y un filtro de panel para obtener perspectivas más profundas. Los especialistas en marketing utilizan este tablero para comprender la velocidad de posible cliente y la velocidad de oportunidad paso a paso, así como la eficacia de diferentes formas de participación de ventas y marketing.

* **Nuevo tablero de Recorrido de cascada de cohorte**: Esto permitirá a los especialistas en marketing ver la progresión de una cohorte seleccionada a través de un conjunto clásico de etapas de &quot;cascada de demanda&quot;, lo que proporciona una comprensión rápida de las tasas de conversión y la causalidad implícita de la conversión de fase paso a paso.

## Integración de Bizible con Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Esta sección incluye nuevas funciones para los usuarios de Bizible que han completado su migración al sistema Identity Management de Adobe (IMS). Si se ha migrado, verá el nuevo Adobe ID en Configuración bisible en la pestaña Adobe ID . Todas las cuentas deberían migrarse a finales de 2021.

* **Integración de Bizible con el Privacy Service**  de Adobe (disponible en septiembre de 2021): La integración de Bizible con el Privacy Service de Adobe unifica el cumplimiento de las normas críticas de privacidad de datos (como el RGPD) en todas las aplicaciones de Adobe Experience Cloud. Ahora puede aprovechar este servicio y administrar todas las solicitudes de privacidad de forma centralizada, de modo que las solicitudes de cambio que llegan a Bizible y a otros productos de Adobe se reflejen en todas las aplicaciones.

* **Bizible en el shell** unificado de Adobe: La adopción por parte de Bizible de Adobe Unified Shell ofrece a los usuarios nuevas funciones que aparecerán en la barra de encabezado de la aplicación Bizible e incluyen un mejor acceso a los recursos de soporte y al cambio de aplicación. Adobe Unified Shell ayuda a crear una experiencia coherente entre Bizible y otras aplicaciones de Adobe Experience Cloud.

* **Propiedad y administración** autónomas de dominio bisible: Los usuarios de Bizible pueden aprovechar Adobe Admin Console para administrar los dominios que desean que Bizible rastree. Esto lleva el autoservicio a un proceso anteriormente manual y proporciona una experiencia coherente en la administración de la propiedad y el seguimiento del dominio en todas las aplicaciones de Adobe Experience Cloud.

## Anuncios {#announcements}

* **Actualizar a la configuración** de ID universal de suscripción: Para admitir la próxima integración de ID de Marketo Engage y Adobe para usuarios existentes, todas las suscripciones de Marketo Engage se unificarán para habilitar la compatibilidad con ID universales.
