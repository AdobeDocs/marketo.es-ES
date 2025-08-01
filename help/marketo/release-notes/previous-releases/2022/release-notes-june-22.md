---
description: 'Notas de la versión, junio de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, junio de 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Notas de la versión: junio de 2022 {#release-notes-june-22}

A continuación encontrará todas las funciones incluidas en la versión de junio de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

Las siguientes características comenzarán a lanzarse el **24 de junio de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exponer campos CreatedAt/UpdatedAt para objetos personalizados**: Permite inspeccionar estos campos en la pantalla Detalles de persona para obtener insight adicional.

## Orquestación entre canales {#cross-channel-orchestration}

* **Uso mejorado de Stream Designer para[!DNL Dynamic Chat]**: agrega tarjetas directamente desde el lienzo de Stream Designer sin necesidad de arrastrarlas y soltarlas. La interfaz [!DNL Dynamic Chat] también se ha mejorado para ofrecer una mejor visibilidad del contenido en tarjetas individuales.

* **Reglas de enrutamiento de citas avanzadas para[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] ofrece más opciones para el enrutamiento de citas de destino. Especifique las citas de los agentes que deben enrutarse según los atributos de Marketo Engage, asegurándose de que los posibles clientes se dirijan a los agentes correspondientes.

* **Informes de diálogo avanzados para[!DNL Dynamic Chat]**: vea el rendimiento de sus campañas de [!DNL Dynamic Chat] con mayor detalle mediante las nuevas visualizaciones de datos para las métricas de participación y conversión.

* **Desincronizar atributos de Marketo Engage no utilizados para[!DNL Dynamic Chat]**: desincronice los atributos de Marketo Engage de su suscripción a [!DNL Dynamic Chat] que no se usen, lo que le ayudará a facilitar la limpieza de los datos y permitirá que se sincronicen atributos alternativos según sea necesario.

## Experiencia de última generación

**Nuevas vistas de conmutador de alternancia**: Las vistas siguientes ya están disponibles en la experiencia de próxima generación:

* [Vista de detalles de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vista de lista de correo electrónico](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatización de experiencias {#experience-automation}

* **Exclusiones de reglas de validación de campos de formulario globales**: excluya formularios específicos de las reglas de validación de formularios globales para que los centros de suscripción y otros flujos de trabajo críticos para la empresa puedan aceptar todos los valores.

* **Pasos de flujo de autoservicio**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de Déclencheur, por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de Déclencheur.

* **Seguimiento de vínculos no basados en protocolos Munchkin**: amplíe la compatibilidad con el seguimiento de vínculos `tel` y `mailto` con Munchkin para realizar el seguimiento de un conjunto ampliado de comportamientos web.

* **Métodos HTTP adicionales para los enlaces web**: especifique PUT, PATCH y DELETE como tipos de solicitud para interactuar con los servicios web.

## [!DNL Sales Insight] {#sales-insight}

![(estrella)](assets/yellow-star.png)

* Conjunto de permisos de **[!DNL Sales Insight]en[!DNL Salesforce]**: los administradores pueden proporcionar acceso de [!DNL Sales Insight] a un conjunto limitado de personas a nivel de usuario en lugar de a nivel de perfil mediante el conjunto de permisos de la aplicación de Marketo, que forma parte del paquete de [!DNL Sales Insight] [!DNL Salesforce].

* **Actualización del mosaico de Mi Marketo - [!DNL Sales Insight] Acciones**: Los administradores de Marketo (y los usuarios que designen) ahora pueden navegar rápidamente a su instancia de Acciones [!DNL Sales Insight] a través de un nuevo mosaico de Acciones [!DNL Sales Insight] ubicado en la página Mi Marketo.

## [!DNL Sales Connect] {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **[!DNL Salesforce]Actualización de API**: Con la versión del verano de 2022, las versiones heredadas de API 21 -30 ya no serán compatibles con [!DNL Salesforce]. [!DNL Salesforce] Con esta versión de Marketo Engage, todas las [!DNL Sales Connect] solicitudes que utilizan versiones de API heredadas se han actualizado para permanecer dentro de una versión admitida. Para obtener detalles completos sobre [!DNL Salesforce] planes de retiro de API, haga clic [aquí](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Mejoras de API {#api-enhancements}

* **Nuevas capacidades de filtrado para la API de extracción masiva de miembros del programa**: filtre por estado de pertenencia al programa, actualización, cadencia o contenido agotado para restringir el conjunto de datos extraídos.

* **Mejora de la API de extracción de miembros de programas en lotes**: especifique hasta 10 programas durante la creación del trabajo para mejorar el rendimiento.

## Anuncios {#announcements}

* **Desaprobación de Forms: Forms 1.0, extremo de captura/guardado de posibles clientes y versiones sin script de formularios**: La compatibilidad con los recursos de Forms 1.0 se eliminará completamente de Marketo Engage en octubre de 2022. Todos los recursos existentes de Forms 1.0 dejarán de funcionar. Los formularios Marketo Engage requerirán que JavaScript se cargue en páginas de aterrizaje y sitios web.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de junio y agosto de 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
