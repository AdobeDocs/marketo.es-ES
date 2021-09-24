---
unique-page-id: 37355826
description: Notas de la versión - Feb 20 - Marketo Docs - Documentación del producto
title: Notas de la versión, febrero de 2020
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Notas de la versión: Febrero de 2020 {#release-notes-feb}

La versión del 20 de febrero incluye las siguientes funciones. Compruebe la disponibilidad de las funciones en su edición de Marketo.

>[!AVAILABILITY]
>
>Las funciones denotadas por una estrella ( ![(star)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestralesLas siguientes_** funciones se lanzaron el 21 de  **febrero de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **Acción** de flujo &quot;Cambiar propietario en Microsoft&quot; de Microsoft Dynamics: Mantenga el control de sus datos de Microsoft Dynamics CRM con la capacidad de cambiar un posible cliente/contacto directamente desde el Marketo Engage. Esta es una mejora de nuestra capacidad de integración nativa de CRM.
* **API de administración de usuarios**: Automatice la administración de usuarios y funciones a través de sistemas de administración de organizaciones e identidades externas. Esta es una mejora de nuestra capacidad de llamadas API.
* **API** de esquema de objetos personalizados: Administre y proporcione automáticamente esquemas de objetos personalizados entre instancias en Marketo Engage para mantener la coherencia de los modelos de datos en las herramientas de marketing y ventas. Con esta API, puede definir y probar objetos personalizados en un entorno limitado o centro de excelencia y aprovisionarlos en tantas instancias como sea necesario. Esta es una mejora de nuestra capacidad de llamadas a API. Póngase en contacto con el representante del Marketo Engage para obtener información sobre cómo obtener acceso a esta mejora.
* **API de reglas de redireccionamiento de páginas de aterrizaje**: Automatice la administración de las reglas de redireccionamiento de páginas de aterrizaje. Esta es una mejora de nuestra capacidad de llamadas API.
* **Almacenamiento en caché del descriptor de formulario**: Estamos reduciendo el tiempo de carga de los formularios incrustados y mejorando la estabilidad general de la aplicación al almacenar en caché los formularios como recursos. Tenga en cuenta que las aprobaciones realizadas en formularios incrustados pueden tardar hasta cuatro minutos en reflejarse en la web. Esta es una mejora de nuestra capacidad de Páginas de aterrizaje y Forms.

<br> 

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/yellow-star.png)

* **Segmentación basada en cuentas**: Analice la atribución a nivel de cuenta con la capacidad de crear segmentos y filtros para tableros de Discover según los atributos de la cuenta. Utilice estos segmentos para explorar en profundidad el rendimiento de marketing basado en cuentas.
* **Guardar filtros**: Guarde filtros específicos del tablero exclusivos para cada usuario a fin de analizar los tableros de forma rápida y coherente.
* **Exportar a PDF**: Comparta perspectivas valiosas en su organización exportando tableros Bizible como PDF.

## Conexión de ventas {#sales-connect}

* **Actualizaciones** de la ventana de composición: Hemos optimizado el proceso para seleccionar plantillas y enviar correos electrónicos a través de Conexión de ventas. Utilice la ventana Componer de nuestro cliente web y Salesforce como ventanilla única para vendedores, con la capacidad de guardar categorías de plantillas, programar correos electrónicos, enviar correos electrónicos de forma masiva y enviar correos electrónicos con vista y rastreo de clics.
* **Actualizaciones** del centro de comandos: Estamos reconstruyendo el Centro de comandos de Conexión de Ventas para ofrecer a los vendedores información sobre todos sus correos electrónicos, llamadas y tareas iniciadas desde Conexión de Ventas. También pueden ver información como la participación por correo electrónico y la capacidad de envío desde el Centro de comandos.

<br> 

## Anuncios {#announcements}

* **Centro de éxito del Marketo Engage**: Lanzaremos el Centro de éxito de Marketo en febrero de 2020. El Centro de éxito es un centro de ayuda integrado en el producto que le permite buscar en la Documentación del producto y la Comunidad, iniciar guías de procedimientos, acceder a contenido de adopción como vídeos de prácticas recomendadas de la Universidad de Marketo y otros, directamente desde la instancia de Marketo Engage. **Nota**: Esta función se lanzará como una versión beta en ANZ y se lanzará a Norteamérica más adelante en el trimestre.

## Degradaciones {#deprecations}

* **Parámetro** &quot;_method&quot; de la API de recursos: A partir de septiembre de 2020, los puntos de conexión de Asset API ya no aceptarán &quot;_method&quot; para pasar parámetros de consulta en un cuerpo de POST para evitar las limitaciones de longitud de URI. Para dar cabida a las solicitudes que requerían este parámetro, el límite de URI para las API de Asset aumentará de 6 KiB a 65 KiB, de modo que se puedan enviar URI de solicitud largas.
* **Desaprobación de la compatibilidad con Internet Explorer**: A partir de nuestra versión del 31 de julio de 2020, la interfaz de usuario de Marketo Engage dejará de ser compatible con Internet Explorer.

**_Seminario_** [web sobre la versión del productoÚnase ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) al sitio el 3 de marzo a las 11:00 a.m. PT/2:00 p.m. ET para ver un seminario web en directo alojado por nuestro equipo de productos y obtenga más información sobre las funciones incluidas en esta versión.
