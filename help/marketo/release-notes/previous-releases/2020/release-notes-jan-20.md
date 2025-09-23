---
unique-page-id: 37355534
description: 'Notas de la versión, enero de 2020: Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 1%

---

# Notas de la versión: enero de 2020 {#release-notes-jan}

Las siguientes funciones se incluyen en la versión de enero de 2020. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características se lanzarán el **17 de enero de 2020**.

## Aplicación principal de Marketo Engage Adobe {#core-marketo-engage-adobe-application}

* [Selector de recursos de Adobe Experience Manager](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): Acceda rápidamente a los recursos que se alinean con su marca con los recursos de AEM disponibles directamente en Marketo Engage. Nota: Aunque esta función está disponible tanto en nuestras experiencias Marketo Sky como en las clásicas, las funcionalidades administrativas se encuentran en nuestra experiencia clásica. Debe ser cliente de AEM Assets y tener la versión 6.5 o superior de.

>[!NOTE]
>
>Actualmente, el Selector de recursos de AEM solo es totalmente compatible con Firefox. Safari no lo admite y es posible que no funcione en la última versión de Chrome (v. 80), según la configuración de la cookie de SameSite.

* **[!DNL Microsoft Dynamics]- Sincronizar posible cliente con CRM en tiempo real**: Sincronización en tiempo real de posibles clientes y contactos entre Marketo Engage y [!DNL Microsoft Dynamics]. Cree posibles clientes o contactos y véalos en [!DNL Microsoft Dynamics] inmediatamente con la acción de flujo &quot;Sincronizar persona con Microsoft&quot;.
* Asignación de campos adicionales de Forms de generación de clientes potenciales **[!DNL LinkedIn]**: capture datos de clientes potenciales de Forms de generación de clientes potenciales [!DNL LinkedIn] para crear experiencias más relevantes tanto para los puntos de contacto de ventas como de marketing. Extraiga los campos ocultos, los campos de consentimiento y el campo de posibles clientes de prueba en Marketo Engage.
* **API de dependencias de plantilla de correo electrónico**: obtenga una lista de los recursos que dependen de una plantilla de correo electrónico para comprender el alcance de los posibles cambios y las dependencias de direcciones para las plantillas se pueden modificar y eliminar más rápido.
* **Mejoras en la administración de varias instancias**: vaya a la instancia que necesite rápidamente con un menú desplegable alfabético y desplazable de sus suscripciones.

## Account-Based Marketing {#account-based-marketing}

![(estrella)](assets/yellow-star.png)

* [Nueva detección de cuentas (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(estrella)](assets/yellow-star.png): Use la generación de perfiles de cuenta para descubrir nuevas cuentas de destino para su estrategia ABM en función de su modelo de perfil de cliente ideal con tecnología de IA. Ver, seleccionar e importar nuevas cuentas recomendadas, junto con sus indicadores de datos de ajuste e intención basados en IA, que aún no existen dentro de la base de datos de posibles clientes y cuentas de Marketo Engage para la segmentación por ABM. Disponible inmediatamente para clientes cualificados de generación de perfiles de cuenta.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## [!DNL Bizible] {#bizible}

![(estrella)](assets/yellow-star.png)

* **Integración de posibles clientes de Marketo Engage**: combine ventas y marketing con una vista unificada de los posibles clientes de [!DNL Bizible] y Marketo Engage. Con esta actualización, Marketo Engage ahora se puede utilizar como fuente de datos de posibles clientes adicional, por lo que ya no tiene que esperar a que los posibles clientes se sincronicen con CRM para informar sobre la generación de posibles clientes.
* **Mejoras de Discover**: Obtenga más información de nuestros paneles de Discover en [!DNL Bizible] con mejoras desarrolladas a partir de los comentarios de los clientes, como la capacidad de explorar en profundidad los registros transaccionales desde mosaicos y atributos, agregar recuentos de registros esenciales y las métricas de costo por valor correspondientes, y agregar o quitar filtros de panel para varios paneles. También se le redirigirá directamente al panel predeterminado tras iniciar sesión.

## [!DNL Marketo Sky] {#marketo-sky}

* [Edición de imágenes](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=es#design-studio): accede a las funciones de edición de Adobe sin tener que salir de Marketo Engage. Esta nueva funcionalidad le permite mejorar, recortar y agregar texto a las imágenes directamente en [!UICONTROL Design Studio].

## [!DNL Sales Insight] {#sales-insight}

* **[!DNL Salesforce Lightning]acciones por lotes**: mejora la eficacia de las ventas y permite que los compradores se involucren con la capacidad de añadir hasta 200 contactos/posibles clientes a las campañas y enviarles correos electrónicos de Marketo Engage por lotes con [!DNL Salesforce Lightning].
* **Compatibilidad móvil con[!DNL Salesforce1]**: Ahora dispone de acceso móvil directo a todas las características de [!DNL Sales Insight], como Momentos interesantes y Actividades web y Correos electrónicos, en la aplicación [!DNL Salesforce1].
* **Mejoras en la interfaz de usuario**: Interfaz actualizada con mejoras en la legibilidad y un diseño coherente con nuestra experiencia [!DNL Marketo Sky].

## [!DNL Sales Connect] {#sales-connect}

* **Componentes de cuadrícula**: optimice la instancia de [!DNL Sales Connect] con nuevas funcionalidades de personalización de cuadrícula. Elija qué columnas mostrar, busque columnas, seleccione o anule la selección de todas las columnas y determine cuántas filas de datos desea ver en cada página.
* **[Bloqueo de contenido](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: Maximice la alineación de marca con una configuración de toda la suscripción que controla si los usuarios que no son administradores tienen la capacidad de crear y editar plantillas y campañas.

>[!NOTE]
>
>* **Desuso de TLS 1.0 y 1.1**: En un esfuerzo continuo por integrarse con la estructura de versiones de Adobe, estamos cambiando el desuso de TLS 1.0 y TLS 1.1 al 13 de enero de 2020. Encontrará información más detallada [aquí](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Actualización de ITP 2.1+ [!DNL Munchkin]**: Debido a los cambios en la directiva de cookies de [!DNL Safari], ITP limitará la capacidad de [!DNL Munchkin] para rastrear a los usuarios entre sesiones en el mismo dominio a 1 o 7 días según la versión del explorador y el explorador que utilice el visitante. Para tener en cuenta esto, estamos implementando un nuevo servicio web para permitir que las cookies de Munchkin se configuren con un encabezado Set-Cookie a través de una respuesta HTTP. Encontrará más información sobre cómo implementar este nuevo servicio [aquí](https://nation.marketo.com/docs/DOC-7351).

**_Seminario web sobre la versión del producto_** [Únase a nosotros](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) el 3 de marzo a las 11:00AM PT / 2:00PM ET para asistir a un seminario web en directo organizado por nuestro equipo de productos y obtener más información sobre las funciones incluidas en esta versión.
