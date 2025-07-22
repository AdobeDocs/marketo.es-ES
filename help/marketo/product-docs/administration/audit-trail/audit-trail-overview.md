---
unique-page-id: 11377945
description: Pista de auditoría&rbrack; Información general - Documentos de Marketo - Documentación del producto
title: Resumen de pista de auditoría
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Resumen de pista de auditoría {#audit-trail-overview}

La pista de auditoría le permite obtener un historial completo (seis meses) de los cambios realizados en la instancia de Marketo.

>[!NOTE]
>
>El historial de datos de pista de auditoría comenzó el 14 de septiembre de 2016.

![](assets/audit-trail-overview-1.png)

## Qué es la pista de auditoría {#what-is-audit-trail}

La pista de auditoría captura, en tiempo real, una lista completa de las acciones y eventos que se producen dentro de una suscripción de Marketo. Incluye una forma de autoservicio de acceder a un historial de datos de seis meses para responder preguntas como las siguientes:

¿Qué ha pasado con este recurso o configuración y quién lo actualizó por última vez?

¿Qué ha estado haciendo el usuario X?

¿Quién inicia sesión en nuestra cuenta?

## Qué auditamos {#what-we-audit}

Marketo auditará las acciones [crear, editar y eliminar](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

* Recursos de Design Studio
* Todos los programas de Marketo
* Campañas inteligentes
* Listas (inteligentes/estáticas)
* Usuarios (administrador)
* Funciones y permisos (administrador)
* Workspace y particiones (administrador)
* Historial de inicio de sesión del usuario

>[!NOTE]
>
>Marketo _no_ está auditando los cambios realizados en Web Personalization, Predictive Content o Sales Insight en este momento.

## Componentes de pista de auditoría {#audit-trail-components}

La pista de auditoría consta de tres componentes.

**1) [Registro de auditoría de recursos](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulte la actividad realizada en recursos específicos.

**2) [Registro de auditoría de administración](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitorice los detalles basados en el usuario.

**3) [Historial de inicio de sesión de usuario](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Ver quién ha iniciado sesión en su suscripción y cuándo. También incluye los intentos de inicio de sesión erróneos.

>[!TIP]
>
>Es mucho lo que puede auditar con la pista de auditoría. ¡Asegúrese de usar [Filtrado](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Exportando datos {#exporting-data}

Solo puede ver datos de 30 días en su instancia. Para obtener (hasta) seis meses, utilice la opción de exportación.

![](assets/two.png)

>[!NOTE]
>
>**Definición**
>
>**Desconocido:** En [!DNL Webhook], es posible que vea el nombre y el correo electrónico de un usuario como &quot;Desconocido&quot;. Esto sucede cuando realiza un cambio en los valores de la lista de selección en su CRM. Estos valores aparecen en formularios Marketo y páginas de aterrizaje. Al realizar esta actualización en CRM, se realizará un borrador automático de las páginas de aterrizaje que hagan referencia al formulario. En [!DNL Webhook], capturaremos que la página de aterrizaje se redactó, pero el nombre y el correo electrónico del usuario se mostrarán como &quot;Desconocido&quot;, ya que no podemos capturar la información del usuario desde CRM.

>[!MORELIKETHIS]
>
>[Habilitar pista de auditoría](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
