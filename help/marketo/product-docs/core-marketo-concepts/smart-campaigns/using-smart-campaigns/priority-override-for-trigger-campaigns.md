---
description: Obtenga información acerca de la anulación de prioridades para campañas de déclencheur. Controle qué campaña se ejecuta cuando se activan varios déclencheur para la misma persona.
title: Anulación de prioridad para campañas de activador
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/XEyORsYajQEhtF-bajLFTtbOsSFg-lM9zU4gUyFcmWk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 5%

---

# Anulación de prioridad para campañas de activador {#priority-override-for-trigger-campaigns}

Los administradores pueden anular la prioridad definida por Marketo Engage para las campañas de Déclencheur a fin de establecer prioridades que se ajusten mejor a los objetivos empresariales.

>[!NOTE]
>
>Esta característica solo está disponible para campañas de Déclencheur y para los usuarios a los que se les ha concedido el permiso [&quot;Editar prioridad de campaña de Déclencheur&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>Se recomienda encarecidamente que utilice esta función en un conjunto limitado de campañas críticas para el negocio (25 es el máximo recomendado). El uso de la función en un conjunto grande puede afectar negativamente a la ejecución general de la campaña.

## Conceder acceso de anulación de prioridad {#grant-priority-override-access}

>[!NOTE]
>
>Solo los administradores o usuarios con responsabilidades de administrador deben tener acceso de anulación de prioridad de campaña.

1. En el área **[!UICONTROL Administrador]**, haga clic en **[!UICONTROL Usuarios y roles]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Haga clic en la ficha **[!UICONTROL Roles]**, seleccione el usuario al que desea conceder acceso y, a continuación, haga clic en **[!UICONTROL Editar rol]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. En **[!UICONTROL Acceder a actividades de marketing]**, seleccione **[!UICONTROL Editar prioridad de campaña de Déclencheur]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Invalidar prioridad {#override-priority}

1. Busque la campaña de Déclencheur. Haga clic con el botón derecho en él y seleccione **[!UICONTROL Anular prioridad de campaña]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Haga clic en el control deslizante **[!UICONTROL Anular prioridad de campaña]** para habilitar. Elija un nuevo nivel de prioridad y haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   El nuevo nivel de prioridad se mostrará en la ficha **[!UICONTROL Programar]**.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Puede ver la prioridad predeterminada de su campaña en [!UICONTROL Cola de campaña] en [!UICONTROL Actividades de marketing]. Para aumentar la tasa de ejecución, recomendamos establecer la prioridad de la campaña en un nivel superior al predeterminado.
>* La prioridad establecida por el usuario solo se aplica a las nuevas personas que cumplen los requisitos para la campaña; las personas que ya están en cola no se verán afectadas.
>* Las invalidaciones de prioridad se capturan en [pista de auditoría](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}.
