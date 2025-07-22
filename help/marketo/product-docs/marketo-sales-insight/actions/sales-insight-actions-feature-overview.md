---
description: Información general sobre la función Acciones de Insight de ventas - Documentos de Marketo - Documentación del producto
title: Resumen de la función Acciones de Insight de ventas
exl-id: 059de248-d1a2-42cd-a7ec-f10b15d0b526
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1361'
ht-degree: 0%

---

# Resumen de la función Acciones de Insight de ventas {#msi-actions-feature-overview}

Acelere los esfuerzos de prospección con herramientas de participación e inteligencia impulsadas por marketing en un solo flujo de trabajo mediante las acciones de Insight de ventas.

>[!NOTE]
>
>Marketo Sales Insight Actions es una aplicación basada en la Web que se integra exclusivamente con Salesforce CRM mediante el [paquete Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. A veces se denomina &quot;Ventas Marketo&quot; o simplemente &quot;Acciones&quot;.

Para ver un vídeo introductorio de las acciones de Sales Insight, [haga clic aquí](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/sales-insight-actions/overview.html?lang=es){target="_blank"}.

![](assets/sales-insight-actions-feature-overview-1.png)

## Diseño del posible cliente y diseño del contacto {#lead-layout-and-contact-layout}

Las siguientes acciones están disponibles en la lista desplegable &quot;Elegir acciones&quot; de la barra de navegación superior:

* Enviar correo electrónico de ventas
   * Los correos electrónicos de ventas tienen seguimiento de visualización, clics y respuestas (cuando se configura el canal de entrega)
   * Incluye Personalization de correo electrónico, firma personalizada y archivos adjuntos
   * Uso compartido de plantillas e informes
   * Uso compartido de equipos, correos electrónicos de grupos y capacidad para CC/CCO
   * La actividad de correo electrónico de ventas se registrará en el registro de persona de Marketo
   * Filtros y déclencheur correspondientes en Marketo Smart Campaigns (detalles a continuación)

* Agregar a la campaña de ventas
   * Añadir posibles clientes a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas
   * Incluye acceso y uso compartido de equipos, generación de tareas, omisión de fines de semana, omisión de correos electrónicos OOO como respuestas y finalización automática
   * La actividad de la campaña se registrará en el registro personal de Marketo
   * Filtros y déclencheur correspondientes en Marketo Smart Campaigns (detalles a continuación)

* Llamada de ventas
   * Realizar llamadas de ventas utilizando el marcador dentro de CRM
   * Incluye presencia local, pregrabada
   * Registra el resultado de la llamada, la grabación de llamadas en el panel y el historial de actividades
   * La actividad de llamada se registrará en el registro de persona de Marketo
   * Filtros y Déclencheur en campañas inteligentes de Marketo

* Agregar tarea
   * Crear correo electrónico, llamadas, InMail y tareas personalizadas para los posibles clientes
   * Automatización de la creación de tareas con campañas de ventas
   * Sincronizar tareas con [!DNL Salesforce]
   * Registrar tareas en [!DNL Salesforce] sección Historial de actividades

Para acceder a Live Feed, haga clic en el icono ((0)) de la barra de navegación superior. Incluye la posibilidad de ver actualizaciones en directo sobre las actividades de ventas, así como la capacidad de acoplamiento de pantalla.

![](assets/sales-insight-actions-feature-overview-2.png)

Los siguientes datos están disponibles en las pestañas del panel MSI:

* Tablero de perspectivas
   * La cuadrícula de velocidad de participación incluirá actividades de Correos electrónicos de ventas, Acciones de campañas de ventas y Llamadas de ventas
   * Próximas campañas de ventas: cuando un posible cliente forma parte de una campaña en curso, esta información está disponible en la pestaña Próximas campañas de ventas
   * Próximas tareas: cuando se aproxima una tarea que pertenece a un posible cliente, esta información está disponible en la pestaña de próximas tareas

* Pestaña Correo electrónico
   * Todos los correos electrónicos de ventas enviados se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
   * Las columnas incluyen Asunto, Abrir, Clic, Respondido (disponible solo para correo electrónico de ventas con canal de entrega configurado), Remitente, Fecha
   * Incluye una tarjeta deslizable con detalles adicionales como remitente, plantilla, campaña de ventas y vista previa de correo electrónico

* Pestaña Llamada
   * Todas las llamadas realizadas con la función de marcador de ventas se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
   * Las columnas incluyen Nombre, Resultado, Notas, Llamado en, Duración y vínculo a la grabación
   * Incluye una tarjeta deslizable con detalles adicionales como Llamada realizada por, Llamada respondida por, Número de teléfono y Estado

## Diseño de cuenta y oportunidad {#account-and-opportunity-layout}

Las siguientes acciones están disponibles en la barra de navegación superior:

* Envío de correo electrónico de ventas: capacidad para enviar correos electrónicos de grupo personalizados o con plantilla con seguimiento de visualización, clics y respuestas a todos los contactos asociados a una cuenta u oportunidad
   * Los correos electrónicos de ventas tienen seguimiento de visualización, clics y respuestas (cuando se configura el canal de entrega)
   * Incluye Personalization de correo electrónico, firma personalizada y archivos adjuntos
   * Uso compartido de plantillas e informes
   * Uso compartido de equipos, correos electrónicos de grupos y capacidad para CC/CCO
   * La actividad de correo electrónico de ventas se registrará en el registro de persona de Marketo
   * Filtros y déclencheur correspondientes en Marketo Smart Campaigns (detalles a continuación)

* Añadir a la campaña de ventas: añade todos los contactos asociados a una cuenta u oportunidad a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas
   * Añadir posibles clientes a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas
   * Incluye acceso y uso compartido de equipos, generación de tareas, omisión de fines de semana, omisión de correos electrónicos OOO como respuestas y finalización automática
   * La actividad de la campaña se registrará en el registro personal de Marketo
   * Filtros y déclencheur correspondientes en Marketo Smart Campaigns (detalles a continuación)

Para acceder a Live Feed, haga clic en el icono ((0)) en la barra de navegación superior. Incluye la posibilidad de ver actualizaciones en directo sobre las actividades de ventas, así como la capacidad de acoplamiento de pantalla.

Los siguientes datos están disponibles en las pestañas:

* Tablero de perspectivas
   * La cuadrícula de velocidad de participación incluirá actividades de Correos electrónicos de ventas, Acciones de campañas de ventas y la Llamada de ventas
   * Próximas campañas de ventas: cuando un contacto de la cuenta/oportunidad forme parte de una campaña en curso, esta información estará disponible en la pestaña Próximas campañas de ventas
   * Próximas tareas: cuando haya una próxima tarea perteneciente a un contacto desde la cuenta o la oportunidad, esta información estará disponible en la pestaña de próximas tareas

* Pestaña Correo electrónico
   * Todos los correos electrónicos de ventas enviados a los contactos desde la cuenta/oportunidad se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
   * Las columnas incluyen Asunto, Abrir, Clic, Respondido (disponible solo para correo electrónico de ventas con canal de entrega configurado), Remitente y Fecha
   * Incluye una tarjeta deslizable con detalles adicionales como remitente, plantilla, campaña de ventas y vista previa de correo electrónico

* Pestaña Llamada
   * Todas las llamadas realizadas a los contactos desde la cuenta/oportunidad utilizando la función de marcador de ventas se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
   * Las columnas incluyen Nombre, Resultado, Notas, Llamado en, Duración y vínculo a la grabación
   * Incluye una tarjeta deslizable con detalles adicionales como Llamada realizada por, Llamada respondida por, Número de teléfono y Estado

## Vista de lista de contactos y posibles clientes (acciones masivas) {#lead-and-contact-list-view}

* [!UICONTROL Enviar correo electrónico de ventas]: capacidad para enviar correos electrónicos personalizados o con plantillas con seguimiento de vistas, clics y respuestas a una lista de contactos o posibles clientes
* [!UICONTROL Agregar a la campaña de ventas] - Agregar a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas a una lista de contactos/posibles clientes

## Pestaña Global de Marketo {#marketo-global-tab}

**[!UICONTROL Lo más probable] Ficha**

![](assets/sales-insight-actions-feature-overview-3.png)

Las siguientes acciones masivas están disponibles en la lista desplegable de la pestaña [!UICONTROL Lo mejor]:

* [!UICONTROL Enviar correo electrónico de ventas]: capacidad para enviar correos electrónicos personalizados o con plantillas con seguimiento de vistas, clics y respuestas
* [!UICONTROL Agregar a la campaña de ventas] - Agregar posibles clientes a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas

  ![](assets/sales-insight-actions-feature-overview-4.png)

Las siguientes acciones en línea están disponibles para contactos o posibles clientes individuales en la pestaña [!UICONTROL Lo mejor]:

* [!UICONTROL Enviar correo electrónico de ventas]: capacidad para enviar correos electrónicos personalizados o con plantillas con seguimiento de vistas, clics y respuestas
* [!UICONTROL Agregar a la campaña de ventas] - Agregar posibles clientes a los libros de reproducción de ventas, que es una secuencia de correos electrónicos y tareas
* [!UICONTROL Llamada de ventas] - Realice llamadas de ventas usando el marcador dentro del CRM
* [!UICONTROL Agregar tarea] - Crear tareas de correo electrónico, llamada, cliente o LinkedIn para posibles clientes potenciales

  ![](assets/sales-insight-actions-feature-overview-5.png)

**Ficha Correo electrónico**

* Todos los correos electrónicos de ventas enviados se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
* Las columnas incluyen Asunto, Abrir, Clic, Respondido (disponible solo para correo electrónico de ventas con canal de entrega configurado), Remitente y Fecha
* Incluye una tarjeta deslizable con detalles adicionales como remitente, plantilla, campaña de ventas y vista previa de correo electrónico

**Ficha de llamada**

* Todas las llamadas realizadas con la función de marcador de ventas se registrarán aquí. Las actividades también se registran en el registro de persona de Marketo
* Las columnas incluyen Nombre, Resultado, Notas, Llamado en, Duración y vínculo a la grabación
* Incluye una tarjeta deslizable con detalles adicionales como Llamada realizada por, Llamada respondida por, Número de teléfono y Estado

**Ficha de tarea**

* Las tareas de correo electrónico, llamada, InMail y personalizadas creadas y completadas estarán disponibles para la administración de tareas en esta pestaña. Incluye la capacidad de Añadir tarea
* Automatización de la creación de tareas con campañas de ventas
* Sincronizar tareas con [!DNL Salesforce]
* Registrar tareas en [!DNL Salesforce] sección Historial de actividades

  ![](assets/sales-insight-actions-feature-overview-6.png)

**Fuente en vivo**

* Posibilidad de ver actualizaciones en directo sobre las actividades de ventas junto con la capacidad de acoplamiento de pantalla
* Los botones de correo electrónico, llamada y cadencia incrustados hacen que cada insight del cliente sea procesable

## Funciones disponibles en Marketo {#features-available-in-marketo}

Actividades de ventas que se capturan en Marketo:

* Enviar correo electrónico de ventas: el usuario envió un correo electrónico de ventas a un posible cliente
* Abrir correo electrónico de ventas: el posible cliente abrió un correo electrónico de ventas enviado
* Haga clic en Correo electrónico de ventas: el posible cliente ha hecho clic en un vínculo de un correo electrónico de ventas
* Correo electrónico de ventas respondido: el posible cliente ha respondido a un correo electrónico de ventas
* Recibir llamada de ventas: el posible cliente recibió una llamada de un vendedor mediante la llamada de ventas.
* Añadir a la campaña de ventas: el posible cliente se ha añadido a una campaña de ventas creada
* Eliminado de la campaña de ventas: el posible cliente se ha eliminado de una campaña de ventas creada

Los filtros y Déclencheur incluyen:

* [!UICONTROL Se Ha Enviado El Correo Electrónico De Ventas]
* [!UICONTROL Abre El Correo Electrónico De Ventas]
* [!UICONTROL Clics en el correo electrónico de ventas]
* [!UICONTROL Respuestas al correo electrónico de ventas]
* [!UICONTROL Recibe Una Llamada De Ventas]
* [!UICONTROL Se agregó a la campaña de ventas]
* [!UICONTROL Eliminado de la campaña de ventas]

  ![](assets/sales-insight-actions-feature-overview-7.png)
