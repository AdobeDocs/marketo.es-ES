---
description: 'Errores de sincronización de Salesforce: Documentos de Marketo: documentación del producto'
title: Errores de sincronización de Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 6%

---

# [!DNL Salesforce] errores de sincronización {#salesforce-sync-errors}

Ver un resumen de los errores enfrentados durante el proceso de sincronización. Esto incluye errores causados por errores en la sincronización de datos incompatibles.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Ver errores de sincronización {#view-sync-errors}

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/salesforce-sync-errors-1.png)

1. En Integración, haga clic en **Salesforce** y luego en la ficha **[!UICONTROL Errores de sincronización]**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Los errores enumerados varían desde la hora actual hasta cinco días antes de la sincronización actual.

| Campo | Descripción |
|---|---|
| Error en | Nivel de registro _o_ nivel de trabajo |
| Fecha y hora del error | Detalles del error |
| Tipo de error | Mensaje de retorno de SFDC |

>[!TIP]
>
>Al hacer clic en el registro de nivel de registro, se muestran el Marketo y [!DNL Salesforce] ID del objeto relacionado. En algunos casos, el mensaje de los errores de nivel de registro y trabajo procede directamente de [!DNL Salesforce]. La búsqueda de ellos en línea puede proporcionar detalles adicionales.

## Filtrar errores de sincronización {#filter-sync-errors}

1. Para filtrar los datos, haga clic en el icono de filtro situado en el extremo derecho de la página.

   ![](assets/salesforce-sync-errors-3.png)

1. Seleccione la fecha y el intervalo de tiempo y, a continuación, filtre por tipo de error (nivel de trabajo o nivel de registro). Haga clic en **[!UICONTROL Aplicar]** cuando haya terminado.

   ![](assets/salesforce-sync-errors-4.png)

**PASO OPCIONAL**: Para exportar los errores de sincronización, haga clic en **[!UICONTROL Exportar]**. Los datos se exportarán como CSV.

![](assets/salesforce-sync-errors-5.png)
