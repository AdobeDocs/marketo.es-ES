---
unique-page-id: 2359418
description: Importar una Lista de personas - Documentos de marketing - Documentación del producto
title: Importar una Lista de personas
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Importar una Lista de personas {#import-a-list-of-people}

## Misión: Importar una lista de hoja de cálculo de asistentes a la presentación de informes en la base de datos {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Requisitos previos**
>
>* [Configurar y Añadir una persona](get-set-up-and-add-a-person.md)

>



`   
`  En este tutorial, aprenderá a importar personas de un archivo de hoja de cálculo en Marketing.

## Paso 1: Descargar y editar una hoja de cálculo {#step-download-and-edit-a-spreadsheet}

1. Para inicio, descargue nuestro archivo de hoja de cálculo de prácticas (** [asistentes a la presentación.csv](http://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)**) en su equipo.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Al importar una fecha, utilice este formato: **21/9/15** (Mes/Día/Año).

   >[!NOTE]
   >
   >Los campos de fecha y hora que se importan se tratan como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla en hora central (América/Chicago).

1. Añada su propio nombre, apellidos, dirección de correo electrónico y título de trabajo y, a continuación, guarde el archivo en su equipo.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Escriba su dirección de correo electrónico real en el archivo CSV para que pueda recibir los mensajes de correo electrónico de atención que enviará en la próxima misión.

## Paso 2: Crear un Programa {#step-create-a-program}

1. Vaya al área Actividades **de** marketing.

   ![](assets/ma-2.png)

1. Seleccione la carpeta **Aprendizaje** y, a continuación, en **Nuevo** , haga clic en **Nuevo Programa**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Asigne un nombre** al programa &quot;Mi Programa de presentación&quot; y seleccione &quot;Evento&quot; para el tipo de **Programa.**

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Seleccione **Presentación** comercial para el **Canal** y haga clic en **Crear**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>**Buceo profundo**
>
>Los programas de evento se producen en fechas específicas. Más información sobre [**Eventos**](http://docs.marketo.com/display/docs/events).

## Paso 3: Importar la hoja de cálculo en Marketing {#step-import-your-spreadsheet-into-marketo}

1. En **Mi Programa** de presentación, haga clic en **Nuevo** y seleccione **Nuevo recurso** local.

   ![](assets/seven-3.png)

1. Haga clic en **Lista**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Asigne un nombre** a la lista &quot;Asistentes a la feria comercial&quot; y haga clic en **Crear**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. En la lista **de asistentes** a la feria comercial, haga clic en Acciones **de** Lista y seleccione **Importar Lista**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Si utiliza su propio archivo CSV, asegúrese de que está codificado como UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >El límite de tamaño de los archivos CSV es de 100 MB.

1. **Vaya** al archivo de hoja de cálculo **de asistentes a la presentación comercial.csv** en el equipo y haga clic en **Siguiente**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >En el modo de importación de Listas, si elige **Omitir nuevas personas y actualizaciones** , no afectará a los registros de personas existentes ni registrará actividades. Utilice este modo si desea una lista estática rápida y prefiltrada de las personas existentes para utilizarla en sus actividades de marketing. Al seleccionar este modo:
   >
   >    
   >    
   >    * Omitir la creación de nuevas personas
   >    * Omitir actualizaciones de campo de persona
   >    * Omitir registro de actividades


1. Asigne los campos Columna de Lista a su correspondiente Campo de marketing y haga clic en **Siguiente**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Los encabezados de columna siempre deben coincidir exactamente con el campo (distinguen mayúsculas de minúsculas) para obtener los mejores resultados de asignación automática. Si está utilizando campos personalizados y no los ve en la lista desplegable, vuelva atrás y [cree los](http://docs.marketo.com/display/DOCS/Create+a+Custom+Field+in+Marketo) campos para que se conviertan en opciones.

   >[!NOTE]
   >
   >Si hay campos que no desea importar, seleccione **Omitir** en el menú desplegable Campo de marketing.

1. Seleccione **Mi Programa** de presentación para el Programa **de** adquisición y, a continuación, haga clic en **Importar**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Espere a que los usuarios importen y cierre la ventana emergente de progreso de importación.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. De vuelta en **Mi Programa** de presentación, haga clic en la ficha **Miembros** . Verás a todas las personas que acabas de importar.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>**Buceo profundo**
>
>Puede analizar el éxito de su programa mediante el seguimiento de la pertenencia a programas. Más información sobre [**Programas**](http://docs.marketo.com/display/docs/programs).

## Misión completada {#mission-complete}

¡Sus asistentes a la feria comercial ahora son miembros de su programa de marketing!

<br> 

[◄ Misión 4: Respuesta](email-auto-response.md) automática por correo electrónico [Misión 6: Derivación, Derivación, Nurtura ►](drip-drip-nurture.md)