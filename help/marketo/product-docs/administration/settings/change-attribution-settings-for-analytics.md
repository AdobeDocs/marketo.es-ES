---
unique-page-id: 2360217
description: Cambiar la configuración de atribución para Analytics - Documentos de marketing - Documentación del producto
title: Cambiar la configuración de atribución para Analytics
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Cambiar la configuración de atribución para Analytics {#change-attribution-settings-for-analytics}

Puede cambiar la forma en que Marketing vincula los contactos con las oportunidades de atribución de primer toque y de varios toques, las métricas de conversión de posibles clientes y el indicador de oportunidad influenciado por el marketing.

Esta configuración afectará los informes del Explorador de ingresos en las áreas [Análisis de oportunidad de Programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análisis de oportunidad](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) y Análisis de posibles clientes. Esto también afectará al informe Analizador de Programas.

1. En la sección **Administración**, haga clic en **Análisis del ciclo de ingresos**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Haga clic en el vínculo **Editar** en **Atribución**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Si se cambia esta configuración no se modifica ningún dato de marketing; simplemente cambia la forma en que se ejecutan los informes. Esto puede revertirse en cualquier momento.

1. Seleccione una opción y haga clic en **Guardar**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >**Explícita**: Solo contactos con funciones (predeterminado).
   >
   >**Híbrido**: Contactos con funciones si están disponibles. Si no hay ninguno disponible, utiliza todos los contactos de las cuentas.
   >
   >**Implícito**: Todos los contactos, independientemente de su función.

>[!CAUTION]
>
>Al utilizar **Implícito**, Marketing siempre examinará todos los contactos asociados a la cuenta independientemente de la función. **Marketo recomienda enfáticamente utilizar el modo** explícito. El uso de Implícito puede crear falsos positivos; es decir, personas a las que se atribuye una oportunidad a pesar de no tener una influencia real en la oportunidad. Utilice Implícito con precaución.
