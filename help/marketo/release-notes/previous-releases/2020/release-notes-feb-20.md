---
unique-page-id: 37355826
description: 'Notas De La Versión, Febrero De 2020: Documentos De Marketo: Documentación Del Producto'
title: Notas de la versión, febrero de 2020
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 2%

---

# Notas de la versión: febrero de 2020 {#release-notes-feb}

En la versión de febrero de 2020 se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes características se lanzaron el **21 de febrero de 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **[!DNL Microsoft Dynamics]&quot;Cambiar propietario en Microsoft&quot; Acción de flujo**: mantenga el control de los datos de CRM [!DNL Microsoft Dynamics] con la capacidad de cambiar un propietario de contacto o posible cliente directamente desde Marketo Engage. Esto supone una mejora de nuestra capacidad nativa de integración de CRM.
* **API de administración de usuarios**: Automatice la administración de usuarios y funciones a través de sistemas de administración de identidades y organizaciones externos. Esto supone una mejora de nuestra capacidad de llamadas de API.
* **API de esquema de objeto personalizado**: administre y aprovisione automáticamente esquemas de objeto personalizados en todas las instancias de Marketo Engage para mantener la coherencia de los modelos de datos en las herramientas de ventas y marketing. Con esta API, puede definir y probar objetos personalizados en una zona protegida o centro de excelencia y aprovisionarlos en tantas instancias como sea necesario. Esto supone una mejora de la capacidad de llamadas de API. Póngase en contacto con su representante de Marketo Engage para obtener información sobre cómo obtener acceso a esta mejora.
* **API de reglas de redirección de páginas de aterrizaje**: Automatice la administración de las reglas de redirección de páginas de aterrizaje. Esto supone una mejora de nuestra capacidad de llamadas de API.
* **Almacenamiento en caché del descriptor de formulario**: estamos reduciendo el tiempo de carga de los formularios incrustados y mejorando la estabilidad general de la aplicación al almacenar en caché los formularios como recursos. Tenga en cuenta que las aprobaciones realizadas en los formularios incrustados pueden tardar hasta cuatro minutos en reflejarse en la web. Esto supone una mejora de nuestra capacidad de páginas de destino y Forms.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## [!DNL Bizible] {#bizible}

![(estrella)](assets/yellow-star.png)

* **Segmentación basada en cuentas**: Analice la atribución en el nivel de cuenta con la capacidad de crear segmentos y filtros para los paneles de detección en función de los atributos de la cuenta. Utilice estos segmentos para explorar en profundidad el rendimiento de marketing basado en cuentas.
* **Filtros de almacenamiento**: guarde filtros específicos de tableros exclusivos de cada usuario para analizar los tableros de forma rápida y coherente.
* **Exportar a PDF**: Comparta información valiosa en toda la organización mediante la exportación de paneles de Bizible en formato PDF.

## [!DNL Sales Connect] {#sales-connect}

* **Actualizaciones de la ventana de composición**: hemos optimizado el proceso de selección de plantillas y envío de correos electrónicos a través de [!DNL Sales Connect]. Utilice la ventana de redacción de nuestro cliente web y Salesforce como punto de venta único para vendedores, con la capacidad de guardar categorías de plantillas, programar correos electrónicos, enviar correos electrónicos por lotes y enviar correos electrónicos con seguimiento de visualizaciones y clics.
* **Actualizaciones del centro de comandos**: Estamos reconstruyendo el centro de comandos [!DNL Sales Connect] para proporcionar a los vendedores insight en todos sus correos electrónicos, llamadas y tareas que se han iniciado desde [!DNL Sales Connect]. También pueden ver información como la participación en el correo electrónico y la capacidad de envío, todo desde el Centro de comandos.

<br> 

## Anuncios {#announcements}

* **Centro de éxito de Marketo Engage**: vamos a lanzar el Centro de éxito de Marketo en febrero de 2020. El Centro de éxito es un centro de ayuda integrado en el producto que le permite buscar en la Documentación del producto, la Comunidad, las guías de inicio prácticas, el acceso al contenido de adopción, como la Universidad de Marketo y los vídeos de prácticas recomendadas de los compañeros, etc., directamente desde su instancia de Marketo Engage. **Nota**: esta característica se lanzará como una versión beta en ANZ y se implementará en Norteamérica más adelante en el trimestre.

## En desuso {#deprecations}

* **Parámetro &quot;_method&quot; de Asset API**: a partir de septiembre de 2020, los puntos de conexión de Asset API ya no aceptarán &quot;_method&quot; para pasar parámetros de consulta en un cuerpo de POST para omitir las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requerían este parámetro, el límite de URI para las API de recursos aumentará de 6 KiB a 65 KiB, de modo que se puedan enviar URI de solicitud largos.
* **Degradación de compatibilidad con Internet Explorer**: a partir de nuestra versión del 31 de julio de 2020, la interfaz de usuario de Marketo Engage dejará de ser compatible con Internet Explorer.

**_Seminario web sobre la versión del producto_** [Únase a nosotros](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) el 3 de marzo a las 11:00AM PT / 2:00PM ET para asistir a un seminario web en directo organizado por nuestro equipo de productos y obtener más información sobre las funciones incluidas en esta versión.
