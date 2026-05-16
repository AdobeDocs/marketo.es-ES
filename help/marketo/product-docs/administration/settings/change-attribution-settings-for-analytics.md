---
unique-page-id: 2360217
description: Cómo establecer opciones de atribución de primer contacto y de múltiples contactos, conversión de posibles clientes y oportunidades influidas por el marketing en Revenue Cycle Analytics.
title: Cambiar la configuración de atribución para Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 5%

---

# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketo vincula los contactos con las oportunidades para la atribución de primer contacto y de varios contactos, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Haga clic en **[!UICONTROL Análisis del ciclo de ingresos]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Haga clic en el vínculo **[!UICONTROL Editar]** en **[!UICONTROL Atribución]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Al cambiar esta configuración no se modifica ningún dato de Marketo; cambia la forma en que se ejecutan los informes. Esto se puede revertir en cualquier momento.

1. Seleccione una opción y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >**[!UICONTROL Explícito]**: solo los contactos con roles (predeterminado).
   >
   >**[!UICONTROL Híbrido]**: contactos con funciones si están disponibles. Si no hay ninguno disponible, utiliza todos los contactos de las cuentas.
   >
   >**[!UICONTROL Implícito]**: todos los contactos independientemente de la función.

>[!CAUTION]
>
>Al usar **[!UICONTROL Implicit]**, Marketo siempre examinará todos los contactos asociados a la cuenta, independientemente de la función. **Marketo recomienda encarecidamente usar [!UICONTROL Modo explícito]**. El uso de [!UICONTROL Implicit] puede crear falsos positivos; es decir, personas con crédito por una oportunidad a pesar de no tener influencia real en la oportunidad. Use [!UICONTROL Implícito] con precaución.
