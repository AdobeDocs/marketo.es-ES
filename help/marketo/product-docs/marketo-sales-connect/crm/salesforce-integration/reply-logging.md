---
unique-page-id: 14352480
description: 'Registro de respuestas (SFDC): documentos de Marketo, documentación del producto'
title: Registro de respuestas (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Registro de respuestas (SFDC) {#reply-logging-sfdc}

Sales Connect le ofrece la posibilidad de registrar automáticamente las respuestas de sus posibles clientes en Salesforce. La estructura que le permite hacerlo se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un posible cliente, podemos registrar esa respuesta en Salesforce.

## Requisitos {#requirements}

* Debe registrar correos electrónicos mediante el registro de API
* Debe poder [rastrear una respuesta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Debe estar conectado con [!DNL Salesforce]
* Debe tener [!DNL Salesforce] [llamadas a la API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm?lang=es) disponibles

## Habilitar registro de respuestas {#enable-reply-logging}

1. Para habilitar el registro de respuestas, puede ir a la página de configuración de [!DNL Salesforce]. Una vez que el registro de API esté desactivado, verá la opción de comprobar _Respuestas al registro_.

   >[!NOTE]
   >
   >El registro de respuestas sigue las mismas reglas que tiene para registrar los correos electrónicos enviados. Esto incluye cómo se registran los correos electrónicos, a posibles clientes y contactos, cuando hay un registro duplicado, si no se encuentran registros coincidentes.

## Estableciendo tipo para responder en [!DNL Salesforce] {#setting-type-to-reply-in-salesforce}

Es importante obtener datos significativos de los informes de [!DNL Salesforce]. Tener la capacidad de que el campo Tipo se rellene como &quot;Respuesta&quot; le permite obtener esos datos en los informes. Asociarse con su `[!DNL Salesforce] admin` para obtener esta configuración.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Personalizar]** > **[!UICONTROL Actividades]** > **[!UICONTROL Campos de tarea]**.
1. Haga clic en **[!UICONTROL Tipo]**.
1. En Valores de lista de selección de tipo de tarea, haga clic en **[!UICONTROL Nuevo]**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de poner en mayúscula la &quot;R&quot; y hacer clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >No es necesario seleccionar un valor por defecto en la lista de selección Tipo. [!DNL Sales Connect] verá que este tipo de actividad está disponible en su instancia de [!DNL Salesforce] y rellenará el campo de tarea en las actividades entrantes según corresponda.
