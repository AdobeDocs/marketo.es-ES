---
unique-page-id: 45416698
description: Notas de la versión - Julio del 2020 - Marketo Docs - Documentación del producto
title: Notas de la versión, julio de 2020
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---


# Notas de la versión: Julio del 20 {#release-notes-july}

La versión del 20 de julio incluye las siguientes funciones. Consulte la edición de Marketo para ver la disponibilidad de las funcionalidades.

>[!AVAILABILITY]
>
>Tenga en cuenta que, según el paquete actual, los elementos con una estrella ( ![(star)](assets/star-yellow.svg)) pueden requerir la compra de un complemento de valor. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestralesLas siguientes_** funciones se lanzarán el 31 de  **julio de 2020**.

## Administración {#administration}

* **[Exportación &quot;Utilizado por&quot; en Field Management](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Los administradores ahora pueden exportar todos los vínculos de recursos &quot;Utilizados por&quot; para un campo seleccionado a un archivo CSV. Esta mejora puede ayudar tanto a los administradores como a los no administradores a limpiar los campos no utilizados. Además, los recursos ahora se pueden abrir en una nueva pestaña o ventana del explorador.

## Marketing basado en cuentas {#account-based-marketing}

![(estrella)](assets/star-yellow.svg)

* **Interfaz de usuario actualizada para la creación de perfiles de cuenta**: Simplifique la creación de la lista de cuentas objetivo en Perfiles de cuenta con pasos optimizados en una sola pantalla.

<br> 

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

* **Servicio** de Forms: Se está introduciendo una validación más sólida de la sintaxis de los campos de formulario y la capacidad de bloquear patrones de bots comunes con las nuevas funciones de Dominios seguros para páginas de aterrizaje. Bloquear los patrones de bots puede reducir los envíos de formularios no deseados y mejorar la calidad de la base de datos.

>[!NOTE]
>
>El despliegue completo de la validación mejorada de la sintaxis de los campos del formulario se ha pospuesto hasta después de nuestra versión de enero de 2021.

* **Límite** de tamaño de URI de API de recurso aumentado: El límite de tamaño del identificador uniforme de recursos (URI) se está aumentando de 8 KB a 65 KB antes de eliminar el parámetro &quot;_method&quot;. Al realizar cadenas de consulta largas, este aumento del límite de tamaño permitirá que los datos pasen más fácilmente. La eliminación del parámetro &quot;_method&quot; forma parte de una próxima actualización de seguridad.

## Perspectiva de ventas {#sales-insight}

![(estrella)](assets/star-yellow.svg)

* **[Perspectiva de ventas habilitada para clientes con integración](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  de Salesforce CRM no nativa (Beta)**: Los clientes Marketo Engage con integraciones de Salesforce CRM no nativas ahora pueden utilizar Sales Insight para ayudar a sus equipos de ventas a comprender, priorizar e interactuar con los posibles clientes y oportunidades más comprometidos a fin de permitir ventas inteligentes y ofertas más rápidas.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/star-yellow.svg)

* **[Consentimiento de dos partes mejorado para las llamadas de venta:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** ahora los administradores tienen bueno control sobre las configuraciones de registro de llamadas. [Habilite las ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) grabaciones de llamadas con confianza en que cumple con la ley de consentimiento de dos partes. Automatice la notificación de la llamada que se está grabando y active los clips de audio que se reproduzcan antes de la llamada.

<br> 

## Anuncios y casos de finalización del soporte {#announcements-deprecations}

* **Eliminación del parámetro &quot;_method&quot; de la API de recursos**: A partir de septiembre de 2020, los extremos de la API de Asset ya no aceptarán &quot;_method&quot; para pasar parámetros de consulta en un cuerpo de POST para evitar las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requerían este parámetro, los límites de URI de las API de Asset aumentarán de 8 KB a 65 KB.
* **[Asociado de Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Con esta versión de Munchkin JavaScript Client, versión 159, comenzaremos a dejar de utilizar el método Munchkin Associate Lead. Si se invoca, recibirá una advertencia que indica que el método se eliminará en una versión futura. Una vez eliminado, el método ya no funcionará y los intentos de utilizarlo fallarán. A los clientes Marketo Engage que hayan utilizado este método recientemente se les notificará de su uso de forma individual.
* **Compatibilidad con Internet Explorer**: Como se anunció anteriormente, el soporte Marketo Engage para Internet Explorer 11 finaliza el 31 de  **julio de 2020**. Seguiremos siendo compatibles con Google Chrome, Mozilla Firefox, Apple Safari y Microsoft Edge.
* **Experiencia** predeterminada de Sky: La opción para que los administradores o usuarios establezcan el Marketo Sky como la experiencia predeterminada se eliminará en esta versión a fin de prepararla para una actualización de la experiencia del usuario principal. En julio estarán disponibles más detalles sobre la actualización de la experiencia principal, prevista para finales de este año. Los usuarios que hayan establecido Marketo Sky como su experiencia predeterminada o a los que se les haya concedido acceso a Marketo Sky, pueden seguir accediendo a Marketo Sky desde un mosaico en la página de inicio de Mi Marketo.
* **Compatibilidad con** EdgeHTML (que no sea Chromium) de Microsoft Edge: Marketo Engage dejará de ser compatible con las versiones EdgeHTML de Microsoft Edge a finales de 2020. A partir del 1 de enero de 2021, solo admitiremos la última versión de Chromium de Microsoft Edge.
