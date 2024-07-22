---
unique-page-id: 12981145
description: Configuración de perspectivas de rendimiento - Documentos de Marketo - Documentación del producto
title: Configuración de perspectivas de rendimiento
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 3%

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
   >Si no tiene RCA, tendrá que seleccionar **Análisis de programa** para el paso 2.

1. En Atribución, haga clic en **Editar**.

   ![](assets/three-1.png)

1. Se muestra Configuración de atribución.

   ![](assets/four-2.png)

   Si la Atribución es explícita, asegúrese de que la Función de contacto de oportunidad se haya rellenado (a través del punto de conexión de la Función de oportunidad o a través de la integración de CRM).

   Si la Atribución está implícita, asegúrese de que el campo de empresa del posible cliente/contacto sea el mismo que el Nombre de cuenta de la oportunidad.

   >[!NOTE]
   >
   >Asegúrese de que todas las oportunidades tengan los campos adecuados rellenados:
   >
   >* Monto de la oportunidad
   >* Es cerrado
   >* Está ganado
   >* Fecha de creación (puede que no se establezca en su caso)
   >* Fecha de cierre (puede que no se establezca en su caso)
   >* Tipo de oportunidad

## Configuración del programa {#program-setup}

Actualice los costes del programa durante al menos 12 meses. Puede hacerlo manualmente o mediante la API del programa. En este ejemplo lo hacemos manualmente.

1. Haga clic en **Actividades de marketing**.

   ![](assets/ma.png)

1. Busque y seleccione su programa.

   ![](assets/select-program.png)

1. Haga clic en la ficha **Configuración**.

   ![](assets/setup-tab.png)

1. Arrastre **Costo de período** al lienzo.

   ![](assets/period-cost.png)

1. Establezca el mes del programa como mínimo hace 12 meses y haga clic en **Aceptar**.

   ![](assets/set-period.png)

1. Establezca el costo del período y haga clic en **Guardar**.

   ![](assets/set-cost.png)

A continuación, revise el comportamiento de Analytics para indicar si algún canal en particular debe incluirse en Analytics. Establezca el Comportamiento de Analytics (Normal, Inclusivo, Operativo).

1. Haga clic en **Administrador**.

   ![](assets/admin.png)

1. Haga clic en **Etiquetas**.

   ![](assets/tags.png)

1. Haga clic en **+** para expandir la lista de canales.

   ![](assets/channel.png)

1. Haga doble clic en el canal deseado.

   ![](assets/channel-click.png)

1. Haga clic en el menú desplegable **Comportamiento de Analytics** y seleccione el comportamiento que desee.

   ![](assets/edit-channel.png)

1. Defina los criterios de éxito.

   ![](assets/success.png)

1. Haga clic en **Guardar**.

   ![](assets/save.png)

## Vinculación del programa a la persona {#tie-the-program-to-the-person}

1. Asegúrese de que el programa de adquisición y la fecha de adquisición se hayan establecido para cada persona de la base de datos para que funcione la Atribución de primer contacto.
1. Asegúrese de que los programas establezcan estados de éxito para sus recursos.

>[!NOTE]
>
>Los cambios realizados no son instantáneos. Se requiere un período de un día para que los cambios entren en vigor.
