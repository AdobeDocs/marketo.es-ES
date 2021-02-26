---
unique-page-id: 45416698
description: Notas de la versión - Julio del 2014 - Documentos de marketing - Documentación del producto
title: Notas de la versión - Julio del 20
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---


# Notas de la versión: 20 de julio {#release-notes-july}

Las siguientes funciones se incluyen en la versión del 20 de julio. Compruebe la disponibilidad de las funciones en la edición de marketing.

>[!AVAILABILITY]
>
>Tenga en cuenta que, según el paquete actual, los elementos con una estrella ( ![(star)](assets/star-yellow.svg)) pueden requerir la compra de un complemento de valor. Comuníquese con el representante de su Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes funciones se lanzarán el 31  **de julio de 2020**.

## Administración {#administration}

* **[Exportación &quot;Utilizada por&quot; en Administración](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** de Campo: Los administradores ahora pueden exportar todos los vínculos de recursos &quot;Utilizados por&quot; de un campo seleccionado a un archivo CSV. Esta mejora puede ayudar tanto a los administradores como a los no administradores a limpiar los campos no utilizados. Además, los recursos ahora se pueden abrir en una nueva ficha o ventana del explorador.

## Marketing basado en cuentas {#account-based-marketing}

![(estrella)](assets/star-yellow.svg)

* **Interfaz de usuario actualizada para la generación de perfiles** de cuenta: Simplifique la creación de su lista de cuenta de destinatario en la generación de perfiles de cuenta con pasos optimizados en una sola pantalla.

<br> 

**_Publicación durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se publicarán en los próximos meses.

* **Servicio** Forms: Estamos introduciendo una validación de la sintaxis de los campos de formulario más sólida y la capacidad de bloquear patrones de bots comunes con las nuevas funciones de Dominios seguros para Páginas de aterrizaje. Bloquear patrones de bots puede reducir el envío de formularios no deseados y mejorar la calidad de la base de datos.
* **Límite** de tamaño de URI de API de recurso aumentado: El límite de tamaño del identificador de recursos uniforme (URI) se está incrementando de 8 KB a 65 KB antes de eliminar el parámetro &quot;_method&quot;. Al realizar cadenas de consulta largas, este aumento del límite de tamaño permitirá que los datos se transmitan con mayor facilidad. La eliminación del parámetro &quot;_method&quot; forma parte de una próxima actualización de seguridad.

## Perspectiva de ventas {#sales-insight}

![(estrella)](assets/star-yellow.svg)

* **[Perspectiva de ventas habilitada para clientes con integración](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  de CRM de Salesforce no nativa (Beta)**: Los clientes Marketo Engage con integraciones CRM no nativas de Salesforce ahora pueden utilizar Sales Insight para ayudar a sus equipos de ventas a comprender, priorizar e interactuar con los posibles clientes y las oportunidades más comprometidos a fin de permitir la venta inteligente y acuerdos más rápidos.

## Sales Connect {#sales-connect}

![(estrella)](assets/star-yellow.svg)

* **[Consentimiento de dos partes mejorado para las llamadas de venta:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** los administradores ahora tienen bueno control sobre las configuraciones de registro de llamadas. [Habilite ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) las grabaciones de llamadas con la confianza de que cumple con la ley de consentimiento de dos partes. Automatice la notificación de la llamada que se está grabando y active los clips de audio para que se reproduzcan antes de la llamada.

<br> 

## Anuncios y desaprobaciones {#announcements-deprecations}

* **Eliminación** del parámetro &quot;_method&quot; de la API de recursos: Después de septiembre de 2020, los extremos de la API de recursos ya no aceptarán &quot;_method&quot; para pasar parámetros de Consulta en un cuerpo de POST para evitar las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requieren este parámetro, los límites de URI para las API de recursos se incrementarán de 8 KB a 65 KB.
* **[Líder](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** asociado de Munchkin: Con esta versión de Munchkin JavaScript Client, versión 159, empezaremos a dejar de utilizar el método Munchkin Associate Lead. Si se invoca, recibirá una advertencia que indica que el método se eliminará en una versión futura. Una vez eliminado, el método dejará de funcionar y los intentos de utilizarlo fallarán. A los clientes Marketo Engage que hayan utilizado este método recientemente se les notificará individualmente su uso.
* **Compatibilidad con Internet Explorer**: Como se ha anunciado anteriormente, la compatibilidad con Internet Explorer 11 finaliza el 31  **de julio de 2020**. Seguiremos admitiendo Google Chrome, Mozilla Firefox, Apple Safari y Microsoft Edge.
* **Experiencia** predeterminada de Sky: La opción para que los administradores o usuarios establezcan Marketo Sky como experiencia predeterminada se eliminará en esta versión como preparación para una actualización de la experiencia de usuario principal. En julio se dispondrá de más detalles sobre la actualización de la experiencia primaria, prevista para finales de este año. Los usuarios que hayan establecido Marketo Sky como su experiencia predeterminada, o a los que se les haya concedido acceso a Marketo Sky, pueden seguir accediendo a Marketo Sky desde un mosaico de la página de inicio Mi marketing.
* **Compatibilidad** con EdgeHTML (sin cromo) con Microsoft Edge: Marketo Engage ya no admitirá las versiones de EdgeHTML de Microsoft Edge a finales de 2020. A partir del 1 de enero de 2021, solo admitiremos la última versión de cromo de Microsoft Edge.
