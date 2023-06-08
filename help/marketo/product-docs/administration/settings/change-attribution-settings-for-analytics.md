---
unique-page-id: 2360217
description: 'Cambiar la configuración de atribución para Analytics: Documentos de Marketo, documentación del producto'
title: Cambiar la configuración de atribución para Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketo vincula los contactos con las oportunidades para la atribución de primer contacto y de varios contactos, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

Esta configuración afectará a [!UICONTROL Explorador de ingresos] informes en el [Análisis de oportunidad de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análisis de oportunidad](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)y áreas de análisis de posibles clientes. Esto también afectará a la [!UICONTROL Analizador de programas] informe.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Clic **[!UICONTROL Análisis del ciclo de ingresos]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Haga clic en **[!UICONTROL Editar]** vínculo en **[!UICONTROL Atribución]**.

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
   >**[!UICONTROL Explícito]**: solo los contactos con funciones (predeterminado).
   >
   >**[!UICONTROL Híbrido]**: contactos con funciones si están disponibles. Si no hay ninguno disponible, utiliza todos los contactos de las cuentas.
   >
   >**[!UICONTROL Implícito]**: todos los contactos independientemente de la función.

>[!CAUTION]
>
>Al utilizar **[!UICONTROL Implícito]**, Marketo siempre examinará todos los contactos asociados a la cuenta, independientemente de la función. **Marketo recomienda encarecidamente utilizar [!UICONTROL Explícito] modo**. Uso de [!UICONTROL Implícito] puede crear falsos positivos; es decir, personas con crédito por una oportunidad a pesar de no tener influencia real en la oportunidad. Uso [!UICONTROL Implícito] con precaución.
