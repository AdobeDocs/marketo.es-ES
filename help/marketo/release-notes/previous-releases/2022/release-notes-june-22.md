---
description: 'Notas de la versión, junio de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, junio de 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Notas de la versión: junio de 2022 {#release-notes-june-22}

A continuación encontrará todas las funciones incluidas en la versión de junio de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

Las siguientes funciones comenzarán a lanzarse el **24 de junio de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exponer campos CreatedAt/UpdatedAt para objetos personalizados**: Permite inspeccionar estos campos en la pantalla Detalles de persona para obtener más información.

## Orquestación entre canales {#cross-channel-orchestration}

* **Uso mejorado del Diseñador de secuencias para el Dynamic Chat**: agregue tarjetas directamente desde el lienzo del Diseñador de secuencias sin necesidad de arrastrar y soltar. La interfaz de Dynamic Chat también se ha mejorado para ofrecer una mejor visibilidad del contenido en tarjetas individuales.

* **Reglas avanzadas de enrutamiento de citas para el Dynamic Chat**: el Dynamic Chat ofrece más opciones para el enrutamiento de citas segmentadas. Especifique las citas de los agentes que se deben dirigir en función de los atributos del Marketo Engage, asegurándose de que los posibles clientes se dirijan a los agentes apropiados.

* **Informes de cuadro de diálogo avanzados para Dynamic Chat**: vea el rendimiento de sus campañas de Dynamic Chat en bueno detalle con las nuevas visualizaciones de datos para las métricas de participación y conversión.

* **Desincronizar atributos de Marketo Engage no utilizados para el Dynamic Chat**: Desincronice los atributos de Marketo Engage de la suscripción de Dynamic Chat que no se utilicen, lo que le ayuda a facilitar la limpieza de los datos y permite sincronizar atributos alternativos según sea necesario.

## Experiencia de última generación

**Nuevas vistas del conmutador de alternancia**: las vistas siguientes ya están disponibles en la experiencia de próxima generación:

* [Vista de detalles de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vista de lista de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatización de experiencias {#experience-automation}

* **Exclusiones de reglas de validación de campos de formulario global**: excluya formularios específicos de las reglas de validación de formularios globales para que los centros de suscripción y otros flujos de trabajo críticos para la empresa puedan aceptar todos los valores.

* **Pasos del flujo de autoservicio**: Amplíe la conectividad entre Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para utilizarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de Déclencheur, por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de Déclencheur.

* **Seguimiento de vínculos agnósticos del protocolo de Munchkin**: Amplíe la compatibilidad con el seguimiento de `tel` y `mailto` Vínculos con Munchkin para rastrear un conjunto ampliado de comportamientos web.

* **Métodos HTTP adicionales para webhooks**: especifique PUT, PATCH y DELETE como tipos de solicitud para interactuar con servicios web.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Conjunto de permisos de información de ventas en Salesforce**: los administradores pueden proporcionar acceso a Sales Insight a un conjunto limitado de personas a nivel de usuario en lugar de a nivel de perfil mediante el conjunto de permisos de la aplicación Marketo, que forma parte del paquete de Sales Insight Salesforce.

* **Actualización del mosaico de Mi Marketo: acciones de perspectiva de ventas**: los administradores de Marketo (y los usuarios que designan) ahora pueden navegar rápidamente a su instancia de acciones de información de ventas a través de un nuevo mosaico de acciones de información de ventas ubicado en la página Mi Marketo.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Actualización de API de Salesforce**: con la versión de verano de 2022 de Salesforce, las versiones heredadas de API 21-30 ya no serán compatibles con Salesforce. Con esta versión de Marketo Engage, todas las solicitudes de Conexión de ventas que utilizan versiones de API heredadas se han actualizado para permanecer dentro de una versión admitida. Para obtener información detallada sobre los planes de retirada de la API de Salesforce, haga clic en [aquí](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Mejoras de API {#api-enhancements}

* **Nuevas funciones de filtrado para la API de extracción masiva de miembros del programa**: filtre por estado de pertenencia al programa, fecha de actualización, cadencia o contenido agotado para restringir el conjunto de datos extraídos.

* **Mejora de la API de extracción masiva de miembros del programa**: especifique hasta 10 programas durante la creación del trabajo para mejorar el rendimiento.

## Anuncios {#announcements}

* **Desaprobación de Forms: Forms 1.0, punto final de captura/guardado de posibles clientes y versiones sin script de formularios**: La compatibilidad con los recursos de Forms 1.0 se eliminará completamente de Marketo Engage en octubre de 2022. Todos los recursos existentes de Forms 1.0 dejarán de funcionar. Los formularios de Marketo Engage requerirán que JavaScript se cargue en páginas de aterrizaje y sitios web.

**_Seminario web sobre lanzamiento de productos_**

[Seminario web de junio y agosto de 2022 sobre la versión para Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
