---
unique-page-id: 14352480
description: Registro de respuestas (SFDC) - Documentos de marketing - Documentación del producto
title: Registro de respuesta (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Registro de respuesta (SFDC) {#reply-logging-sfdc}

Sales Connect le permite registrar automáticamente las respuestas de sus clientes potenciales en Salesforce. La estructura que le permite hacer esto se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un cliente potencial, podemos registrar esa respuesta en Salesforce.

## Requisitos {#requirements}

* Debe registrar correos electrónicos mediante el registro de API
* Debe poder [rastrear una respuesta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Debe estar conectado con Salesforce
* Debe tener disponibles las llamadas de API de Salesforce [](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)

## Habilitar registro de respuesta {#enable-reply-logging}

1. Para habilitar el registro de respuestas, puede dirigirse a la página de configuración de Salesforce. Una vez que el registro de la API esté desactivado, verá la opción de comprobar _Respuestas de registro_.

   >[!NOTE]
   >
   >El registro de respuestas sigue las mismas reglas que tiene establecidas para el registro de correos electrónicos enviados. Esto incluye cómo se registran los correos electrónicos; a posibles clientes y contactos; cuando haya un registro de duplicados; si no se encuentran registros coincidentes.

## Configuración del tipo para responder en Salesforce {#setting-type-to-reply-in-salesforce}

Es importante obtener datos significativos de los informes de Salesforce. Tener la capacidad de rellenar el campo Tipo como &#39;Respuesta&#39; le permite obtener esos datos en los informes. Asocie con su `Salesforce admin` para obtener esta configuración.

1. Vaya a **Configuración** > **Personalizar** > **Actividades** > **Campos de Tarea**.
1. Haga clic en **Tipo**.
1. En Tipo de Tarea Valores de lista de , haga clic en **Nuevo**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de que pone en mayúscula la &#39;R&#39; y haga clic en **Guardar**.

   >[!NOTE]
   >
   >No es necesario que seleccione un valor predeterminado en la lista de selección Tipo. Sales Connect comprobará que este tipo de Actividad está disponible en la instancia de Salesforce y rellenará el campo de tarea de las actividades entrantes en consecuencia.
