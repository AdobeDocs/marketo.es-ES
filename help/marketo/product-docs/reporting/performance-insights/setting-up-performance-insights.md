---
unique-page-id: 12981145
description: Configuración de perspectivas de rendimiento - Documentos de marketing - Documentación del producto
title: Configuración de perspectivas de rendimiento
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Configuración de perspectivas de rendimiento {#setting-up-performance-insights}

Siga los pasos a continuación para configurar MPI.

## Configuración de oportunidad {#opportunity-setup}

1. Haga clic en **Administración**.

   ![](assets/admin.png)

1. Haga clic en **Análisis del ciclo de ingresos**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Si no tiene RCA, deberá seleccionar **Análisis de Programa** para el paso 2.

1. En Atribución, haga clic en **Editar**.

   ![](assets/three-1.png)

1. Se muestra Configuración de atribución.

   ![](assets/four-2.png)

   Si la atribución es explícita, asegúrese de que se ha rellenado la función de contacto de oportunidad (ya sea mediante el extremo de la función de oportunidad o mediante la integración de CRM).

   Si la atribución está implícita, asegúrese de que el campo de compañía del posible cliente o contacto sea el mismo que el nombre de la cuenta de la oportunidad.

   >[!NOTE]
   >
   >Asegúrese de que todas las oportunidades tengan rellenados los campos correspondientes:
   >
   >* Cantidad de oportunidad
   >* Está cerrado
   >* Es Ganado
   >* Fecha de creación (puede que no esté establecida en su caso)
   >* Fecha de cierre (puede que no esté establecida en su caso)
   >* Tipo de oportunidad


## Configuración de programa {#program-setup}

Actualice los costes de programa durante al menos 12 meses. Puede hacerlo manualmente o mediante la API de programa. En este ejemplo lo hacemos manualmente.

1. Haga clic en **Actividades de mercadotecnia**.

   ![](assets/ma.png)

1. Busque y seleccione su programa.

   ![](assets/select-program.png)

1. Haga clic en la ficha **Configuración**.

   ![](assets/setup-tab.png)

1. Arrastre **Costo de período** al lienzo.

   ![](assets/period-cost.png)

1. Establezca el Mes de Programa para hace al menos 12 meses y haga clic en **Aceptar**.

   ![](assets/set-period.png)

1. Configure el costo del período y haga clic en **Guardar**.

   ![](assets/set-cost.png)

A continuación, revise el comportamiento de los análisis para indicar si se debe incluir un canal concreto en los análisis. Establezca el comportamiento de Analytics (Normal, Inclusivo, Operativo).

1. Haga clic en **Administración**.

   ![](assets/admin.png)

1. Haga clic en **Etiquetas**.

   ![](assets/tags.png)

1. Haga clic en **+** para expandir la lista de Canal.

   ![](assets/channel.png)

1. Haga clic con el doble en el canal que desee.

   ![](assets/channel-click.png)

1. Haga clic en la lista desplegable **Comportamiento de Analytics** y seleccione el comportamiento que desee.

   ![](assets/edit-channel.png)

1. Establezca los criterios de éxito.

   ![](assets/success.png)

1. Haga clic en **Guardar**.

   ![](assets/save.png)

## Enlazar el Programa con la persona {#tie-the-program-to-the-person}

1. Asegúrese de que el Programa de adquisición y la fecha de adquisición se han establecido para cada persona de la base de datos para que funcione la atribución de primer toque.
1. Asegúrese de que sus programas estén configurando los estados de éxito para su gente.

>[!NOTE]
>
>Los cambios realizados no son instantáneos. Se requiere un período nocturno antes de que los cambios entren en vigor.
