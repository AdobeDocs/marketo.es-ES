---
unique-page-id: 37356893
description: 'Información general de las funciones MSI: documentos de Marketo, documentación del producto'
title: Información general de funciones MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 7%

---

# Información general de funciones MSI {#msi-feature-overview}

MSI tiene las siguientes características disponibles en [!DNL Salesforce] Lightning y Classic.

>[!NOTE]
>
>Para ver todos los datos disponibles, asegúrese de que el zoom del navegador esté configurado en no más del 125% cuando utilice Windows y del 150% en el sistema operativo Mac.

## Visualforce Panel {#visualforce-panel}

MSI Visualforce Panel incluye las siguientes funcionalidades:

* Pestañas

   * [Tablero de perspectivas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Momentos interesantes
   * Actividad en la web
   * Correo electrónico
   * Puntuación

* Acciones

   * Añadir a Marketo Campaign
   * Enviar correo electrónico a Marketo
   * Agregar o quitar de la lista de observación

* Estrellas y llamas

## Diseño de posible cliente {#lead-layout}

Páginas de Visualforce:

* Posible cliente: incluye la opción de hacer clic en Hyper &quot;Ir a lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI será visible en un diseño de página completa
* Lista completa de posibles clientes: no incluye la opción &quot;Ir a la lista completa&quot;
* Móvil principal: visible en la aplicación móvil de Salesforce
* Bridge de contactos de clientes potenciales: muestra el panel MSI del contacto que ha agregado en el campo ID de contacto MSI

Campos:

* Último momento interesante
* Fecha del último momento interesante
* Descripción del último momento interesante
* Origen del último momento interesante
* Tipo del último momento interesante
* Última actividad de Marketo por parte de ventas
* Última participación de Marketo por parte de ventas
* Puntaje relativo
* Valor de puntuación relativa
* Urgencia
* Valor de urgencia
* Ver en Marketo: haga clic en este campo para abrir una vista no editable del posible cliente en Marketo. Incluye: información del posible cliente, información de la empresa, información del posible cliente de SFDC, campos personalizados de SFDC, registro de actividad
* ID de contacto MSI: agregue un contacto de Salesforce a este campo e incluya el panel &quot;Contacto de posible cliente Bridge&quot; en la presentación del posible cliente para ver el panel MSI del contacto

## Diseño de contacto {#contact-layout}

Páginas de Visualforce:

* Contacto: incluye la opción de hacer clic en hiper &quot;Ir a la lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI estará visible en un diseño de página completa
* Lista completa de contactos: no incluye la opción &quot;Ir a la lista completa&quot;
* Contacto Móvil: visible en la aplicación móvil de Salesforce
* Agregar a la página de contacto de Marketo Campaign: la función Agregar a Marketo Campaign está disponible en este panel

Campos:

* Último momento interesante
* Fecha del último momento interesante
* Descripción del último momento interesante
* Origen del último momento interesante
* Tipo del último momento interesante
* Última actividad de Marketo por parte de ventas
* Puntaje relativo
* Valor de puntuación relativa
* Urgencia
* Valor de urgencia
* Ver en Marketo: haga clic en este campo para abrir una vista no editable del posible cliente en Marketo. Incluye: información del posible cliente, información de la empresa, información del posible cliente de SFDC, campos personalizados de SFDC, registro de actividad
* Puntuación de cliente potencial Mkto
* [!DNL Sales Insight] - Abre la página de lista completa de contactos

## Diseño de cuenta {#account-layout}

Páginas de Visualforce:

* Cuenta: incluye la opción de hacer clic en hiper &quot;Ir a la lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI estará visible en un diseño de página completa
* Lista completa de cuentas: no incluye la opción &quot;Ir a la lista completa&quot;
* Móvil de cuenta: visible en la aplicación móvil de Salesforce

Campos:

* [!DNL Sales Insight] - Abre la página de lista completa de contactos

Acciones:

* Añadir a Marketo Campaign
* Enviar correo electrónico a Marketo
* Agregar o quitar de la lista de observación

Las siguientes características **no están disponibles** en la página Diseño de cuenta:

* Estrellas y llamas

## Diseño de oportunidad {#opportunity-layout}

Páginas de Visualforce:

* Oportunidad: incluye la opción de hacer clic en hiper &quot;Ir a la lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI estará visible en un diseño de página completa
* Lista completa de oportunidades: no incluye la opción &quot;Ir a la lista completa&quot;
* Oportunidad móvil: visible en la aplicación móvil de Salesforce

Campos:

* [!DNL Sales Insight] - Abre la página de lista completa de contactos
* Análisis de oportunidades de Marketo: abre el Analizador de influencia de oportunidades en Marketo

Acciones:

* Añadir a Marketo Campaign
* Enviar correo electrónico a Marketo
* Agregar o quitar de la lista de observación

Las siguientes características **no están disponibles** en la página Diseño de oportunidad:

* Estrellas y llamas

## Vista de lista de contactos y posibles clientes (acciones masivas) {#lead-and-contact-list-view-bulk-actions}

[!DNL Salesforce Lightning]: botones de acción masiva Agregar a la lista de observación, Agregar a Marketo Campaign y Enviar correo electrónico de Marketo en la vista de lista de posibles clientes y contactos.

[!DNL Salesforce Classic]: los botones de acción masiva Agregar a la lista de observación, Agregar a Marketo Campaign y Enviar correo electrónico de Marketo en la vista de lista de posibles clientes y contactos.

## Pestaña Marketo {#marketo-tab}

* [!DNL Best Bets]

   * Incluye la capacidad de crear y editar vistas. Posibilidad de ocultar los resultados más probables en función de la configuración de la opción &quot;Ocultar predeterminados&quot; en la página Configuración de Marketo
   * Columnas: Nombre, Cuenta, Último momento interesante, Encabezado de estado, Participación (estrellas y llamas), Ocultar

* Mi lista a observar

   * Incluye la capacidad de crear y editar vistas
   * Columnas: Nombre, Cuenta, Último momento interesante, Encabezado de estado, Participación (estrellas y llamas), Eliminar

* Actividad en la web

   * Incluye la capacidad de crear y editar vistas y la funcionalidad de filtro de lapso de tiempo
   * Columna: vista de página, nombre, cuenta, última visita

* Actividad web anónima

   * Incluye la capacidad de crear y editar vistas y la funcionalidad de filtro de lapso de tiempo
   * Columnas: vista de página, compañía, última visita, referencia (abre la página de LinkedIn de la compañía)

* Mi correo electrónico

   * Incluye la capacidad de crear y editar vistas
   * Columnas: nombre, cuenta, asunto, fecha, apertura, clic

* Fuente de posibles clientes: incluye la capacidad de suscribirse a momentos interesantes, la fuente RSS de la página de configuración debe estar habilitada para utilizar esta función

   * Posible cliente/contacto que ha tenido este momento interesante
   * Tipo de momento interesante (web, correo electrónico o hito) y descripción
   * Nombre de la cuenta
   * Hora a la que ocurrió este momento interesante
   * Opción Suscribirse para recibir notificaciones por correo electrónico para este tipo de evento
   * Icono de alta prioridad para mostrar que esta persona es lo más probable

## [!DNL Marketo Sales Insight] ficha de configuración {#marketo-sales-insight-configuration-tab}

* Configuración operativa: incluye las credenciales de la API de SOAP y REST necesarias para configurar MSI en SFDC
* Configuración de MSI: incluye la configuración de la pestaña de Marketo y el panel MSI visual force
* Restablecer [!DNL Marketo Sales Insight]: incluye la capacidad de borrar todas las configuraciones

>[!MORELIKETHIS]
>
>[[!DNL Marketo Sales Insight] Ficha de configuración en [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## [!DNL Sales Insight] informes de rendimiento {#sales-insight-performance-reports}

Ver el rendimiento de los mensajes de correo electrónico enviados a través de [!DNL Salesforce], [!DNL Microsoft Dynamics] o un complemento de Gmail o [!DNL Outlook]

## MSI para dispositivos móviles {#msi-for-mobile}

Las características de MSI son compatibles con la aplicación móvil [!DNL Salesforce]

## Compatibilidad de idiomas {#language-support}

[!DNL Marketo Sales Insight] se almacena por idioma. Por lo tanto, si desea que funcione para más de un idioma, debe introducir las credenciales por separado para cada idioma.

>[!NOTE]
>
>* Un contacto/posible cliente debe estar en la partición predeterminada para poder agregarse a la lista de observación.
>
>* El paquete MSI [!DNL Salesforce] no admite la vista personalizada con campos dependientes.
