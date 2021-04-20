---
title: priority-override-for-déclencheur-igns
description: Anulación de prioridad para campañas de Déclencheur
exl-id: 4468868c-33d7-4b5e-b524-bfcc2785c8ce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Anulación de prioridad para campañas de Déclencheur

<br> 

Los administradores pueden anular la prioridad determinada de Marketo para las campañas de déclencheur a fin de establecer prioridades que se ajusten mejor a los objetivos empresariales.

>[!NOTE]
>
>Esta función solo está disponible para campañas de déclencheur y para usuarios a los que se ha concedido el permiso &quot;Editar prioridad de campaña de Déclencheur&quot;.

>[!CAUTION]
>
>Se recomienda encarecidamente que utilice esta función en un conjunto limitado de campañas críticas para el negocio (el máximo recomendado es 25). El uso de la función de forma flexible en un conjunto grande puede afectar negativamente a la ejecución general de la campaña.

## Anular prioridad

1. En la campaña de déclencheur, haga clic en la pestaña **[!UICONTROL Schedule]** y, a continuación, haga clic en **[!UICONTROL Override Priority]**.

   ![Imagen uno](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Elija un nuevo nivel de prioridad en la lista desplegable. Haga clic en **[!UICONTROL Confirm]**.

   ![Imagen dos](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Imagen tres](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Puede ver la prioridad predeterminada de su campaña en [!UICONTROL Campaign Queue] en [!UICONTROL Marketing Activities]. Para mejorar la tasa de ejecución, se recomienda establecer la prioridad de la campaña en un nivel superior al predeterminado.
>* La prioridad establecida por el usuario solo se aplica a las personas nuevas que cumplen los requisitos para la campaña; las personas que ya estén en cola no se verán afectadas.


## Restaurar prioridad

1. Para restablecer la prioridad de campaña a la predeterminada del sistema, vaya a la pestaña **[!UICONTROL Schedule]** de la campaña de déclencheur y haga clic en **[!UICONTROL Reset Priority]**.

   ![Imagen Cuatro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Haga clic en **[!UICONTROL Reset]** para confirmar.

   ![Imagen cinco](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Las anulaciones y los restablecimientos de prioridad se capturan en la pista de auditoría. Puede ver la [Pista de auditoría](https://docs.marketo.com/x/GZ2t) a través del área [!UICONTROL Administración] en la experiencia clásica.

## Conceder acceso de anulación de prioridad

>[!CAUTION]
>
>Solo los administradores o usuarios con responsabilidades administrativas deben tener acceso de anulación de la prioridad de campaña.

1. En el área [!UICONTROL Administración], haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![Imagen seis](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Haga clic en la pestaña **[!UICONTROL Roles]**, seleccione el usuario al que desea conceder acceso y, a continuación, haga clic en **[!UICONTROL Editar función]**.

   ![Image Seven](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. En [!UICONTROL Acceso a actividades de marketing], marque **[!UICONTROL Editar prioridad de campaña de Déclencheur]**. Haga clic en **[!UICONTROL Guardar]**.

   ![Imagen ocho](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Ver la prioridad de campaña en Marketo Classic

Puede ver la prioridad de campaña en la experiencia [!DNL Classic] haciendo clic en la pestaña **[!UICONTROL Schedule]** dentro de una campaña de déclencheur.

![Imagen nueve](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>La prioridad de la experiencia [!DNL Classic] es de solo vista. El cambio o restablecimiento de la prioridad de campaña solo está disponible mediante el Marketo Sky .
