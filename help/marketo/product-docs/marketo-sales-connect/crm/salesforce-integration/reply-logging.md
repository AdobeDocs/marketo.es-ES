---
unique-page-id: 14352480
description: Registro de respuestas (SFDC) - Documentos de marketing - Documentación del producto
title: Registro de respuesta (SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Registro de respuesta (SFDC) {#reply-logging-sfdc}

Sales Connect le permite registrar automáticamente las respuestas de sus clientes potenciales en Salesforce. La estructura que le permite hacer esto se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un cliente potencial, podemos registrar esa respuesta en Salesforce.

## Requisitos {#requirements}

* Debe registrar correos electrónicos mediante el registro de API
* Debe poder [rastrear una respuesta](http://docs.marketo.com/x/BYPS)
* Debe estar conectado con Salesforce
* Debe tener disponibles las llamadas [de](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) API de Salesforce

## Habilitar registro de respuesta {#enable-reply-logging}

1. Para habilitar el registro de respuestas, puede dirigirse a la página de configuración [de](http://docs.marketo.com/pages/assets/external-link.jspa) Salesforce. Una vez que el registro de la API se haya desmarcado, verá la opción de comprobar *Respuestas de registro.\
   *

   >[!NOTE]
   >
   >El registro de respuestas sigue las mismas reglas que tiene establecidas para el registro de correos electrónicos enviados. Esto incluye cómo se registran los correos electrónicos; a posibles clientes y contactos; cuando haya un registro de duplicados; si no se encuentran registros coincidentes.

## Configuración del tipo para responder en Salesforce {#setting-type-to-reply-in-salesforce}

Es importante obtener datos significativos de los informes de Salesforce. Tener la capacidad de rellenar el campo Tipo como &#39;Respuesta&#39; le permite obtener esos datos en los informes. Asociarse con su `Salesforce admin` equipo para obtener esta configuración.

1. Vaya a **Configuración **> **Personalizar **> **Actividades **> Campos **** de Tarea.
1. Haga clic en **Tipo**.
1. En Tipo de Tarea Valores de lista de selección, haga clic en **Nuevo**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de que pone en mayúscula la &#39;R&#39; y haga clic en **Guardar**.

   >[!NOTE]
   >
   >No es necesario que seleccione un valor predeterminado en la lista de selección Tipo. Sales Connect comprobará que este tipo de Actividad está disponible en la instancia de Salesforce y rellenará el campo de tarea de las actividades entrantes en consecuencia.

