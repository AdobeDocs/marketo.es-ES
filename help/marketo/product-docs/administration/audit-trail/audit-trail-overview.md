---
unique-page-id: 11377945
description: Información general sobre la pista de auditoría y cómo captura un historial de seis meses de cambios y actividad de inicio de sesión en la instancia de Marketo.
title: Información general de seguimiento de auditoría
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 759f14f3913491d95e637e0d80217720beda55b1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 2%

---

# Información general de seguimiento de auditoría {#audit-trail-overview}

La pista de auditoría le permite obtener un historial completo (seis meses) de los cambios realizados en la instancia de Marketo.

>[!NOTE]
>
>El historial de datos de pista de auditoría comenzó el 14 de septiembre de 2016.

![](assets/audit-trail-overview-1.png)

## Qué es la pista de auditoría {#what-is-audit-trail}

La pista de auditoría captura, en tiempo real, una lista completa de las acciones y eventos que se producen dentro de una suscripción de Marketo. Incluye una forma de autoservicio de acceder a un historial de datos de seis meses para responder preguntas como las siguientes:

&quot;¿Qué ha pasado con este recurso o configuración y quién lo actualizó por última vez?&quot;

&quot;¿Qué ha estado haciendo el usuario X?&quot;

&quot;¿Quién inicia sesión en nuestra cuenta?&quot;

## Qué auditamos {#what-we-audit}

Marketo audita las acciones [crear, editar y eliminar](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

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

Ver quién ha iniciado sesión en su suscripción y cuándo (también incluye intentos de inicio de sesión fallidos).

>[!TIP]
>
>Dado que hay muchas cosas que puedes auditar usando la pista de auditoría, [filtrar](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) puede ahorrar mucho tiempo.

## Exportando datos {#exporting-data}

Solo puede ver datos de 30 días en su instancia. Para obtener (hasta) seis meses, utilice la opción de exportación.

![](assets/two.png)

>[!NOTE]
>
>**Definición**
>
>**Desconocido:** En [!DNL Webhook], es posible que vea el nombre y el correo electrónico de un usuario como &quot;Desconocido&quot;. Esto sucede cuando realiza un cambio en los valores de la lista de selección en su CRM. Estos valores aparecen en formularios Marketo y páginas de aterrizaje. Al realizar esta actualización en CRM, se realizará un borrador automático de las páginas de aterrizaje que hagan referencia al formulario. En [!DNL Webhook], Marketo captura que la página de aterrizaje se redactó, pero el nombre y el correo electrónico del usuario se mostrarán como &quot;Desconocido&quot;, ya que Marketo no puede capturar la información del usuario desde CRM.

>[!MORELIKETHIS]
>
>[Habilitar pista de auditoría](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
