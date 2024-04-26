---
unique-page-id: 6848747
description: Descripciones de los permisos de funciones - Documentos de Marketo - Documentación del producto
title: Descripciones de los permisos de funciones
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: 548f3f84bf6a7d39dadbf1eb5069618c4f4d44b5
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 15%

---

# Descripciones de los permisos de funciones {#descriptions-of-role-permissions}

A continuación, se muestra una lista de todos los permisos disponibles que puede asignar a sus funciones. Los permisos generalmente están asociados con áreas funcionales específicas dentro de Marketo y pueden ayudarle a controlar a qué áreas y funcionalidades tienen acceso distintos usuarios.

Información adicional sobre los permisos:

* El permiso &quot;Acceso&quot; proporciona un permiso de función para ver y, a veces, editar esa parte de la aplicación.
* Para que una función tenga acceso a los subpermisos (&quot;Crear&quot;, &quot;Eliminar&quot;, etc.), dicha función debe tener permiso de &quot;Acceso&quot; a esa parte de la aplicación. Por ejemplo, si desea conceder permiso a alguien para editar campañas, debe tener permiso general para acceder a las actividades de marketing.
* Puede ver acciones o recursos que no tiene permiso para utilizar. Sin embargo, si intenta acceder a ellos, verá un mensaje que le advierte sobre su acceso limitado.

## Permisos disponibles {#available-permissions}

Cuando usted [crear o editar un rol](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), puede seleccionar cuál de los siguientes permisos permite esa función marcando las casillas correspondientes.

![](assets/descriptions-of-role-permissions-1.png)

## Acceder a Administración  {#access-admin}

Vea y realice cambios en la configuración en la sección Mi cuenta de Admin.

* Acceso a Adobe Connect: otorga a los usuarios acceso a la pantalla de Adobe Connect
* Acceso a Adobe Experience Manager&#42; : otorga a los usuarios acceso a la pantalla de Adobe Experience Manager
* Asignación de organización de Adobe de acceso&#42; : otorga a los usuarios acceso a la pantalla Asignación de organizaciones de Adobe
* Registro de auditoría de administración de acceso&#42; : otorga a los usuarios acceso a la pantalla Registro de auditoría de administración
* Registro de auditoría de acceso&#42; : otorga a los usuarios acceso a la pista de auditoría de acceso
* Pista de auditoría de acceso: otorga a los usuarios acceso a la pista de auditoría de recursos y a la pista de auditoría de administración
* Acceso a CAPTCHA: acceso a la pantalla CAPTCHA
* Acceso a canales: otorga a los usuarios acceso solo para modificar la etiqueta Canal, no otras etiquetas personalizadas
* Límite de comunicación de acceso: otorga a los usuarios acceso para habilitar un límite de comunicación en la administración
* Acceso a CRM: otorga a los usuarios acceso a CRM, como [!DNL Salesforce] o [!DNL Microsoft Dynamics], en Administración
* Acceso [[!DNL Data.com]](https://data.com) : otorga a los usuarios acceso a la acción de flujo Data.com
* Acceso a la administración de correo electrónico: otorga a los usuarios acceso a la administración de correo electrónico para cambiar la configuración predeterminada, como cancelar la suscripción y personalizar la marca de los dominios
* Acceso a socios de eventos: otorga a los usuarios acceso a LaunchPoint en administración
* Acceso a Administración de campos: otorga a los usuarios acceso a Administración de campos en Administración
* Carga de archivos de Access: permite a los usuarios cargar imágenes y archivos en Design Studio
* Acceso a páginas de aterrizaje: otorga a los usuarios acceso a las páginas de aterrizaje en la administración
* Ubicación de acceso: otorga a los usuarios acceso a Ubicación en la administración para establecer el idioma, la configuración regional, la zona horaria y la moneda predeterminados
* Acceder al historial de inicio de sesión: otorga a los usuarios acceso al historial de inicio de sesión del usuario en la pista de auditoría
* Configuración de inicio de sesión con acceso: otorga a los usuarios acceso a la configuración de inicio de sesión en Administración para la configuración de seguridad, restricciones de IP e informes de listas inteligentes
* Acceder a nueva experiencia&#42; : otorga a los usuarios acceso a la pantalla Nueva experiencia
* Acceso a la actividad personalizada de Marketo: otorga a los usuarios acceso a las actividades personalizadas de Marketo en Administración
* Acceso al objeto personalizado de Marketo: otorga a los usuarios acceso a los objetos personalizados de Marketo en la administración
* Acceso [!DNL Munchkin] - Acceso de los usuarios de GIves a [!DNL Munchkin] en Administración, para configurar el código de seguimiento, el seguimiento de personas y habilitar la configuración de la API
* Acceso a Predictive Audiences&#42; : otorga a los usuarios acceso a la pantalla Audiencias predictivas
* Acceso a Revenue Cycle Analytics: otorga a los usuarios acceso a Revenue Cycle Analytics en Administración para configurar la sincronización de resumen y atribución
* Acceder a funciones: otorga a los usuarios acceso para administrar y editar funciones, pero no para los usuarios
* Acceder a la perspectiva de ventas: otorga a los usuarios acceso para administrar la perspectiva de ventas en Administración, para establecer el estado, la configuración de la API, la puntuación de persona y otras configuraciones
* Acceso al inicio de sesión único: otorga a los usuarios acceso para administrar el inicio de sesión único en la administración, para habilitar SAML y trabajar con la configuración de SAML y redirigir las direcciones URL de la página
* Acceso a campaña inteligente: otorga a los usuarios acceso a la campaña inteligente en administración, para restringir los límites de personas calificadas
* Acceso a la API de SOAP: otorga a los usuarios acceso para administrar las API de SOAP en los servicios web de administración
* Etiquetas de acceso: otorga a los usuarios acceso a todas las etiquetas personalizadas excepto a la etiqueta de canal
* Acceder al cofre del tesoro: otorga a los usuarios acceso a las características experimentales del cofre del tesoro en Administración
* Acceder a usuarios: otorga a los usuarios acceso para editar y administrar usuarios (pero no funciones) en Administración
* Acceder a webhooks: otorga a los usuarios acceso a los webhooks en administración para configurar detalles y asignaciones de respuestas
* Acceso a espacios de trabajo y particiones: otorga a los usuarios acceso para crear, editar y eliminar espacios de trabajo y particiones en la administración

_&#42;Para evitar interrupciones a los usuarios existentes, este permiso se introduce en modo pasivo y es visible, pero no accesible en este momento. Comunicaremos cómo implementarlo cuando se active a mediados de 2024._

## Acceder a API  {#access-api}

Otorga a los usuarios el **Solo API** **Rol** Acceda a las API individuales que se enumeran a continuación.

* Aprobar recursos
* Ejecutar campaña
* Actividad de solo lectura
* Metadatos de la actividad de solo lectura
* Recursos de solo lectura
* Campaña de solo lectura
* Compañía de solo lectura
* Objeto personalizado de solo lectura
* Persona de solo lectura
* Cuenta nombrada de solo lectura
* Oportunidad de solo lectura
* Persona de ventas de solo lectura
* Actividad de solo escritura
* Metadatos de la actividad de escritura y lectura
* Recursos habilitados para lectura y escritura
* Campaña habilitada para lectura y escritura
* Compañía habilitada para lectura y escritura
* Objeto personalizado habilitado para lectura y escritura
* Persona de escritura-lectura
* Cuenta nombrada de lectura y escritura
* Oportunidad habilitada para lectura y escritura
* Persona de ventas habilitada para lectura y escritura

## Acceder a Análisis {#access-analytics}

Proporciona a los usuarios acceso a las pestañas de Analytics, a las perspectivas de correo electrónico, a los informes y a los tres elementos siguientes, a menos que estén desmarcados.

* Al desmarcar se elimina el acceso del usuario al Explorador de ingresos
* Crear informe&#42; : otorga a los usuarios acceso para crear, clonar, leer, actualizar y mover recursos de informes en Analytics y actividades de marketing, así como recursos del Modelador del ciclo de ingresos
* Eliminar informe: al desmarcar se elimina la capacidad del usuario para eliminar informes
* Exportar datos de Analytics: al desmarcar se elimina la capacidad del usuario para exportar datos de Analytics

_&#42;Para evitar interrupciones a los usuarios existentes, este permiso se introduce en modo pasivo y es visible, pero no accesible en este momento. Comunicaremos cómo implementarlo cuando se active a mediados de 2024._

## Acceder a presentaciones del calendario {#access-calendar-presentations}

Proporciona a los usuarios acceso a las presentaciones del calendario; habilita la visualización del botón Presentations en la parte inferior.

* Editar calendario Presentations: permite a los usuarios editar presentaciones en el calendario

## Acceder a Estudio de diseño {#access-design-studio}

Proporciona a los usuarios acceso a la ficha Design Studio y a la vista del árbol, pero no a los detalles.

* Acceder a Correo electrónico
   * Editar correo electrónico: otorga a los usuarios permiso para editar, crear y clonar correos electrónicos
      * Hacer que el correo electrónico sea operativo: otorga permiso a los usuarios para hacer que un correo electrónico sea operativo. Consulte: [Hacer que un correo electrónico sea operativo](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Aprobar correo electrónico: permite a los usuarios aprobar correos electrónicos.
      * Eliminar correo electrónico: permite a los usuarios eliminar correos electrónicos.
      * Establecer dominio con marca: permite a los usuarios trabajar con dominios con marca. Consulte: [Añadir un dominio de promoción de otras marcas](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Acceder a Plantilla de correo electrónico

   * Aprobar plantilla de email
   * Eliminar plantilla de email
   * Editar plantilla de correo electrónico: editar, crear y clonar plantillas de correo electrónico

* Acceder a Formulario

   * Aprobar formulario
   * Eliminar formulario
   * Editar formulario: editar, crear y clonar formularios

* Acceder a Imagen

   * Eliminar imagen
   * Cargar imagen

* Acceder a Página de destino

   * Aprobar página de destino
   * Eliminar página de destino
   * Editar página de aterrizaje: edite, cree y clone páginas de aterrizaje

* Acceder a Plantilla de página de destino

   * Aprobar plantilla de página de destino
   * Eliminar plantilla de página de destino
   * Editar plantilla de página de aterrizaje: edite, cree y clone plantillas de página de aterrizaje

* Acceder a Fragmento

   * Aprobar fragmento
   * Eliminar fragmento
   * Editar fragmento

* Acceder a Aplicación social

   * Aprobar aplicación social
   * Eliminar aplicación social
   * Editar aplicación social

## Acceder a la base de datos {#access-database}

Vea la base de datos, así como las listas inteligentes/estáticas.

* Acceder a Segmentación

   * Aprobar segmentación
   * Eliminar segmentación
   * Editar segmentación

* Eliminar persona
* Crear lista&#42;
   * Acceso para crear un recurso de lista en actividades de base de datos y marketing
   * Acceso para crear un recurso de lista inteligente en actividades de base de datos y marketing
* Eliminar lista
* Editar persona: evita la edición manual y la ejecución de pasos de flujo únicos; aún puede editar personas ejecutando campañas en su contra
* Exportar persona: exporte hojas de cálculo con desde las listas de la base de datos
* Importar personalizados
* Lista de importación
* Combinar personas
* Ejecutar acciones de flujo único: permite a los usuarios ejecutar **Cambiar valor de datos** paso de flujo en las personas de la base de datos

* Ver datos de oportunidad: oculta la información de la oportunidad en la página de detalles de la persona

_&#42;Para evitar interrupciones a los usuarios existentes, este permiso se introduce en modo pasivo y es visible, pero no accesible en este momento. Comunicaremos cómo implementarlo cuando se active a mediados de 2024._

## Acceder a Actividades de marketing {#access-marketing-activities}

Vea la pestaña Actividades de marketing, las campañas y las carpetas de campaña.

* Acceder a mensaje SMS

   * Aprobar mensaje SMS
   * Eliminar mensaje SMS
   * Editar mensaje SMS

* Acceder a la notificación de inserción

   * Aprobar notificación de inserción
   * Eliminar notificación de inserción
   * Editar notificación de inserción

* Acceder a recompensas
* Activar campaña desencadenadora
* Aprobar programa de email
* Clonar recurso de marketing
* Eliminar recurso de marketing
* Editar restricciones de campaña
* Editar recurso de marketing
* Exportar actividad de campaña&#42;
* Importar programa
* Lista de importación
* Programar campaña por lotes

Acceder al SEO

* Administrar SEO
* SEO estándar

_&#42;Para evitar interrupciones a los usuarios existentes, este permiso se introduce en modo pasivo y es visible, pero no accesible en este momento. Comunicaremos cómo implementarlo cuando se active a mediados de 2024._

## Enfoque y personalización {#targeting-and-personalization}

* Administración de personalización web
* Editor de campañas principales
* Lanzador de campañas CRE
* Editor de campañas web
* Selector de campañas web

Administración del espacio de trabajo

* Acceso de administrador para un espacio de trabajo específico (solo si tiene espacios de trabajo habilitados)
* Mover recursos entre espacios de trabajo (solo si están habilitados los espacios de trabajo)
