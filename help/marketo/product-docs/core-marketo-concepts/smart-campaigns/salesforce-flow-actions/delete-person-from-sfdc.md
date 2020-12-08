---
unique-page-id: 1147031
description: Eliminar persona de SFDC - Documentos de marketing - Documentación del producto
title: Eliminar persona de SFDC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Eliminar persona de SFDC {#delete-person-from-sfdc}

Si necesita eliminar un conjunto específico de leads de Salesforce pero dejarlos como personas en Marketing, puede utilizar la acción Eliminar persona de flujo SFDC.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Sólo disponible cuando se integra con Salesforce.

1. En la base de datos, haga clic en la persona que desee eliminar de Salesforce. A continuación, haga clic en **Acciones** personales y seleccione **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Seleccione **Eliminar persona de SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Asegúrese de que la opción **Eliminar en marketing** es **falsa** y, a continuación, haga clic en **Ejecutar ahora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Después de que se ejecute el paso de flujo, su persona ya no será un líder en Salesforce, pero permanecerá en Marketing.

   >[!CAUTION]
   >
   >Si establece **Eliminar en Marketing** en **true** y elimina las personas de Marketing y los leads de Salesforce, éstas desaparecerán para siempre. Esto no se puede deshacer.

