---
description: Registro de respuestas - Documentos de Marketo - Documentación del producto
title: Registro de respuestas
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Registro de respuestas {#reply-logging}

Las acciones de perspectiva de ventas le permiten registrar automáticamente las respuestas de sus posibles clientes a Salesforce. La estructura que le permite hacerlo se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un cliente potencial, podemos registrar esa respuesta en Salesforce.

## Requisitos {#requirements}

* Debe registrar los correos electrónicos mediante el registro de API
* Debe poder [seguimiento de una respuesta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Debe estar conectado con Salesforce
* Debe tener Salesforce [Llamadas de API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) available

## Habilitar el registro de respuestas {#enable-reply-logging}

1. Para habilitar el registro de respuestas, puede acceder a la página de configuración de Salesforce. Una vez que el registro de API esté desactivado, verá la opción de comprobar _Respuestas de registro_.

   >[!NOTE]
   >
   >El registro de respuestas sigue las mismas reglas que se aplican para registrar los correos electrónicos enviados. Esto incluye cómo se registran los correos electrónicos; a posibles clientes y contactos; cuando haya un registro duplicado; si no se encuentran registros coincidentes.

## Configuración del tipo para responder en Salesforce {#setting-type-to-reply-in-salesforce}

Es importante obtener datos significativos de los informes de Salesforce. Tener la capacidad de rellenar el campo Tipo como &quot;Respuesta&quot; le permite obtener esos datos en los informes. Asociarse con su `Salesforce admin` para obtener esta configuración.

1. Vaya a **Configuración** > **Personalizar** > **Actividades** > **Campos de tareas**.
1. Haga clic en **Tipo**.
1. En Valores de lista de selección de tipo de tarea, haga clic en **Nuevo**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de poner en mayúsculas la &quot;R&quot; y haga clic en **Guardar**.

   >[!NOTE]
   >
   >No es necesario que seleccione un Predeterminado en la lista de selección Tipo. Las acciones de perspectiva de ventas verán que este tipo de actividad está disponible en la instancia de Salesforce y rellenarán el campo de tareas en las actividades entrantes en consecuencia.
