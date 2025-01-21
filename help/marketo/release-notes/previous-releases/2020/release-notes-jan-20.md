---
unique-page-id: 37355534
description: 'Notas de la versión, enero de 2020: Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 89995b2cd6fdc2f2e4ea43906304bdf16d367de1
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Notas de la versión: enero de 2020 {#release-notes-jan}

Las siguientes funciones se incluyen en la versión de enero de 2020. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características se lanzarán el **17 de enero de 2020**.

## Aplicación de Adobe de Marketo Engage principal {#core-marketo-engage-adobe-application}

* [Selector de recursos de Adobe Experience Manager AEM](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): Acceda rápidamente a los recursos que se alinean con su marca con los recursos que están disponibles directamente en Marketo Engage. Nota: Aunque esta función está disponible tanto en las experiencias Marketo Sky como en las clásicas, las funcionalidades administrativas se encuentran en nuestra experiencia clásica. Debe ser cliente de AEM Assets y tener la versión 6.5 o superior de.

>[!NOTE]
>
>AEM Actualmente, solo se admite el Selector de recursos de en Firefox. Safari no lo admite y es posible que no funcione en la última versión de Chrome (v. 80), según la configuración de la cookie de SameSite.

* **Microsoft Dynamics: sincronizar posible cliente con CRM en tiempo real**: sincronización en tiempo real de posibles clientes y contactos entre Marketo Engage y Microsoft Dynamics. Cree posibles clientes o contactos y véalos en Microsoft Dynamics inmediatamente con la acción de flujo &quot;Sincronizar persona con Microsoft&quot;.
* **Asignación de campos adicionales para Forms de generación de clientes potenciales de LinkedIn**: capture datos de clientes potenciales de Forms de generación de clientes potenciales de LinkedIn para crear experiencias más relevantes tanto para puntos de contacto de ventas como de marketing. Extraer campos ocultos, campos de consentimiento y el campo de posibles clientes de prueba al Marketo Engage.
* **API de dependencias de plantilla de correo electrónico**: obtenga una lista de los recursos que dependen de una plantilla de correo electrónico para comprender el alcance de los posibles cambios y las dependencias de direcciones para las plantillas se pueden modificar y eliminar más rápido.
* **Mejoras en la administración de varias instancias**: vaya a la instancia que necesite rápidamente con un menú desplegable alfabético y desplazable de sus suscripciones.

## Account-Based Marketing {#account-based-marketing}

![(estrella)](assets/yellow-star.png)

* [Nueva detección de cuentas (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(estrella)](assets/yellow-star.png): Use la generación de perfiles de cuenta para descubrir nuevas cuentas de destino para su estrategia ABM en función de su modelo de perfil de cliente ideal con tecnología de IA. Ver, seleccionar e importar nuevas cuentas recomendadas, junto con sus indicadores de datos de ajuste e intención basados en IA, que no existen ya en la base de datos de clientes potenciales y cuentas de Marketo Engage para la segmentación ABM. Disponible inmediatamente para clientes cualificados de generación de perfiles de cuenta.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/yellow-star.png)

* **Integración de posibles clientes de Marketo Engage**: combine ventas y marketing con una vista unificada de los posibles clientes de Bizible y Marketo Engage. Con esta actualización, Marketo Engage ahora se puede utilizar como fuente de datos de posibles clientes adicional, por lo que ya no tiene que esperar a que los posibles clientes se sincronicen con CRM para informar sobre la generación de posibles clientes.
* **Mejoras de Discover**: saque más partido de nuestros paneles de Discover en Bizible con las mejoras desarrolladas a partir de los comentarios de los clientes, como la capacidad de explorar en profundidad los registros transaccionales desde mosaicos y atributos, agregar recuentos de registros esenciales y las métricas de coste por unidad correspondientes, y agregar o quitar filtros de panel para varios paneles. También se le redirigirá directamente al panel predeterminado tras iniciar sesión.

## Marketo Sky {#marketo-sky}

* [Edición de imágenes](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio): accede a las capacidades de edición de un Adobe sin tener que salir del Marketo Engage. Esta nueva funcionalidad le permite realizar fácilmente tareas como mejorar, recortar y agregar texto a imágenes directamente en Design Studio.

## Sales Insight {#sales-insight}

* **Acciones masivas de Lightning de Salesforce**: mejora la eficacia de las ventas y permite que los compradores se involucren con la capacidad de agregar hasta 200 contactos/posibles clientes en campañas y enviarles correos electrónicos de Marketo Engage por lotes con Lightning de Salesforce.
* **Soporte móvil para Salesforce1**: Ahora dispone de acceso móvil directo a todas las funciones de Sales Insight, como Momentos interesantes y Actividades web y Correos electrónicos, directamente en la aplicación Salesforce1.
* **Mejoras en la interfaz de usuario**: Interfaz actualizada con mejoras en la legibilidad y un diseño coherente con nuestra experiencia de Marketo Sky.

## Conexión de ventas {#sales-connect}

* **Componentes de cuadrícula**: optimice su instancia de Sales Connect con nuevas funcionalidades de personalización de cuadrícula. Elija qué columnas mostrar, busque columnas, seleccione o anule la selección de todas las columnas y determine cuántas filas de datos desea ver en cada página.
* **[Bloqueo de contenido](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: Maximice la alineación de marca con una configuración de toda la suscripción que controla si los usuarios que no son administradores tienen la capacidad de crear y editar plantillas y campañas.

>[!NOTE]
>
>* **Desuso de TLS 1.0 y 1.1**: En un esfuerzo continuo por integrarse con la estructura de versiones de Adobe, estamos cambiando el desuso de TLS 1.0 y TLS 1.1 al 13 de enero de 2020. Encontrará información más detallada [aquí](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ Munchkin Update**: Debido a los cambios en la directiva de cookies de Safari, ITP limitará la capacidad de Munchkin para rastrear usuarios entre sesiones en el mismo dominio a 1 o 7 días según la versión del explorador y el visitante que utilice. Para tener en cuenta esto, estamos implementando un nuevo servicio web para permitir que las cookies de Munchkin se configuren con un encabezado Set-Cookie a través de una respuesta HTTP. Encontrará más información sobre cómo implementar este nuevo servicio [aquí](https://nation.marketo.com/docs/DOC-7351).

**_Seminario web sobre la versión del producto_** [Únase a nosotros](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) el 3 de marzo a las 11:00 a.m. PT / 2:00 p.m. ET para asistir a un seminario web en directo organizado por nuestro equipo de productos y obtener más información sobre las funciones incluidas en esta versión.
