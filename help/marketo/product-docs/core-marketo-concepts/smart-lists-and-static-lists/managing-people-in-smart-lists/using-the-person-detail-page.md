---
unique-page-id: 2953415
description: Uso de la página de detalles de persona - Documentos de Marketo - Documentación del producto
title: Uso de la página Detalles de Persona
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 50%

---

# Uso de la página Detalles de Persona {#using-the-person-detail-page}

La página de detalles de la persona contiene toda la información que Marketo conoce sobre una persona. Puede editar los datos directamente desde esta página.

## Cómo llegar a la página Detalles de Persona {#getting-to-person-detail-page}

Hay muchas maneras de abrir a personas específicas. Algunos ejemplos son:

* Desde la **base de datos**, puede buscar en Búsqueda rápida
* Cualquier **lista inteligente** o lista
* Pestaña **Miembros** de un programa
* **Ver miembros de campaña** en una campaña inteligente
* Algunos **informes**
  <br> 

1. Haga doble clic en cualquier persona o haga clic en el ID a la izquierda.

   ![](assets/one-1.png)

1. Se abrirá la pantalla de detalles de la persona.

   ![](assets/two-5.png)

## Organización de la página - Salesforce {#page-organization-salesforce}

La información de la persona se clasifica en las siguientes pestañas:

| Ficha | Descripción |
|---|---|
| Información | Información de contacto y campos personalizados sobre una persona. |
| Información de la compañía | Información y dirección de la empresa de la persona. |
| Información de oportunidad | Información de oportunidad sincronizada desde Salesforce. |
| Campo de lead de SFDC | Campos integrados de Salesforce. |
| Campo personalizado de SFDC | Campos personalizados de Salesforce. |
| Registro de actividades | Todas las actividades relacionadas con la persona. |

## Organización de la página - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Ficha | Descripción |
|---|---|
| Información | Información de contacto y campos personalizados sobre una persona. |
| Información de la compañía | Información y dirección de la empresa de la persona. |
| Información de oportunidad | Información de oportunidad sincronizada desde Microsoft. |
| Campos personalizados de Microsoft | Campos personalizados de Microsoft. |
| Campo de leads de Microsoft | Campos integrados de Microsoft. |
| Registro de actividades | Todas las actividades relacionadas con la persona. |

>[!NOTE]
>
>También puede ver la información de oportunidad [insertada a través de la API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities) para instancias que no están sincronizadas con un CRM.

## Edición de un campo {#editing-a-field}

Muchos campos son editables. Para actualizar la información de una persona, escriba un nuevo valor y haga clic fuera del campo para guardar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campos predeterminados de Marketo anteriores a la sincronización de CRM {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Dirección | Ingresos anuales | IP anónima | Dirección de facturación | Ciudad de facturación |
| País de facturación | Código postal de facturación | Estado de facturación | Ciudad | Nombre de la empresa |
| País | Creado en | Fecha de nacimiento | Departamento | No llamar |
| Causa por la que no se debe llamar | Razón por la que no se debe llamar | Correo electrónico | Email no válido | Causa de email no válido |
| Identificación de compañía externa | Identificación de persona de ventas externa | Número de fax | Nombre | Nombre completo |
| Industria | Ciudad inferida | Compañía inferida | País inferido | Área metropolitana inferida |
| Código de área telefónico inferido | Código postal inferido | Región del estado inferida | Es anónimo | Es cliente |
| Es socio | Cargo | Apellido | Calificación | Puntaje |
| Origen de la persona | Estado | Teléfono principal: | Nombre de Marketo Social para mostrar en Facebook | Identificación de Marketo Social en Facebook |
| URL de imagen de Marketo Social para Facebook | URL de perfil de Marketo Social en Facebook | Alcance de Marketo Social en Facebook | Ins. ref. desde Facebook de Marketo Social | Visitas referidas desde Facebook de Marketo Social |
| Sexo de Marketo Social | Última inscripción referida desde Marketo Social | Última visita referida desde  Marketo Social | Nombre de Marketo Social para mostrar en LinkedIn | Identificación de Marketo Social en LinkedIn |
| URL de imagen de Marketo Social para LinkedIn | URL de perfil de Marketo Social en LinkedIn | Alcance de Marketo Social en LinkedIn | Ins. ref. desde  LinkedIn de Marketo Social | Visitas referidas desde LinkedIn de Marketo Social |
| Identificación de distribución de Marketo Social | Inscripciones referidas totales de Marketo Social | Visitas referidas totales de Marketo Social | Nombre de Marketo Social para mostrar en Twitter | Identificación de Marketo Social en Twitter |
| URL de imagen de Marketo Social para Twitter | URL de perfil de Marketo Social en Twitter | Alcance de Marketo Social en Twitter | Ins. ref. desde Twitter de Marketo Social | Visitas referidas desde Twitter de Marketo Social |
| Segundo nombre | Número de teléfono móvil | Cantidad de empleados | Número de teléfono | Código postal |
| Prioridad | Puntaje relativo | Función | Saludo | Código SIC |
| Sitio | Estado | Suscripción cancelada | Razón de la cancelación de la suscripción | Actualizado en |
| Urgencia | Sitio web |  |  |  |

>[!NOTE]
>
>Algunos campos _no_ son editables:
>
>* Registro de actividades
>* Información de empresa
>* Oportunidades para contactos de SFDC
>* Algunos campos específicos de Marketo, como Fecha de creación y Tipo de Source original.
>
>Más información sobre [Campos administrados por el sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Creando una ficha personalizada para la página de detalles de persona](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
