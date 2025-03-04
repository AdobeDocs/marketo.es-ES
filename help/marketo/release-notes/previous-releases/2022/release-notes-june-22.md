---
description: 'Notas de la versión, junio de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, junio de 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Notas de la versión: junio de 2022 {#release-notes-june-22}

A continuación encontrará todas las funciones incluidas en la versión de junio de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

Las siguientes características comenzarán a lanzarse el **24 de junio de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exponer campos CreatedAt/UpdatedAt para objetos personalizados**: Permite inspeccionar estos campos en la pantalla Detalles de persona para obtener información adicional.

## Orquestación entre canales {#cross-channel-orchestration}

* **Uso mejorado de Stream Designer para Dynamic Chat**: agrega tarjetas directamente desde el lienzo de Stream Designer sin necesidad de arrastrar y soltar. La interfaz de Dynamic Chat también se ha mejorado para ofrecer una mejor visibilidad del contenido en tarjetas individuales.

* **Reglas de enrutamiento de citas avanzadas para el Dynamic Chat**: el Dynamic Chat ofrece más opciones para el enrutamiento de citas de destino. Especifique las citas de los agentes que se deben dirigir en función de los atributos del Marketo Engage, asegurándose de que los posibles clientes se dirijan a los agentes apropiados.

* **Informes de cuadros de diálogo avanzados para el Dynamic Chat**: vea el rendimiento de sus campañas de Dynamic Chat con mayor detalle mediante las nuevas visualizaciones de datos para las métricas de participación y conversión.

* **Desincronizar atributos de Marketo Engage no utilizados para Dynamic Chat**: desincronice los atributos de Marketo Engage de su suscripción de Dynamic Chat que no se usen, lo que le ayuda a facilitar la limpieza de los datos y permite sincronizar atributos alternativos según sea necesario.

## Experiencia de última generación

**Nuevas vistas de conmutador de alternancia**: Las vistas siguientes ya están disponibles en la experiencia de próxima generación:

* [Vista de detalles de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vista de lista de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatización de experiencias {#experience-automation}

* **Exclusiones de reglas de validación de campos de formulario globales**: excluya formularios específicos de las reglas de validación de formularios globales para que los centros de suscripción y otros flujos de trabajo críticos para la empresa puedan aceptar todos los valores.

* **Pasos de flujo de autoservicio**: expanda la conectividad entre el Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de Déclencheur, por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de Déclencheur.

* **Seguimiento de vínculos independientes del protocolo Munchkin**: amplíe la compatibilidad con el seguimiento de vínculos `tel` y `mailto` con Munchkin para realizar el seguimiento de un conjunto ampliado de comportamientos web.

* **Métodos HTTP adicionales para los enlaces web**: especifique el PUT, el PATCH y el DELETE como tipos de solicitud para interactuar con los servicios web.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Conjunto de permisos de Sales Insight en Salesforce**: los administradores pueden proporcionar acceso a Sales Insight a un conjunto limitado de personas a nivel de usuario en lugar de a nivel de perfil mediante el conjunto de permisos de la aplicación Marketo, que forma parte del paquete de Sales Insight Salesforce.

* **Actualización del mosaico de Mi Marketo - Acciones de perspectiva de ventas**: Los administradores de Marketo (y los usuarios que designen) ahora pueden navegar rápidamente a su instancia de Acciones de perspectiva de ventas a través de un nuevo mosaico Acciones de perspectiva de ventas ubicado en la página Mi Marketo.

## Sales Connect {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Actualización de la API de Salesforce**: con la versión del verano de 2022 de Salesforce, las versiones heredadas de la API 21 -30 ya no serán compatibles con Salesforce. Con esta versión de Marketo Engage, todas las solicitudes de Conexión de ventas que utilizan versiones de API heredadas se han actualizado para permanecer dentro de una versión admitida. Para obtener detalles completos sobre los planes de retiro de la API de Salesforce, haga clic [aquí](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Mejoras de API {#api-enhancements}

* **Nuevas capacidades de filtrado para la API de extracción masiva de miembros del programa**: filtre por estado de pertenencia al programa, actualización, cadencia o contenido agotado para restringir el conjunto de datos extraídos.

* **Mejora de la API de extracción de miembros de programas en lotes**: especifique hasta 10 programas durante la creación del trabajo para mejorar el rendimiento.

## Anuncios {#announcements}

* **Desaprobación de Forms: Forms 1.0, extremo de captura/guardado de posibles clientes y versiones sin script de formularios**: La compatibilidad con los recursos de Forms 1.0 se eliminará completamente de Marketo Engage en octubre de 2022. Todos los recursos existentes de Forms 1.0 dejarán de funcionar. Los formularios de Marketo Engage requerirán que JavaScript se cargue en páginas de aterrizaje y sitios web.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión del Marketo Engage de junio y agosto de 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
