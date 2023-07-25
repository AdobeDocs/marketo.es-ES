---
description: 'Errores de sincronización de Salesforce: Documentos de Marketo: documentación del producto'
title: Errores de sincronización de Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 2%

---

# Errores de sincronización de Salesforce {#salesforce-sync-errors}

Ver un resumen de los errores enfrentados durante el proceso de sincronización. Esto incluye errores causados por errores en la sincronización de datos incompatibles.

>[!NOTE]
>
>**Permisos de administración necesarios**

## Ver errores de sincronización {#view-sync-errors}

1. Clic **Administrador**.

   ![](assets/salesforce-sync-errors-1.png)

1. En Integración, haga clic en **Salesforce** y, a continuación, el **Errores de sincronización** pestaña.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Los errores enumerados varían desde la hora actual hasta cinco días antes de la sincronización actual.

| Campo | Descripción |
|---|---|
| Error el | Nivel de registro _o_ Nivel de trabajo |
| Fecha y hora del error | Detalles del error |
| Tipo de error | Mensaje devuelto de SFDC |

>[!TIP]
>
>Al hacer clic en el registro de nivel de registro, se muestran los ID de Marketo y Salesforce del objeto relacionado. En algunos casos, el mensaje de los errores de nivel de registro y trabajo procede directamente de Salesforce. La búsqueda de ellos en línea puede proporcionar detalles adicionales.

## Filtrar errores de sincronización {#filter-sync-errors}

1. Para filtrar los datos, haga clic en el icono de filtro situado en el extremo derecho de la página.

   ![](assets/salesforce-sync-errors-3.png)

1. Seleccione la fecha y el intervalo de tiempo y, a continuación, filtre por tipo de error (nivel de trabajo o nivel de registro). Clic **Aplicar** cuando termine.

   ![](assets/salesforce-sync-errors-4.png)

**PASO OPCIONAL**: Para exportar los errores de sincronización, haga clic en **Exportar**. Los datos se exportarán como CSV.

![](assets/salesforce-sync-errors-5.png)
