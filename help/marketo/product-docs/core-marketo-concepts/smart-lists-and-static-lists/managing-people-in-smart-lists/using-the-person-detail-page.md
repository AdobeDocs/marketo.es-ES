---
unique-page-id: 2953415
description: 'Uso de la página de detalles de la persona: Marketo Docs: documentación del producto'
title: Uso de la página de detalles de persona
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 44%

---

# Uso de la página de detalles de persona {#using-the-person-detail-page}

La página de detalles de la persona contiene toda la información que Marketo conoce sobre una persona. Los datos se pueden editar directamente desde esta página.

## Página de detalles de persona {#getting-to-person-detail-page}

Hay muchas maneras de abrir personas específicas. Algunos ejemplos son:

* En el **Base de datos**, puede buscar en Búsqueda rápida
* Cualquier elemento inteligente **list** o lista
* **Miembros** pestaña de un programa
* **Ver miembros de campaña** en una campaña inteligente
* Algunas **informes**

   <br> 

1. Haga doble clic en cualquier persona o haga clic en el ID de la izquierda.

   ![](assets/one-1.png)

1. Se abrirá la pantalla de detalles de la persona.

   ![](assets/two-5.png)

## Organización de páginas - Salesforce {#page-organization-salesforce}

La información de la persona se clasifica en las siguientes pestañas:

| Tabulación | Descripción |
|---|---|
| Información | Información de contacto y campos personalizados sobre una persona. |
| Información de la empresa | Información y dirección de la empresa de la persona. |
| Información de oportunidad | Información de oportunidad sincronizada desde Salesforce. |
| Campo de posible cliente de SFDC | Campos integrados de Salesforce. |
| Campo personalizado SFDC | Campos de Salesforce personalizados. |
| Registro de actividades | Todas las actividades relacionadas con la persona. |

## Organización de páginas - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabulación | Descripción |
|---|---|
| Información | Información de contacto y campos personalizados sobre una persona. |
| Información de la empresa | Información y dirección de la empresa de la persona. |
| Información de oportunidad | Información de oportunidad sincronizada desde Microsoft. |
| Campos personalizados de Microsoft | Campos personalizados de Microsoft . |
| Campo de posible cliente de Microsoft | Campos integrados de Microsoft. |
| Registro de actividades | Todas las actividades relacionadas con la persona. |

>[!NOTE]
>
>También puede ver la información de oportunidad [insertado mediante API](https://developers.marketo.com/rest-api/lead-database/opportunities/) para instancias que no se sincronizan con un CRM.

## Edición de campos {#editing-a-field}

Muchos campos son editables. Para actualizar la información de una persona, escriba un valor nuevo y haga clic fuera del campo para guardar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campos predeterminados de Marketo antes de la sincronización con CRM {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Dirección | Ingresos anuales | IP anónima | Dirección de facturación | Ciudad de facturación |
| País de facturación | Código postal de facturación | Estado de facturación | Ciudad | Nombre de la compañía |
| País | Creado en | Fecha de nacimiento | Departamento | No llamar |
| Causa por la que no se debe llamar | Razón por la que no se debe llamar | Dirección de email | Email no válido | Causa de email no válido |
| Identificación de compañía externa | Identificación de persona de ventas externa | Número de fax | Nombre | Nombre completo |
| Industria | Ciudad inferida | Compañía inferida | País inferido | Área metropolitana inferida |
| Código de área telefónico inferido | Código postal inferido | Región del estado inferida | Es anónimo | Es cliente |
| Es socio | Cargo | Apellido | Calificación | Puntuación |
| Origen de la persona | Estado | Teléfono principal | Nombre de Marketo Social para mostrar en Facebook | Identificación de Marketo Social en Facebook |
| URL de imagen de Marketo Social para Facebook | URL de perfil de Marketo Social en Facebook | Alcance de Marketo Social en Facebook | Inscripciones referidas desde Facebook de Marketo Social | Visitas referidas desde Facebook de Marketo Social |
| Sexo de Marketo Social | Última inscripción referida desde Facebook de Marketo Social | Última visita referida desde Facebook de Marketo Social | Nombre de Marketo Social para mostrar en LinkedIn | Identificación de Marketo Social en LinkedIn |
| URL de imagen de Marketo Social para LinkedIn | URL de perfil de Marketo Social en LinkedIn | Alcance de Marketo Social en LinkedIn | Inscripciones referidas desde LinkedIn de Marketo Social | Visitas referidas desde LinkedIn de Marketo Social |
| Marketo Social Syndication ID | Inscripciones referidas totales de Marketo Social | Visitas referidas totales de Marketo Social | Nombre de Marketo Social para mostrar en Twitter | Identificación de Marketo Social en Twitter |
| URL de imagen de Marketo Social para Twitter | URL de perfil de Marketo Social en Twitter | Alcance de Marketo Social en Twitter | Inscripciones referidas desde Twitter de Marketo Social | Visitas referidas desde Twitter de Marketo Social |
| Segundo nombre | Número de teléfono móvil | Cantidad de empleados | Número de teléfono | Código postal |
| Prioridad | Puntaje relativo | Rol | Saludo | Código SIC |
| Sitio | Estado | Suscripción cancelada | Razón de la cancelación de la suscripción | Actualizado en |
| Urgencia | Sitio web |  |  |  |

>[!NOTE]
>
>Algunos campos son _not_ editable:
>
>* Registro de actividades
>* Información de la empresa
>* Oportunidades para los contactos de SFDC
>* Ciertos campos específicos de Marketo, como Fecha de creación y Tipo de origen original.
>
>Más información sobre [Campos administrados por el sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Creación de una ficha personalizada para la página de detalles de la persona](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
