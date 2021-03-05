---
unique-page-id: 2953415
description: Uso de la página de detalles de la persona - Marketo Docs - Documentación del producto
title: Uso de la página de detalles de persona
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---


# Uso de la página de detalles de persona {#using-the-person-detail-page}

La página de detalles de la persona contiene toda la información que Marketo conoce sobre una persona. Los datos se pueden editar directamente desde esta página.

## Acceder a la página de detalles de persona {#getting-to-person-detail-page}

Hay muchas maneras de abrir personas específicas. Algunos ejemplos son:

* Desde **Database**, puede buscar en la Búsqueda rápida
* Cualquier **lista** o lista inteligente
* **** Membresía de un programa
* **Visualización de** miembros de Campaign en una campaña inteligente
* Algunos **informes**

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
| Campos personalizados de Microsoft | Campos personalizados de Microsoft. |
| Campo de posible cliente de Microsoft | Campos integrados de Microsoft. |
| Registro de actividades | Todas las actividades relacionadas con la persona. |

>[!NOTE]
>
>También puede ver la información de oportunidad [insertada a través de la API](http://developers.marketo.com/rest-api/lead-database/opportunities/) para instancias que no están sincronizadas con un CRM.

## Edición de un campo {#editing-a-field}

Muchos campos son editables. Para actualizar la información de una persona, escriba un valor nuevo y haga clic fuera del campo para guardar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo Campos predeterminados antes de la sincronización con CRM {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Dirección | Ingresos anuales | IP anónima | Dirección de facturación | Ciudad de facturación |
| País de facturación | Código postal de facturación | Estado de facturación | Ciudad | Nombre de la empresa |
| País | Creado en | Fecha de nacimiento | Departamento | No llamar |
| No llamar a causa | Motivo de no llamada | Dirección de correo electrónico | Correo electrónico no válido | Causa no válida de correo electrónico |
| Id. de compañía externa | Id. de persona de ventas externas | Número de fax | Nombre | Nombre completo |
| Industria | Ciudad vinculada | Empresa vinculada | País afectado | Área metropolitana vinculada |
| Código de área de teléfono insertado | Código postal adjunto | Región Estado Inferior | Is Anonymous | Is Customer |
| Es socio | Puesto de trabajo | Apellidos | Clasificación | Puntuación |
| Fuente de persona | Estado | Teléfono principal | Marketo Social Nombre para mostrar de Facebook | Marketo Social Facebook Id |
| Marketo Social Photo URL | URL del perfil de Facebook de Marketo Social | Alcance de Marketo Social Facebook | Marketo Social Facebook Inscripciones referidas | Visitas referidas a Marketo Social Facebook |
| Género de Marketo Social | Marketo Social Última Inscripción Remitida | Marketo Social Última visita referida | Nombre para mostrar de Marketo Social LinkedIn | Marketo Social LinkedIn Id |
| URL de foto de Marketo Social LinkedIn | URL del perfil de Marketo Social LinkedIn | Alcance de Marketo Social LinkedIn | Marketo Social LinkedIn Menciona inscripciones | Marketo Social LinkedIn Visitas referidas |
| ID de distribución social de Marketo | Marketo Social Total de inscripciones referidas | Visitas de referencia totales de Marketo Social | Marketo Social Twitter Display Name | Marketo Social Twitter Id |
| Marketo Social Twitter Photo URL | URL del perfil de Twitter de Marketo Social | Alcance de Marketo Social Twitter | Marketo Social Twitter: inscripciones referidas | Visitas referidas a Marketo Social Twitter |
| Segundo nombre | Número de teléfono móvil | Número de empleados | Número de teléfono | Código postal |
| Prioridad | Puntuación relativa | Función | Saludo | Código SIC |
| Sitio | Estado | Cancelación de suscripción | Motivo de cancelación de suscripción | Actualizado en |
| Urgencia | Sitio web |  |  |  |

>[!NOTE]
>
>Algunos campos son _no_ editables:
>
>* Registro de actividades
>* Información de la empresa
>* Oportunidades para los contactos de SFDC
>* Ciertos campos específicos de Marketo, como Fecha de creación y Tipo de origen original.

>
>
Obtenga más información sobre [Campos administrados por el sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Creación de una ficha personalizada para la página de detalles de la persona](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
