---
unique-page-id: 37356194
description: 'Envío de una lista a Adobe Experience Cloud: documentos de Marketo, documentación del producto'
title: Enviar una lista a Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 3%

---

# Enviar una lista a Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Una implementación compatible con HIPAA de una instancia de Marketo Engage no puede utilizar esta función.

>[!PREREQUISITES]
>
>[Configurar la asignación de organización de Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Aplicaciones de destino admitidas {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_solo_ si posee una licencia de Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-Time Customer Data Platform
* Adobe Target

## Cómo enviar una lista estática {#how-to-send-a-static-list}

Una lista estática es sólo eso, estática. No se producirán cambios en la lista de Adobe Experience Cloud a menos que los realice manualmente.

1. En Marketo, busque la lista que desee exportar. Haga clic con el botón derecho en él y seleccione **[!UICONTROL Enviar a Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Haga clic en la lista desplegable **[!UICONTROL Carpeta de Audience Manager]** y seleccione la carpeta de destino que desee en Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Elija si desea crear una audiencia nueva o sobrescribir una existente (en este ejemplo creamos una nueva). Escriba el nuevo nombre de audiencia y haga clic en **[!UICONTROL Enviar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >La pertenencia a audiencias puede tardar entre 6 y 8 horas en rellenarse completamente en Adobe.

## Cómo enviar una lista sincronizada {#how-to-send-a-synced-list}

Sincronizar una lista significa que, cada vez que actualice una lista en Marketo, ese cambio se sincroniza automáticamente con su audiencia en Adobe Experience Cloud.

1. En Marketo, busque la lista que desee exportar. Haga clic con el botón derecho en él y seleccione **[!UICONTROL Enviar a Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Haga clic en la lista desplegable **[!UICONTROL Carpeta de biblioteca de audiencias]** y seleccione la carpeta de destino que desee en Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Elija si desea crear una audiencia nueva o sobrescribir una existente (en este ejemplo creamos una nueva). Escriba el nuevo nombre de audiencia, marque la casilla **[!UICONTROL Mantener pertenencia a audiencia sincronizada]** y haga clic en **[!UICONTROL Enviar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Cómo detener una sincronización de lista {#how-to-stop-a-list-sync}

Puede detener la sincronización de la lista en cualquier momento.

1. En Marketo, busque y haga clic con el botón derecho en la lista que desee detener la sincronización. Haga clic en **[!UICONTROL Detener sincronización de lista]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Seleccione las audiencias que desea detener y haga clic en **[!UICONTROL Detener]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Haga clic en **[!UICONTROL Detener]** para confirmar.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Cosas que hay que tener en cuenta {#things-to-note}

### Uso compartido en Adobe Analytics {#sharing-to-adobe-analytics}

* Para los usuarios que poseen Adobe Audience Manager y Adobe Analytics, esta integración permite compartir audiencias desde Marketo a sus grupos de informes de Adobe Analytics. Sin embargo, hay que seguir algunos pasos de configuración adicionales en Adobe Audience Manager para habilitar esta opción. Consulte la [documentación de Adobe Audience Manager](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=es){target="_blank"} para obtener más información sobre cómo configurarla.

* Una vez cargada una lista desde Marketo a Adobe Audience Manager, también se puede acceder a ella desde Adobe Target. Esa configuración [debe estar habilitada en Adobe Target](https://experienceleague.adobe.com/es/docs/target/using/integrate/audience-manager-target-integration){target="_blank"}.

* Si una lista está vacía o no tiene personas con valores ECID, el nombre de la lista no se insertará para que se haga referencia fuera de Marketo.

### Uso de rasgos para clientes de Adobe Audience Manager {#trait-usage-aam}

Cuando inicie una exportación de lista en Marketo, verá los siguientes cambios reflejados en la instancia de Adobe Audience Manager:

* Para todas las personas de la lista exportada, Marketo escribirá un rasgo utilizando sus correos electrónicos con hash como identificador entre dispositivos. El nombre de la característica coincidirá con el nombre de audiencia de destino especificado durante la exportación.
* Para todos los ECID que Marketo ha logrado hacer coincidir con People en la lista exportada, Marketo escribirá un rasgo mediante el Identificador de dispositivo ECID. El nombre de la característica coincidirá con el nombre de audiencia de destino especificado durante la exportación.
* Marketo también creará un segmento en la instancia de Audience Manager utilizando el rasgo ECID como único criterio de segmentación. El nombre del segmento coincidirá con el Nombre de audiencia de destino especificado durante la exportación.

## Preguntas frecuentes {#faq}

**¿Por qué el tamaño de la lista en Marketo es diferente al de Adobe?**

Bajo el capó, la integración de audiencias funciona sincronizando las cookies de Marketo Munchkin con la cookie de ECID de Adobe correspondiente. Marketo solo puede compartir datos de pertenencia de personas para las que Marketo haya sincronizado un ECID. Para obtener los mejores resultados posibles, se recomienda cargar el script de seguimiento munchkin.js de Marketo en paralelo con el código de seguimiento visitor.js de Adobe en todas las páginas en las que esté interesado en realizar el seguimiento con fines de marketing.

**¿Cómo funciona la sincronización de cookies?**

Cuando la sincronización de cookies está habilitada para su suscripción a Marketo, munchkin.js de Marketo intentará capturar y almacenar los ECID de Adobe para la organización IMS de Adobe que haya especificado durante la configuración de la integración y hacer coincidir estos ECID con el identificador de cookie de Marketo correspondiente. Esto permite que los perfiles de usuario anónimos de Marketo se enriquezcan con ECID de Adobe.

Se requiere un paso adicional para asociar el perfil de usuario anónimo a un perfil de persona, que se identifica mediante un correo electrónico de texto sin formato. Se [describe aquí](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"} cómo funciona esto exactamente.

**¿Qué información se comparte?**

Esta integración solo comparte información de pertenencia a listas de Marketo a Adobe (por ejemplo, el conocimiento de que la persona X es miembro de la lista Y). No se comparten atributos de persona adicionales con Adobe a través de esta integración.
