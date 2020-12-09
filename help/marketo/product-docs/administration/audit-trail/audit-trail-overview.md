---
unique-page-id: 11377945
description: Información general de pista de auditoría - Documentos de marketing - Documentación del producto
title: Información general de pista de auditoría
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Información general de pista de auditoría {#audit-trail-overview}

La pista de auditoría le permite obtener un historial completo (seis meses) de los cambios realizados en la instancia de Marketing.

>[!NOTE]
>
>El historial de datos de seguimiento de auditoría comenzó el 14 de septiembre de 2016.

![](assets/one.png)

## ¿Qué es la pista de auditoría? {#what-is-audit-trail}

La pista de auditoría captura, en tiempo real, una lista completa de acciones y eventos que se producen dentro de una suscripción de marketing. Incluye una forma de autoservicio de acceder a un historial de datos de seis meses para responder preguntas como:

¿Qué ha pasado con este recurso o configuración y quién lo actualizó por última vez?

¿Qué ha estado haciendo el usuario X?

¿Quién está iniciando sesión en nuestra cuenta?

## Qué auditamos {#what-we-audit}

Marketo auditará las acciones de [creación, edición y eliminación](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) para:

* Diseñar recursos de estudio
* Todos los programas de marketing
* Campañas inteligentes
* Listas (inteligentes/estáticas)
* Usuarios (administrador)
* Funciones y permisos (administrador)
* Espacio de trabajo y particiones (administrador)
* Historial de inicio de sesión del usuario

>[!NOTE]
>
>Marketo **no audita** los cambios realizados en Personalización web, Contenido predictivo o Perspectiva de ventas en este momento.

## Componentes de pista de auditoría {#audit-trail-components}

La pista de auditoría consta de tres componentes.

**1) Pista de auditoría de [activos](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

Consulte actividad a recursos específicos.

**2) Seguimiento de auditoría [del administrador](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

Monitorear los detalles basados en el usuario.

**3) Historial [de inicio de sesión del usuario](http://docs.marketo.com/display/DOCS/User+Login+History)**

Ver quién ha estado iniciando sesión en tu suscripción y cuándo. También incluye los intentos fallidos de inicio de sesión.

>[!TIP]
>
>Hay tanto que puede auditar usando la pista de auditoría, ¡asegúrese de utilizar [el filtrado](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## Exportación de datos {#exporting-data}

Sólo puede vista de datos de 30 días en su instancia. Para obtener un valor de hasta seis meses, utilice la opción de exportación.

![](assets/two.png)

>[!NOTE]
>
>**Definición**
>
>**Desconocido:** En la pista de auditoría, puede ver el nombre y el correo electrónico de un usuario como &quot;Desconocido&quot;. Esto sucede cuando se realizan cambios en los valores de la lista de selección en el CRM. Estos valores aparecen en formularios y páginas de aterrizaje de marketing. Al realizar esta actualización en CRM, se borrarán automáticamente las páginas de aterrizaje que hagan referencia al formulario. En la pista de auditoría, capturaremos que la página de aterrizaje se ha redactado, pero el nombre y el correo electrónico del usuario se mostrarán como &quot;Desconocido&quot;, ya que no podemos capturar la información del usuario desde el lado de CRM.

>[!MORELIKETHIS]
>
>* [Habilitar pista de auditoría](enable-audit-trail.md)

>



