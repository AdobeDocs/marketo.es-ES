---
unique-page-id: 12981145
description: Configuración de perspectivas de rendimiento - Documentos de Marketo - Documentación del producto
title: Configuración de perspectivas de rendimiento
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 2%

---

# Configuración de perspectivas de rendimiento {#setting-up-performance-insights}

Siga los pasos a continuación para configurar MPI.

## Configuración de oportunidad {#opportunity-setup}

1. Haga clic en **Administrador**.

   ![](assets/admin.png)

1. Haga clic en **Análisis del ciclo de ingresos**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Si no tiene RCA, deberá seleccionar **Análisis del programa** para el paso 2.

1. En Atribución, haga clic en **Editar**.

   ![](assets/three-1.png)

1. Configuración de atribución .

   ![](assets/four-2.png)

   Si la atribución es explícita, asegúrese de que se ha rellenado la función de contacto de oportunidad (a través del extremo de la función de oportunidad o a través de la integración de CRM).

   Si Attribution está implícita, asegúrese de que el campo de empresa del posible cliente o contacto sea el mismo que el Nombre de cuenta de la oportunidad.

   >[!NOTE]
   >
   >Asegúrese de que todas las oportunidades tengan los campos adecuados rellenados:
   >
   >* Monto de la oportunidad
   >* Es cerrado
   >* Está ganado
   >* Fecha de creación (puede que no esté establecida en su caso)
   >* Fecha de cierre (es posible que no esté establecido en su caso)
   >* Tipo de oportunidad


## Configuración del programa {#program-setup}

Actualice los costes del programa durante al menos 12 meses. Puede hacerlo manualmente o mediante la API del programa. En este ejemplo lo hacemos manualmente.

1. Haga clic en **Actividades de marketing**.

   ![](assets/ma.png)

1. Busque y seleccione el programa.

   ![](assets/select-program.png)

1. Haga clic en el **Configuración** pestaña .

   ![](assets/setup-tab.png)

1. Arrastrar **Costo de período** en el lienzo.

   ![](assets/period-cost.png)

1. Establezca el Mes del programa para hace al menos 12 meses y haga clic en **Ok**.

   ![](assets/set-period.png)

1. Establezca el coste del periodo y haga clic en **Guardar**.

   ![](assets/set-cost.png)

A continuación, revise el comportamiento de los análisis para indicar si se debe incluir un canal en particular en los análisis. Establezca el comportamiento de Analytics (Normal, Inclusivo, Operativo).

1. Haga clic en **Administrador**.

   ![](assets/admin.png)

1. Haga clic en **Etiquetas**.

   ![](assets/tags.png)

1. Haga clic en el **+** para expandir la lista Canal .

   ![](assets/channel.png)

1. Haga doble clic en el canal deseado.

   ![](assets/channel-click.png)

1. Haga clic en el **Comportamiento de Analytics** y seleccione el comportamiento deseado.

   ![](assets/edit-channel.png)

1. Establezca los criterios de éxito.

   ![](assets/success.png)

1. Haga clic en **Guardar**.

   ![](assets/save.png)

## Vincular el programa a la persona {#tie-the-program-to-the-person}

1. Asegúrese de que el Programa de adquisición y la Fecha de adquisición se hayan establecido para cada persona de la base de datos para que funcione la Atribución de primer toque.
1. Asegúrese de que sus programas estén configurando estados de éxito para su gente.

>[!NOTE]
>
>Los cambios realizados no son instantáneos. Se requiere un periodo de pernoctación antes de que los cambios entren en vigor.
