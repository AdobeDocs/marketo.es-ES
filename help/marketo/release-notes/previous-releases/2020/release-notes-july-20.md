---
unique-page-id: 45416698
description: 'Notas de la versión, julio de 2020: Documentos de Marketo: documentación del producto'
title: Notas de la versión, julio de 2020
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
TQID: https://experienceleague.adobe.com/m0gaKwTahjs5M2I7i-XVYMLZT4COy0XRTYwIsd3p9g8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
subfeature_v2: id: f5e85a9b-a883-40d0-8759-f3651efb32e9
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 651
ht-degree: 2%

---

# Notas de la versión: julio de 2020 {#release-notes-july}

Las siguientes funciones se incluyen en la versión de julio de 2020. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Tenga en cuenta que, según el paquete actual, los elementos con un asterisco (![(estrella)](assets/yellow-star.png)) pueden requerir la compra de un complemento de valor. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes características se lanzarán el **31 de julio de 2020**.

## Administración {#administration}

* Exportación de **[&quot;Utilizado por&quot; en Administración de campos](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: los administradores ahora pueden exportar todos los vínculos de recursos &quot;Utilizado por&quot; de un campo seleccionado a un archivo CSV. Esta mejora puede ayudar a los administradores y a los no administradores a limpiar los campos no utilizados. Además, los recursos ahora se pueden abrir en una nueva pestaña o ventana del explorador.

## Account-Based Marketing {#account-based-marketing}

![(estrella)](assets/yellow-star.png)

* **Interfaz de usuario actualizada para el perfil de cuenta**: Simplifique la creación de la lista de cuentas de destino en el perfil de cuenta con pasos optimizados, todo en una sola pantalla.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

* **Servicio de Forms**: se está implementando una validación más sólida de la sintaxis de los campos de formulario y la capacidad de bloquear patrones de bots comunes con nuevas funciones de dominios seguros para páginas de aterrizaje. Bloquear patrones de bots puede reducir los envíos de formularios de correo no deseado y mejorar la calidad de la base de datos.

>[!NOTE]
>
>La implementación completa de la validación de la sintaxis de los campos de formulario mejorados se ha pospuesto hasta después de nuestra versión de enero de 2021.

* **Límite de tamaño de URI de Asset API aumentado**: El límite de tamaño de identificador uniforme de recursos (URI) se está aumentando de 8 KB a 65 KB antes de que se elimine el parámetro &quot;_method&quot;. Al realizar cadenas de consulta largas, este aumento del límite de tamaño permite que los datos pasen más fácilmente. La eliminación del parámetro &quot;_method&quot; forma parte de una próxima actualización de seguridad.

## [!DNL Sales Insight] {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Habilitado para clientes con integración no nativa [!DNL Salesforce] CRM](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: Los clientes de Marketo Engage con integraciones no nativas de CRM [!DNL Salesforce] ahora pueden usar [!DNL Sales Insight] para ayudar a sus equipos de ventas a comprender, priorizar e interactuar con los posibles clientes más comprometidos y las oportunidades para permitir ventas inteligentes y ofertas más rápidas.

## [!DNL Sales Connect] {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **[Consentimiento mejorado de dos partes para llamadas de ventas:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Los administradores ahora tienen un mayor control sobre las configuraciones de grabación de llamadas. [Habilite las grabaciones de llamadas](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) con la seguridad de que cumple con la ley de consentimiento de dos partes. Automatice la notificación de la llamada que se está grabando y active los clips de audio que se van a reproducir antes de la llamada.

<br> 

## Anuncios y desaprobaciones {#announcements-deprecations}

* **Eliminación del parámetro &quot;_method&quot; de la API de Asset**: a partir de septiembre de 2020, los puntos de conexión de Asset API ya no aceptarán &quot;_method&quot; para pasar parámetros de consulta en un cuerpo de POST para omitir las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requerían este parámetro, los límites de URI para las API de recursos se aumentarán de 8 KB a 65 KB.
* **[[!DNL Munchkin] Asociar posible cliente](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Con esta versión de Munchkin JavaScript Client, versión 159, comenzaremos la desaprobación del método de asociado de posible cliente [!DNL Munchkin]. Si se invoca, recibirá una advertencia que indica que el método se eliminará en una versión futura. Una vez eliminado, el método deja de funcionar y los intentos de utilizarlo dan error. A los clientes de Marketo Engage que hayan utilizado este método recientemente se les notificará individualmente su uso.
* **Compatibilidad con Internet Explorer**: Como se anunció anteriormente, la compatibilidad con Marketo Engage para Internet Explorer 11 finaliza el **31 de julio de 2020**. Seguiremos admitiendo [!DNL Google Chrome], [!DNL Mozilla Firefox], [!DNL  Apple Safari] y [!DNL Microsoft Edge].
* **Experiencia predeterminada en Sky**: La opción para que los administradores o usuarios establezcan [!DNL Marketo Sky] como la experiencia predeterminada se eliminará en esta versión como preparación para una actualización de la experiencia del usuario principal. En julio estarán disponibles más detalles sobre la actualización de la experiencia principal, programada para finales de este año. Los usuarios que hayan establecido [!DNL Marketo Sky] como su experiencia predeterminada o a los que se les haya concedido acceso a [!DNL Marketo Sky], pueden seguir teniendo acceso a [!DNL Marketo Sky] desde un mosaico en la página principal de Mi Marketo.
* **Compatibilidad con EdgeHTML (que no es Chromium) [!DNL Microsoft Edge]**: Marketo Engage dejará de ser compatible con las versiones EdgeHTML de Microsoft Edge a finales de 2020. A partir del 1 de enero de 2021, solo admitiremos la última versión de Chromium de Microsoft Edge.
