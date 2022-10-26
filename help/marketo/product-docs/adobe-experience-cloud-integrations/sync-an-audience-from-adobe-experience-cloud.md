---
description: 'Sincronización de una audiencia desde Adobe Experience Cloud: Marketo Docs: Documentación del producto'
title: Sincronizar una audiencia desde Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: c396c205d3cececc752f9b563c0d2ab41ff92b6a
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Sincronizar una audiencia desde Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Una implementación lista para HIPAA de una instancia de Marketo no puede utilizar esta integración.

>[!PREREQUISITES]
>
>[Configuración de la asignación de organización de Adobe](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-organization-mapping.md)

## Sincronización de una audiencia {#how-to-sync-an-audience}

1. En Mi Marketo, haga clic en el botón **Base de datos** mosaico.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Haga clic en el **Nuevo** y seleccione **Sincronización desde la audiencia de Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Haga clic en el **Carpeta de la biblioteca de audiencias** y seleccione la carpeta de origen que desee.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Seleccione un **Nombre de audiencia**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Para el destino, puede seleccionar una lista existente o escribir el nombre de una nueva. En este ejemplo estamos creando uno nuevo. Haga clic en **Sincronización** cuando haya terminado.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Haga clic en **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Preguntas frecuentes {#faq}

**¿Cómo funciona la sincronización de cookies?**

Cuando la sincronización de cookies esté habilitada para su suscripción a Marketo, munchkin.js de Marketo intentará capturar y almacenar los ECID de Adobe para la organización de IMS de Adobe que especificó durante la configuración de la integración y hacer coincidir estos ECID con el identificador de cookie de Marketo correspondiente. Esto permite que los perfiles de usuario anónimos de Marketo se enriquezcan con los ECID de Adobe.

Se requiere un paso más para asociar el perfil de usuario anónimo a un perfil de posible cliente, que se identifica mediante un correo electrónico de texto sin formato. Exactamente cómo funciona esto [se describe aquí](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**¿Por qué el tamaño de la lista en Marketo es diferente del de la lista en Adobe?**

Una persona tampoco se sincronizará si no podemos vincular un ID de cookie de ECID a una persona conocida en Marketo.

**¿Se trata de una sincronización única?**

Solo es necesario iniciar la sincronización una vez. Después, los registros se sincronizarán automáticamente. La sincronización inicial puede tardar hasta 24 horas; en adelante, los registros nuevos se sincronizarán en 2-3 horas.
