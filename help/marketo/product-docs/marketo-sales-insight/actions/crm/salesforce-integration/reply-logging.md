---
description: 'Registro de respuestas: documentos de Marketo, documentación del producto'
title: Registro de respuestas
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Registro de respuestas {#reply-logging}

Las acciones de ventas de Insight le permiten registrar automáticamente las respuestas de sus posibles clientes a [!DNL Salesforce]. La estructura que le permite hacerlo se basa en nuestro seguimiento de respuestas por correo electrónico. Si podemos rastrear la respuesta de un posible cliente, podemos registrar esa respuesta en [!DNL Salesforce].

## Requisitos {#requirements}

* Debe registrar correos electrónicos mediante el registro de API
* Debe poder [rastrear una respuesta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
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
1. En [!UICONTROL Valores de lista de selección de tipo de tarea], haga clic en **[!UICONTROL Nuevo]**.
1. Escriba &quot;Responder&quot; en el cuadro vacío. Asegúrese de poner en mayúscula la &quot;R&quot; y hacer clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >No es necesario seleccionar un valor por defecto en la lista de selección Tipo. [!DNL Sales Insight Actions] verá que este tipo de actividad está disponible en su instancia de [!DNL Salesforce] y rellenará el campo de tarea en las actividades entrantes según corresponda.
