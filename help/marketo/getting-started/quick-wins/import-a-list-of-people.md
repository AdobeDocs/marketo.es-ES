---
unique-page-id: 2359418
description: 'Importar una lista de personas: Marketo Docs: documentación del producto'
title: Importar una lista de personas
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Importar una lista de personas {#import-a-list-of-people}

## Misión: Importe una hoja de cálculo de los asistentes a los programas comerciales en la base de datos {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

En este tutorial, aprenderá a importar personas de un archivo de hoja de cálculo en Marketo.

## Paso 1: Descargar y editar una hoja de cálculo {#step-download-and-edit-a-spreadsheet}

1. Para empezar, descargue nuestro archivo de hoja de cálculo de prácticas ([**discursos-asistentes.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)) en su equipo.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Al importar una fecha, use este formato: **21/9/20** (Mes/Día/Año).

   >[!NOTE]
   >
   >Cualquier campo de fecha y hora que se importe se tratará como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla a la hora central (América/Chicago).

1. Añada su propio nombre, apellido, dirección de correo electrónico y puesto de trabajo y, a continuación, guarde el archivo en su equipo.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Introduzca su dirección de correo electrónico real en el archivo CSV para que pueda recibir los correos electrónicos de alimentación que enviará en la próxima misión.

## Paso 2: Crear un programa {#step-create-a-program}

1. Vaya al área **Marketing Activities** .

   ![](assets/ma-2.png)

1. Seleccione la carpeta **Learning** y, a continuación, en **New** haga clic en **New Program**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** Asigne un nombre al programa &quot;Mi programa de presentación de ofertas&quot; y seleccione &quot;Evento&quot; para el  **tipo** de programa.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Seleccione **Tradeshow** para el **Channel** y haga clic en **Create**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Los programas de eventos se producen en fechas específicas. Obtenga más información sobre [**Events**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Paso 3: Importar la hoja de cálculo en Marketo {#step-import-your-spreadsheet-into-marketo}

1. En **My Tradeshow Program**, haga clic en **New** y seleccione **New Local Asset**.

   ![](assets/seven-3.png)

1. Haga clic en **List**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** Asigne un nombre a la lista &quot;Asistentes a la feria comercial&quot; y haga clic en  **Crear**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. En la lista **Ofertas de asistencia**, haga clic en **Acciones de lista** y seleccione **Lista de importación**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Si utiliza su propio archivo CSV, asegúrese de que está codificado en UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >El límite de tamaño para los archivos CSV es de 100 MB.

1. **** Vaya al archivo  **trashow-atendees.** csvhoja de cálculo de su equipo y haga clic en  **Siguiente**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >En el modo de importación de lista, elegir **Omitir nuevas personas y actualizaciones** significa que no afectará a los registros de personas existentes ni registrará ninguna actividad. Utilice este modo si desea una lista estática rápida y prefiltrada de personas existentes para utilizarla en sus actividades de marketing. Al seleccionar este modo:
   >
   > * Omitir la creación de nuevas personas
   > * Omitir actualizaciones de campos de persona
   > * Omitir el registro de actividades


1. Asigne los campos de la columna de lista a sus respectivos campos de Marketo y haga clic en **Siguiente**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Los encabezados de columna siempre deben coincidir exactamente con el campo (con distinción de mayúsculas y minúsculas) para lograr los mejores resultados de asignación automática. Si está utilizando campos personalizados y no los ve en la lista desplegable, vuelva atrás y [créelos](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) para que puedan convertirse en opciones.

   >[!NOTE]
   >
   >Si hay campos que no desea importar, seleccione **Ignore** en el menú desplegable Campo de Marketo.

1. Seleccione **My Tradeshow Program** para el **Programa de adquisición** y haga clic en **Importar**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Espere a que las personas se importen y cierre la ventana emergente de progreso de importación.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. De nuevo en **My Tradeshow Program**, haga clic en la pestaña **Members**. Verán a todas las personas que acaban de importar.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Puede analizar el éxito del programa realizando un seguimiento de la pertenencia a este. Obtenga más información sobre [**Programas**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Misión completada {#mission-complete}

¡Sus asistentes a la feria comercial ahora son miembros de su programa de Marketo!

<br> 

[◄ Misión 4: Respuesta automática de correo electrónico](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Misión 6: Perforación, Perforación, Enfermedad ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
