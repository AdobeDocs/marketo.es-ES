---
unique-page-id: 2360217
description: Cambio de la configuración de atribución para Analytics - Marketo Docs - Documentación del producto
title: Cambiar la configuración de atribución para Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketo vincula los contactos con las oportunidades para la atribución de primer toque y de varios toque, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

Esta configuración afectará a los informes del Explorador de ingresos en la sección [Análisis de oportunidades del programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análisis de oportunidades](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)y Análisis de posibles clientes. Esto también afectará al informe del Analizador de programas.

1. Vaya a la **Administrador** .

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Haga clic en **Análisis del ciclo de ingresos**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Haga clic en el **Editar** vincular en **Atribución**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Si se cambia esta configuración, no se modificarán los datos de Marketo. simplemente cambia la forma en que se ejecutan los informes. Esto se puede invertir en cualquier momento.

1. Seleccione una opción y haga clic en **Guardar**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >**Explícito**: Solo contactos con roles (predeterminado).
   >
   >**Híbrido**: Contactos con funciones si están disponibles. Si ninguna está disponible, utiliza todos los contactos de las cuentas.
   >
   >**Implicit**: Todos los contactos independientemente de la función.

>[!CAUTION]
>
>Al usar **Implicit**, Marketo siempre examinará todos los contactos asociados a la cuenta, independientemente de su función. **Marketo recomienda encarecidamente utilizar el modo explícito**. El uso de Implicit puede crear falsos positivos; es decir, personas a las que se atribuye una oportunidad a pesar de no tener influencia real en la oportunidad. Utilice Implicit con precaución.
