---
unique-page-id: 37355826
description: 'Notas De La Versión, Febrero De 2020: Documentos De Marketo: Documentación Del Producto'
title: Notas de la versión, febrero de 2020
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Notas de la versión: 20 de febrero {#release-notes-feb}

En la versión de febrero de 2020 se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella ( ![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes funciones se lanzaron el **21 de febrero de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **Acción de flujo &quot;Cambiar propietario en Microsoft&quot; de Microsoft Dynamics**: mantenga el control de los datos de CRM de Microsoft Dynamics con la capacidad de cambiar un propietario de posible cliente/contacto directamente desde el Marketo Engage. Esto supone una mejora de nuestra capacidad nativa de integración de CRM.
* **API de administración de usuarios**: automatice la administración de usuarios y funciones a través de sistemas de administración de identidades y organizaciones externos. Esto supone una mejora de nuestra capacidad de llamadas de API.
* **API de esquema de objeto personalizado**: administre y aprovisione automáticamente esquemas de objetos personalizados en todas las instancias de Marketo Engage para mantener la coherencia de los modelos de datos en las herramientas de ventas y marketing. Con esta API, puede definir y probar objetos personalizados en una zona protegida o centro de excelencia y aprovisionarlos en tantas instancias como sea necesario. Esto supone una mejora de la capacidad de llamadas de API. Póngase en contacto con el representante del Marketo Engage para obtener información sobre cómo obtener acceso a esta mejora.
* **API de reglas de redireccionamiento de página de aterrizaje**: Automatice la administración de las reglas de redireccionamiento de páginas de aterrizaje. Esto supone una mejora de nuestra capacidad de llamadas de API.
* **Caché del descriptor de formulario**: estamos reduciendo el tiempo de carga de los formularios incrustados y mejorando la estabilidad general de la aplicación almacenando en caché los formularios como recursos. Tenga en cuenta que las aprobaciones realizadas en los formularios incrustados pueden tardar hasta cuatro minutos en reflejarse en la web. Esto supone una mejora de nuestra capacidad de páginas de destino y Forms.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/yellow-star.png)

* **Segmentación basada en cuentas**: Analice la atribución a nivel de cuenta con la capacidad de crear segmentos y filtros para paneles de Discover en función de atributos de cuenta. Utilice estos segmentos para explorar en profundidad el rendimiento de marketing basado en cuentas.
* **Almacenamiento de filtros**: guarde filtros específicos de tableros exclusivos para cada usuario para analizar los tableros de forma rápida y coherente.
* **Exportar a PDF**: comparta perspectivas valiosas en toda la organización exportando Bizible Dashboards como PDF.

## Conexión de ventas {#sales-connect}

* **Actualizaciones de la ventana de composición**: Hemos optimizado el proceso de selección de plantillas y envío de correos electrónicos a través de Sales Connect. Utilice la ventana de redacción de nuestro cliente web y Salesforce como punto de venta único para vendedores, con la capacidad de guardar categorías de plantillas, programar correos electrónicos, enviar correos electrónicos por lotes y enviar correos electrónicos con seguimiento de visualizaciones y clics.
* **Actualizaciones del centro de comandos**: Estamos reconstruyendo el Centro de actuación de Sales Connect para que los vendedores comprendan todos sus correos electrónicos, llamadas y tareas que se han iniciado desde Sales Connect. También pueden ver información como la participación en el correo electrónico y la capacidad de envío, todo desde el Centro de comandos.

<br> 

## Anuncios {#announcements}

* **Centro de éxito de Marketo Engage**: vamos a lanzar el Centro de éxito de Marketo en febrero de 2020. El Centro de éxito es un centro de ayuda integrado en el producto que le permite buscar en la Documentación del producto, la Comunidad, las guías de inicio prácticas, el acceso al contenido de adopción, como la Universidad de Marketo y los vídeos de prácticas recomendadas de los compañeros, etc., directamente desde la instancia de Marketo Engage. **Nota**: Esta función se lanzará como una versión beta en ANZ y se comercializará en Norteamérica más adelante en el trimestre.

## Degradaciones {#deprecations}

* **Parámetro de API de recursos &quot;_method&quot;**: A partir de septiembre de 2020, los puntos de conexión de Asset API ya no aceptarán &quot;_method&quot; para pasar parámetros de consulta en un cuerpo de POST para omitir las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requerían este parámetro, el límite de URI para las API de recursos aumentará de 6 KiB a 65 KiB, de modo que se puedan enviar URI de solicitud largos.
* **Degradación de compatibilidad con Internet Explorer**: A partir de nuestra versión del 31 de julio de 2020, la interfaz de usuario de Marketo Engage dejará de ser compatible con Internet Explorer.

**_Seminario web sobre lanzamiento de productos_** [Únase a nosotros](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) el 3 de marzo a las 11:00 (PT)/14:00 (ET) para asistir a un seminario web en directo organizado por nuestro equipo de productos y obtener más información sobre las funciones incluidas en esta versión.
