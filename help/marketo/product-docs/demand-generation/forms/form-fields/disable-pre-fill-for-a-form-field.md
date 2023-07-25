---
unique-page-id: 2359675
description: Deshabilitar el rellenado previo de un campo de formulario - Documentos de Marketo - Documentación del producto
title: Deshabilitar el rellenado previo de un campo de formulario
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Deshabilitar el rellenado previo de un campo de formulario {#disable-pre-fill-for-a-form-field}

Cuando se conoce a un visitante web (con cookies), los formularios de Marketo rellenarán previamente los campos con su información de forma predeterminada. Si quieres apagar esto, así es como se hace.

>[!NOTE]
>
>**Relleno previo del formulario** está activada de forma predeterminada. La configuración de rellenado previo del nivel de página de aterrizaje y la configuración de relleno previo del nivel de administrador supera la configuración del nivel de formulario:
>
>Formulario > Página de aterrizaje > Administración

## Cómo deshabilitar el relleno previo {#how-to-disable-pre-fill}

1. Ir a **Actividades de marketing**.

   ![](assets/login-marketing-activities-7.png)

1. Seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >El rellenado previo del formulario no funciona al incrustar un formulario en sus propias páginas. Solo funciona en páginas de aterrizaje de Marketo.

1. Seleccione uno de los campos y defina **Relleno previo del formulario** hasta **Desactivado**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >También puede deshabilitar el rellenado previo de formularios en el nivel de página de aterrizaje o de administrador.

1. Clic **Finalizar**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Clic **Aprobar y cerrar**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Campos confidenciales {#sensitive-fields}

Cuando usted [marcar un campo como confidencial](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md), lo que evita que sus valores se rellenen previamente en los formularios, verá esto en la opción Relleno previo.

![](assets/disable-pre-fill.png)