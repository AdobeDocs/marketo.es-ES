---
unique-page-id: 2360217
description: Cambio de la configuración de atribución para Analytics - Marketo Docs - Documentación del producto
title: Cambiar la configuración de atribución para Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketo vincula los contactos con las oportunidades para la atribución de primer toque y de varios toque, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

Esta configuración afecta a los informes del Explorador de ingresos en las áreas [Análisis de oportunidades de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análisis de oportunidades](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) y Análisis de posibles clientes. Esto también afectará al informe del Analizador de programas.

1. En la sección **Administración**, haga clic en **Análisis del ciclo de ingresos**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Haga clic en el enlace **Edit** en **Attribution**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Si se cambia esta configuración, no se modificarán los datos de Marketo. simplemente cambia la forma en que se ejecutan los informes. Esto se puede invertir en cualquier momento.

1. Seleccione una opción y haga clic en **Save**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

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
>Al utilizar **Implicit**, Marketo siempre examinará todos los contactos asociados a la cuenta, independientemente de la función. **Marketo recomienda encarecidamente utilizar el modo** Explícito. El uso de Implicit puede crear falsos positivos; es decir, personas a las que se atribuye una oportunidad a pesar de no tener influencia real en la oportunidad. Utilice Implicit con precaución.
