---
unique-page-id: 37356194
description: Exportación de una Lista estática a Adobe Experience Cloud - Documentos de marketing - Documentación del producto
title: Exportación de una Lista estática a Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---


# Exportación de una Lista estática a Adobe Experience Cloud {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Una implementación preparada para HIPAA de una instancia de Marketing no puede utilizar esta función.

>[!NOTE]
>
>**Requisitos previos**
>
>[Configurar el uso compartido de Audiencias de Adobe Experience Cloud](http://docs.marketo.com/x/D4GMAg)

## Aplicaciones de destino admitidas {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (**solo** si posee una licencia de Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Plataforma de datos de clientes en tiempo real de Adobe
* Adobe Target

## Cómo exportar una Lista {#how-to-export-a-list}

1. En Marketing, busque y seleccione la lista que desee exportar.

   ![](assets/one.png)

1. Haga clic en la lista desplegable Acciones **de** Lista y seleccione **Enviar al Experience Cloud**.

   ![](assets/two-1.png)

1. Haga clic en la lista desplegable Carpeta **del** Audience Manager y seleccione la carpeta de destino que desee en el Experience Cloud.

   ![](assets/three-1.png)

1. Elija si desea crear una nueva audiencia o sobrescribir una existente (en este ejemplo estamos creando una nueva). Introduzca el nuevo nombre de audiencia y haga clic en **Enviar**.

   ![](assets/four.png)

1. Haga clic en **Aceptar**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Puede tomar hasta 6-8 horas para que la membresía en la audiencia se complete en Adobe.

## Aspectos a tener en cuenta {#things-to-note}

**Compartir con Adobe Analytics**

Para los clientes que son propietarios de Adobe Audience Manager y Adobe Analytics, esta integración permitirá que las audiencias se compartan desde Marketing a sus grupos de informes de Adobe Analytics; sin embargo, hay que realizar algunos pasos de configuración adicionales en Adobe Audience Manager para habilitarlos. Consulte la documentación de Adobe Audience Manager para obtener más información sobre cómo configurarla: [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](http://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Uso de características para clientes de Adobe Audience Manager**

Al iniciar una exportación de listas en Marketing, verá los siguientes cambios reflejados en la instancia de Adobe Audience Manager:

* Para todos los posibles clientes de la Lista exportada, Marketing escribirá una característica utilizando los correos electrónicos con hash de los posibles clientes como un identificador entre dispositivos. El nombre de la característica coincidirá con el nombre de la Audiencia de destino que especificó durante la exportación.
* Para todos los ECID que Marketing ha logrado coincidir con los leads de la Lista exportada, Marketo escribirá una característica utilizando el identificador de dispositivo ECID. El nombre de la característica coincidirá con el nombre de la Audiencia de destino que especificó durante la exportación.
* Marketo también creará un segmento en la instancia de Audience Manager utilizando la característica ECID como único criterio de segmentación. El nombre del segmento coincidirá con el nombre de la Audiencia de destino que especificó durante la exportación.

## Preguntas más frecuentes {#faq}

**¿Por qué el tamaño de la lista en Marketing es diferente al del Adobe?**

En el capó, la integración de audiencias funciona sincronizando las cookies de Marketing Munchkin con la cookie ECID de Adobe correspondiente. Marketo solo puede compartir datos de pertenencia para leads para los que Marketing haya sincronizado un ECID. Para obtener los mejores resultados posibles, se recomienda cargar el script de seguimiento munchkin.js de Marketing en paralelo con el código de seguimiento visitante.js de Adobe en todas las páginas que le interesen rastrear con fines de mercadotecnia.

**¿Cómo funciona la sincronización de cookies?**

Cuando la sincronización de cookies está habilitada para su Suscripción de Marketing, el archivo munchkin.js de Marketing intentará capturar y almacenar los ECID de Adobe para la organización de IMS de Adobe que especificó durante la configuración de la integración y hacer coincidir estos ECID con el identificador de cookie de marketing correspondiente. Esto permite a los perfiles de usuarios anónimos de Marketing enriquecer los ECID de Adobe.

Se requiere un paso más para asociar el perfil de usuario anónimo a un Perfil de posibles clientes, que se identifica mediante un correo electrónico de texto sin formato. Exactamente cómo funciona esto aquí: [https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](http://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People).
