---
unique-page-id: 2359675
description: Desactivación del rellenado previo de un campo de formulario - Documentos de Marketo - Documentación del producto
title: Deshabilitar el rellenado previo de un campo de formulario
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Deshabilitar el rellenado previo de un campo de formulario {#disable-pre-fill-for-a-form-field}

Cuando se conoce (se coordina) a un visitante web, los formularios de Marketo rellenarán previamente los campos con su información de forma predeterminada. Si quieres apagar esto, así es como hacerlo.

>[!NOTE]
>
>**Formulario Previo al** archivo habilitado de forma predeterminada. La configuración de rellenado previo de nivel de página de aterrizaje y la configuración de rellenado previo de nivel de administrador prevalecen sobre la configuración de nivel de formulario:
>
>Formulario > Página de aterrizaje > Administración

## Deshabilitar el rellenado previo {#how-to-disable-pre-fill}

1. Vaya a **Marketing Activities**.

   ![](assets/login-marketing-activities-7.png)

1. Seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >El rellenado previo del formulario no funciona al incrustar un formulario en sus propias páginas. Solo funciona en páginas de aterrizaje de Marketo.

1. Seleccione uno de los campos y establezca **Form Pre-fill** en **Disabled**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >También puede desactivar el rellenado previo del formulario en la página de aterrizaje o a nivel de administrador.

1. Haga clic en **Finish**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Haga clic en **Aprobar y cerrar**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Campos confidenciales {#sensitive-fields}

Cuando [marque un campo como sensible](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md), evitando que sus valores se rellenen previamente en formularios, lo verá en la opción Relleno previo .

![](assets/disable-pre-fill.png)