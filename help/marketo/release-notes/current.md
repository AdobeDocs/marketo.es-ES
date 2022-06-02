---
description: Notas de la versión actuales - Documentos de Marketo - Documentación del producto
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 40e88a573079b87b3af9a653d8e0b64b5b7522bc
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Notas de la versión: Junio de 2022 {#release-notes-june-22}

A continuación encontrará todas las funciones incluidas en la versión del 22 de junio. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

Las siguientes funciones empezarán a lanzarse en **24 de junio de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exponer campos de CreatedAt/UpdatedAt para objetos personalizados**: Permite inspeccionar estos campos en la pantalla Detalle de persona para obtener información adicional.

## Organización en canales múltiples {#cross-channel-orchestration}

* **Se ha mejorado la facilidad de uso del Diseñador de flujos para la conversación dinámica**: Añada tarjetas directamente desde el lienzo del Diseñador de secuencias sin necesidad de arrastrar y soltar. La interfaz de chat dinámico también se ha mejorado para ofrecer una mejor visibilidad del contenido en tarjetas individuales.

* **Reglas de enrutamiento de citas avanzadas para chat dinámico**: Dynamic Chat ofrece más opciones para el enrutamiento de citas con objetivo. Especifique las citas del agente que deben enrutarse en función de los atributos del Marketo Engage, asegurándose de que los posibles clientes se dirijan a los agentes adecuados.

* **Informes de diálogos avanzados para la conversación dinámica**: Vea en bueno detalle el rendimiento de sus campañas de chat dinámico mediante las visualizaciones de datos nuevas para métricas de participación y conversión.

* **Desincronizar atributos de Marketo Engage no utilizados para Dynamic Chat**: Desincronice los atributos de Marketo Engage de su suscripción de Dynamic Chat que no se utilicen, lo que le ayudará a facilitar la limpieza de los datos y le permitirá sincronizar atributos alternativos según sea necesario.

## Automatización de la experiencia {#experience-automation}

* **Exclusiones de reglas de validación de campos de formulario globales**: Excluya formularios específicos de las reglas de validación del formulario global, de modo que los centros de suscripción y otros flujos de trabajo críticos para la empresa puedan aceptar todos los valores.

* **Pasos de flujo de autoservicio**: Amplíe la conectividad entre el Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para utilizarlos en campañas inteligentes. Tanto los usuarios como los socios Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de Déclencheur, por lotes y ejecutables, a diferencia de los Webhooks, que solo se pueden usar en campañas de Déclencheur.

* **Protocolo Munchkin Seguimiento de vínculos agnósticos**: Ampliación de la compatibilidad con el seguimiento de `tel` y `mailto` vínculos con Munchkin para realizar un seguimiento de un conjunto ampliado de comportamientos web.

* **Métodos HTTP adicionales para los enlaces web**: Especifique PUT, PATCH y DELETE como tipos de solicitud para interactuar con los servicios web.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Conjunto de permisos de Insight de ventas en Salesforce**: Los administradores pueden proporcionar acceso a la perspectiva de ventas a un conjunto limitado de personas a nivel de usuario en lugar de a nivel de perfil a través del conjunto de permisos de la aplicación de Marketo, que forma parte del paquete Sales Insight Salesforce.

* **My Marketo Tile Update - Sales Insight Actions**: Los administradores de Marketo (y los usuarios que designen) ahora pueden navegar rápidamente a su instancia de Acciones de perspectiva de ventas a través de un nuevo mosaico de Acciones de perspectiva de ventas ubicado en la página Mi Marketo .

## Conexión de ventas {#sales-connect}

* **Actualización de la API de Salesforce**: Con la versión de verano de 22 de Salesforce, las versiones heredadas de API 21-30 ya no serán compatibles con Salesforce. Con esta versión del Marketo Engage, todas las solicitudes de conexión de ventas que utilizan versiones de API heredadas se han actualizado para permanecer en una versión compatible. Para obtener más información sobre los planes de retiro de la API de Salesforce, haga clic en [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## Mejoras de API {#api-enhancements}

* **Nuevas funciones de filtrado para la API de extracción de miembros de un programa en lote**: Filtre por estado de pertenencia al programa, fecha de actualización, cadencia o contenido agotado para refinar el conjunto de datos extraído.

* **Mejora de la API de Extracción de miembros de un programa masivo**: Especifique hasta 10 programas durante la creación del trabajo para mejorar el rendimiento.

## Anuncios {#announcements}

* **Desaprobación de Forms: Forms 1.0, extremo de captura/guardado de posibles clientes y versiones sin script de formularios**: La compatibilidad con los recursos de Forms 1.0 se eliminará completamente de Marketo Engage en octubre de 2022. Todos los recursos de Forms 1.0 existentes dejarán de funcionar. Los formularios de Marketo Engage requerirán que JavaScript se cargue en páginas de aterrizaje y sitios web.

**_Seminario web sobre la versión del producto_**

Únase a nosotros el 24 de agosto de 2022 a las 9:00 am PT / 12:00 pm ET para un [seminario web en directo](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} alojado por nuestro equipo de productos, donde puede aprender a utilizar las últimas innovaciones de productos.
