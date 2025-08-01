---
unique-page-id: 2360217
description: 'Cambiar la configuración de atribución para Analytics: Documentos de Marketo, documentación del producto'
title: Cambiar la configuración de atribución para Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketo vincula los contactos con las oportunidades para la atribución de primer contacto y de varios contactos, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

Esta configuración afectará los informes de [!UICONTROL Explorador de ingresos] en las áreas de [Análisis de oportunidad de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análisis de oportunidad](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) y Análisis de posibles clientes. Esto también afectará el informe [!UICONTROL Analizador de programas].

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Haga clic en **[!UICONTROL Análisis del ciclo de ingresos]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Haga clic en el vínculo **[!UICONTROL Editar]** en **[!UICONTROL Atribución]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Al cambiar esta configuración no se modifica ningún dato de Marketo; simplemente se cambia la forma en que se ejecutan los informes. Esto se puede revertir en cualquier momento.

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
