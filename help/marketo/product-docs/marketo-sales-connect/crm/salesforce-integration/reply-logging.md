---
unique-page-id: 14352480
description: 'Registro de respuestas (SFDC): documentos de Marketo, documentación del producto'
title: Registro de respuestas (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Registro de respuestas (SFDC) {#reply-logging-sfdc}

Sales Connect permite registrar automáticamente las respuestas de los posibles clientes en Salesforce. La estructura que le permite hacerlo se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un posible cliente, podemos registrar esa respuesta en Salesforce.

## Requisitos {#requirements}

* Debe registrar correos electrónicos mediante el registro de API
* Debe ser capaz de [seguimiento de una respuesta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Debe estar conectado con Salesforce
* Debe tener Salesforce [Llamadas de API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponible

## Habilitar registro de respuestas {#enable-reply-logging}

1. Para habilitar el registro de respuestas, puede ir a la página de configuración de Salesforce. Una vez desactivado el registro de la API, verá la opción para comprobar _Registrar respuestas_.

   >[!NOTE]
   >
   >El registro de respuestas sigue las mismas reglas que tiene para registrar los correos electrónicos enviados. Esto incluye cómo se registran los correos electrónicos, a posibles clientes y contactos, cuando hay un registro duplicado, si no se encuentran registros coincidentes.

## Configuración del tipo de respuesta en Salesforce {#setting-type-to-reply-in-salesforce}

Es importante obtener datos significativos de los informes de Salesforce. Tener la capacidad de que el campo Tipo se rellene como &quot;Respuesta&quot; le permite obtener esos datos en los informes. Asociarse con su `Salesforce admin` para obtener esta configuración.

1. Ir a **Configurar** > **Personalizar** > **Actividades** > **Campos de tarea**.
1. Clic **Tipo**.
1. En Valores de Lista de selección de tipo de tarea, haga clic en **Nuevo**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de poner en mayúscula la &quot;R&quot; y haga clic en **Guardar**.

   >[!NOTE]
   >
   >No es necesario seleccionar un valor por defecto en la lista de selección Tipo. Sales Connect comprobará que este tipo de actividad está disponible en la instancia de Salesforce y rellenará el campo de tarea de las actividades entrantes según corresponda.
