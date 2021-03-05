---
unique-page-id: 6848747
description: Descripciones de los permisos de funciones - Marketo Docs - Documentación del producto
title: Descripciones de los permisos de funciones
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---


# Descripciones de los permisos de funciones {#descriptions-of-role-permissions}

A continuación se muestra una lista de todos los permisos disponibles que puede asignar a sus funciones. Los permisos generalmente están asociados con áreas funcionales específicas dentro de Marketo y pueden ayudarle a controlar a qué áreas y funcionalidades tienen acceso los distintos usuarios.

Información adicional sobre permisos:

* El permiso &quot;Acceso&quot; da a una función permiso para ver y a veces editar esa parte de la aplicación.
* Para que una función tenga acceso a los subpermisos (&quot;Crear&quot;, &quot;Eliminar&quot;, etc.), esa función debe tener permiso de &quot;Acceso&quot; a esa parte de la aplicación. Por ejemplo, si desea conceder a alguien permiso para Editar campañas, debe tener permiso general para acceder a las actividades de marketing.
* Puede ver acciones o recursos que no tiene permiso para usar. Sin embargo, si intenta acceder a ellos, verá un mensaje en el que se le advierte sobre su acceso limitado.

## Permisos disponibles {#available-permissions}

Cuando [crea o edita una función](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), puede seleccionar cuál de los siguientes permisos permite esa función marcando las casillas adecuadas.

![](assets/createnewrole.png)

## Acceso al administrador {#access-admin}

Vea y realice cambios en la configuración en la sección Mi cuenta de Administración.

* Acceso a la pista de auditoría : otorga a los usuarios acceso a la pista de auditoría de recursos y a la pista de auditoría de administración
* Canales de acceso : otorga a los usuarios acceso solo para modificar la etiqueta Canal, no otras etiquetas personalizadas
* Límite de comunicación de acceso : otorga a los usuarios acceso para habilitar un límite de comunicación en el administrador
* Acceso a CRM : otorga a los usuarios acceso a CRM, como Salesforce o Microsoft Dynamics, en Admin
* Acceso [Data.com](https://Data.com) : otorga a los usuarios acceso a la acción de flujo de Data.com
* Acceso al administrador de correo electrónico : otorga a los usuarios acceso al administrador de correo electrónico para cambiar la configuración predeterminada, como cancelar suscripción y personalizar la marca de los dominios.
* Acceso a socios de eventos : otorga a los usuarios acceso a LaunchPoint en la administración
* Acceso a la administración de campos : otorga a los usuarios acceso a la administración de campos en administración
* Acceso a la carga de archivos : permite a los usuarios cargar imágenes y archivos en Design Studio.
* Acceso a las páginas de aterrizaje : otorga a los usuarios acceso a las páginas de aterrizaje en el Administrador
* Ubicación de acceso : otorga a los usuarios acceso a Ubicación en el Administrador para establecer el idioma, la configuración regional, la zona horaria y la moneda predeterminados.
* Acceso al historial de inicio de sesión : otorga a los usuarios acceso al historial de inicio de sesión del usuario en la pista de auditoría
* Acceso a la configuración de inicio de sesión : otorga a los usuarios acceso a la configuración de inicio de sesión en Administración para seguridad, restricciones de IP y configuración de informes de listas inteligentes
* Acceso a Marketo Actividad personalizada : otorga a los usuarios acceso a Marketo Actividades personalizadas en Administradores
* Acceso a Marketo Custom Object : otorga a los usuarios acceso a Marketo Personalizar objetos en Administradores
* Acceso a Munchkin : Los usuarios de GI tienen acceso a Munchkin en Administración para configurar el código de seguimiento, el seguimiento de personas y activar la configuración de API
* Acceso a Análisis de ciclo de ingresos : otorga a los usuarios acceso a Análisis de ciclo de ingresos en Administración para configurar Resumen de sincronización y Atribución
* Funciones de acceso : otorga a los usuarios acceso para administrar y editar funciones, pero no a los usuarios
* Acceso a la perspectiva de ventas : otorga a los usuarios acceso para administrar la perspectiva de ventas en el administrador, para establecer el estado, la configuración de la API, la puntuación de las personas y otros ajustes
* Acceso al inicio de sesión único : otorga a los usuarios acceso para administrar el inicio de sesión único en el administrador, para habilitar SAML y trabajar con la configuración de SAML y las direcciones URL de la página de redireccionamiento
* Acceso a Smart Campaign : otorga a los usuarios acceso a Smart Campaign en Admin para restringir los límites de personas cualificadas
* Acceso a la API de SOAP : otorga a los usuarios acceso para administrar las API de SOAP en los servicios web en la administración
* Etiquetas de acceso : otorga a los usuarios acceso a todas las etiquetas personalizadas excepto a la etiqueta Canal .
* Access Treasure Chest : otorga a los usuarios acceso a las funciones experimentales de Treasure Chest en administración
* Acceso de usuarios : otorga a los usuarios acceso para editar y administrar usuarios (pero no funciones) en Administradores
* Acceso a Webhooks : otorga a los usuarios los Webhooks en el Administrador, para configurar detalles y asignaciones de respuesta
* Acceso a espacios de trabajo y particiones : otorga a los usuarios acceso para crear, editar y eliminar espacios de trabajo y particiones en el administrador

## API de acceso {#access-api}

Proporciona a los usuarios con la **API Only** **Role** acceso a las API individuales que se enumeran a continuación.

* Aprobar recursos
* Ejecutar campaña
* Actividad de solo lectura
* Metadatos de actividad de solo lectura
* Recursos de solo lectura
* Campaña de solo lectura
* Empresa de solo lectura
* Objeto personalizado de sólo lectura
* Persona de solo lectura
* Cuenta con nombre de solo lectura
* Oportunidad de solo lectura
* Vendedor de sólo lectura
* Actividad de lectura y escritura
* Metadatos de actividades de lectura y escritura
* Recursos de lectura y escritura
* Campaña de lectura y escritura
* Empresa de lectura y escritura
* Objeto personalizado de lectura y escritura
* Lectura y escritura
* Cuenta con nombre de lectura y escritura
* Oportunidad de lectura y escritura
* Leer-Escribir persona de ventas

## Acceso a Analytics {#access-analytics}

Proporciona a los usuarios acceso a las fichas de Analytics, a las Perspectivas de correo electrónico, a los informes y a los tres elementos siguientes, a menos que no estén marcados.

* Acceso al Explorador de ingresos: la desactivación elimina el acceso del usuario al Explorador de ingresos
* Eliminar informe: al desmarcar se elimina la capacidad del usuario de eliminar informes
* Exportar datos de Analytics: al desmarcar se elimina la capacidad del usuario para exportar datos de Analytics

## Acceso a las presentaciones del calendario {#access-calendar-presentations}

Permite a los usuarios acceder a las presentaciones del Calendario : permite mostrar el botón Presentaciones en la parte inferior.

* Editar presentaciones de calendario : permite a los usuarios editar presentaciones en el calendario

## Acceso a Design Studio {#access-design-studio}

Permite a los usuarios acceder a la ficha Design Studio y a la vista del árbol, pero no a los detalles.

* Acceso a correo electrónico
   * Editar correo electrónico : otorga a los usuarios permiso para editar, crear y clonar correos electrónicos.
      * Hacer que el correo electrónico sea operativo : otorga a los usuarios permiso para hacer que un correo electrónico sea operativo. Consulte: [Hacer que un correo electrónico sea operativo](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Aprobar correo electrónico : permite a los usuarios aprobar correos electrónicos.
      * Eliminar correo electrónico : permite a los usuarios eliminar correos electrónicos.
      * Establecer dominio de marca : permite a los usuarios trabajar con dominios de marca. Consulte: [Agregar un dominio de marca adicional](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Acceso a la plantilla de correo electrónico

   * Aprobar plantilla de correo electrónico
   * Eliminar plantilla de correo electrónico
   * Editar plantilla de correo electrónico: editar, crear y clonar plantillas de correo electrónico

* Formulario de acceso

   * Eliminar formulario
   * Editar formulario: editar, crear y clonar formularios

* Acceder a imagen

   * Eliminar imagen
   * Cargar imagen

* Acceso a la página de aterrizaje

   * Aprobar página de aterrizaje
   * Eliminar página de aterrizaje
   * Editar página de aterrizaje: editar, crear y clonar páginas de aterrizaje

* Acceso a la plantilla de página de aterrizaje

   * Aprobar plantilla de página de aterrizaje
   * Eliminar plantilla de página de aterrizaje
   * Editar plantilla de página de aterrizaje: editar, crear y clonar plantillas de página de aterrizaje

* Fragmento de acceso

   * Aprobar fragmento
   * Eliminar fragmento
   * Editar fragmento

* Acceso a la aplicación social

   * Aprobar aplicación social
   * Eliminar aplicación social
   * Editar aplicación social

## Acceso a la base de datos {#access-database}

Vea la base de datos, así como vea y edite listas inteligentes/estáticas.

* Acceder a la segmentación

   * Aprobar segmentación
   * Eliminar segmentación
   * Editar segmentación

* Importación de lista avanzada
* Eliminar persona
* Eliminar lista
* Editar persona : evita la edición manual y la ejecución de pasos de flujo único; aún puede editar personas ejecutando campañas en su contra
* Exportar persona: exporte hojas de cálculo con desde las listas de bases de datos
* Importar objeto personalizado
* Lista de importación
* Combinar personas
* Ejecutar acciones de flujo único : permite a los usuarios ejecutar el paso de flujo **Cambiar valor de datos** en las personas de la base de datos

* Ver datos de oportunidad: oculta la información de oportunidad en la página de detalles de la persona

## Acceso a actividades de marketing {#access-marketing-activities}

Vea la pestaña Actividades de marketing , las campañas y las carpetas de campaña.

* Acceso al mensaje SMS

   * Aprobar mensaje SMS
   * Eliminar mensaje SMS
   * Editar mensaje SMS

* Acceso a la notificación push

   * Aprobar notificación push
   * Eliminar notificación push
   * Editar notificación push

* Premios Access
* Activar campaña
* Aprobar programa de correo electrónico
* Clonar recurso de marketing
* Eliminar recurso de marketing
* Editar restricciones de campaña
* Editar recurso de marketing
* Importar programa
* Importación de lista
* Programar campaña por lotes

Acceso a SEO

* Administración de SEO
* SEO estándar

## Segmentación y personalización {#targeting-and-personalization}

* Administrar personalización web
* Editor de campañas CRE
* Iniciador de campaña CRE
* Editor de campañas web
* Iniciador de campaña web

Administración de Workspace

* Acceso de administrador para un espacio de trabajo específico (solo si tiene espacios de trabajo habilitados)
* Mover recursos entre espacios de trabajo (solo si tiene habilitados espacios de trabajo)
