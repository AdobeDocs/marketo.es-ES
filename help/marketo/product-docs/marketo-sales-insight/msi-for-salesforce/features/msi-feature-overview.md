---
unique-page-id: 37356893
description: Información general sobre las funciones de MSI - Documentos de Marketo - Documentación del producto
title: Información general de características de MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
source-git-commit: 7a6108b3c68c5845fcf0169b111e058596e3d4a6
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 4%

---

# Información general de características de MSI {#msi-feature-overview}

MSI tiene las siguientes funciones disponibles en Salesforce Lightning y Classic.

## Panel de VisualForce {#visualforce-panel}

El panel de fuerza visual MSI incluye las siguientes funcionalidades:

* Pestañas

   * [Panel de perspectivas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Momento interesante
   * Actividad web
   * Email
   * Puntuación

* Acciones

   * Añadir a Marketo Campaign
   * Enviar correo electrónico de Marketo
   * Agregar o quitar de la lista de observación

* Estrellas y llamas

## Diseño de posible cliente {#lead-layout}

Páginas de fuerza visual:

* Posible cliente: incluye la opción de hacer clic en &quot;Ir a la lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI será visible en un diseño de página completa
* Lista completa de posibles clientes: no incluye la opción &quot;Ir a lista completa&quot;
* Lead Mobile: visible en la aplicación móvil de Salesforce
* Puente de contacto de posible cliente : muestra el panel MSI del contacto que ha agregado en el campo ID de contacto MSI

Campos:

* Último momento interesante
* Fecha del último momento interesante
* Descripción del último momento interesante
* Origen del último momento interesante
* Tipo del último momento interesante
* Última actividad de Marketo por ventas
* Última participación de Marketo por ventas
* Puntaje relativo
* Valor de puntuación relativo
* Urgencia
* Valor de urgencia
* Ver en Marketo : haga clic en este campo para abrir una vista no editable del posible cliente en Marketo. Incluye: Información de posible cliente, información de la empresa, información de posible cliente de SFDC, campos personalizados de SFDC, registro de actividades
* ID de contacto MSI: agregue un contacto de Salesforce a este campo e incluya el panel &quot;Puente de contacto de posible cliente&quot; en el diseño de posible cliente para ver el panel MSI del contacto

## Diseño de contacto {#contact-layout}

Páginas de fuerza visual:

* Contacto: incluye la opción de hacer clic en &quot;Ir a lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI será visible en un diseño de página completa
* Contacto Lista completa: no incluye la opción &quot;Ir a lista completa&quot;
* Contacto con Mobile: visible en la aplicación móvil de Salesforce
* Agregar a la página de contacto de Marketo Campaign: la función Agregar a Marketo Campaign está disponible en este panel

Campos:

* Último momento interesante
* Fecha del último momento interesante
* Descripción del último momento interesante
* Origen del último momento interesante
* Tipo del último momento interesante
* Última actividad de Marketo por ventas
* Puntaje relativo
* Valor de puntuación relativo
* Urgencia
* Valor de urgencia
* Ver en Marketo : haga clic en este campo para abrir una vista no editable del posible cliente en Marketo. Incluye: Información de posible cliente, información de la empresa, información de posible cliente de SFDC, campos personalizados de SFDC, registro de actividades
* Puntuación de posibles clientes de Mkto
* Perspectiva de ventas: abre la página de lista completa de contactos

## Diseño de la cuenta {#account-layout}

Páginas de fuerza visual:

* Cuenta: incluye la opción de hacer clic en &quot;Ir a la lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI será visible en un diseño de página completa
* Lista completa de la cuenta: no incluye la opción &quot;Ir a la lista completa&quot;
* Móvil de cuenta: visible en la aplicación móvil de Salesforce

Campos:

* Perspectiva de ventas: abre la página de lista completa de contactos

Acciones:

* Añadir a Marketo Campaign
* Enviar correo electrónico de Marketo
* Agregar o quitar de la lista de observación

Las siguientes funciones son **no disponible** en la página Diseño de cuenta :

* Estrellas y llamas

## Diseño de oportunidad {#opportunity-layout}

Páginas de fuerza visual:

* Oportunidad : incluye la opción de hacer clic en &quot;Ir a lista completa&quot;, se le enviará a una nueva pestaña en Salesforce donde el panel MSI será visible en un diseño de página completa
* Lista completa de oportunidades: no incluye la opción &quot;Ir a lista completa&quot;
* Oportunidad móvil: visible en la aplicación móvil de Salesforce

Campos:

* Perspectiva de ventas: abre la página de lista completa de contactos
* Análisis de oportunidades de Marketo: abre el Analizador de influencias de oportunidades en Marketo

Acciones:

* Añadir a Marketo Campaign
* Enviar correo electrónico de Marketo
* Agregar o quitar de la lista de observación

Las siguientes funciones son **no disponible** en la página Diseño de oportunidad:

* Estrellas y llamas

## Vista Lista de posibles clientes y contactos (acciones masivas) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning: Agregue a la lista de observación, Añadir a Marketo Campaign y Enviar correos electrónicos de Marketo botones de acción masiva en la vista de lista de posibles clientes y contactos .

Salesforce Classic: Agregue a la lista de observación, Añadir a Marketo Campaign y Enviar botones de acción masiva de correo electrónico de Marketo en la vista de lista de posibles clientes y contactos .

## Ficha Marketo {#marketo-tab}

* Mejores apuestas

   * Incluye la capacidad de crear y editar vistas. Posibilidad de ocultar las mejores apuestas según la configuración de la opción &quot;Ocultar predeterminado&quot; en la página Configuración de Marketo
   * Columnas: Nombre, Cuenta, Último Momento Interesante, Encabezado De Estado, Participación (Estrellas Y Flames), Ocultar

* Mi lista de observación

   * Incluye la capacidad de crear y editar vistas
   * Columnas: Nombre, Cuenta, Último Momento Interesante, Encabezado De Estado, Participación (Estrellas Y Flames), Quitar

* Actividad web

   * Incluye la capacidad de crear y editar vistas y la funcionalidad del filtro de intervalo de tiempo
   * Columna : vista de página, nombre, cuenta, última visita

* Actividad web anónima

   * Incluye la capacidad de crear y editar vistas y la funcionalidad del filtro de intervalo de tiempo
   * Columnas: vista de página, empresa, última visita, investigación (abre la página de LinkedIn de la empresa)

* Mi correo electrónico

   * Incluye la capacidad de crear y editar vistas
   * Columnas: Nombre, Cuenta, Asunto, Fecha, Abrir, Haga Clic

* Fuente de posibles clientes : incluye la capacidad de suscribirse a momentos interesantes, la fuente RSS de la página de configuración debe estar habilitada para utilizar esta función

   * Plomo/Contacto que tuvo este interesante momento
   * Tipo de momento interesante (web, correo electrónico o hito) y descripción
   * Nombre de la cuenta
   * Momento en que ocurrió este momento interesante
   * Suscribirse opción para recibir una notificación por correo electrónico para este tipo de evento
   * Icono de alta prioridad para mostrar que esta persona es una apuesta recomendada

## Ficha Configuración de la perspectiva de ventas de Marketo {#marketo-sales-insight-configuration-tab}

* Configuración operativa: Incluye las credenciales de API Soap &amp; Rest necesarias para configurar MSI en SFDC
* Configuración de MSI: Incluye la configuración de la pestaña Marketo y el panel de fuerza visual MSI
* Restablecer la perspectiva de ventas de Marketo: Incluye la capacidad de borrar todas las configuraciones

>[!MORELIKETHIS]
>
>[Ficha Configuración de la perspectiva de ventas de Marketo en Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Informes de rendimiento de perspectivas de ventas {#sales-insight-performance-reports}

Ver el rendimiento de los correos electrónicos enviados a través de Salesforce, Microsoft Dynamics o un complemento de Gmail o Outlook

## MSI para dispositivos móviles {#msi-for-mobile}

Las funciones MSI son compatibles con la aplicación móvil de Salesforce

## Compatibilidad de idiomas {#language-support}

Marketo Sales Insight se almacena por idioma. Por lo tanto, si desea que funcione para más de un idioma, debe introducir las credenciales por separado para cada idioma.

>[!NOTE]
>
>Un contacto/posible cliente debe estar en la partición Default para poder agregarse a la lista Watchlist.
