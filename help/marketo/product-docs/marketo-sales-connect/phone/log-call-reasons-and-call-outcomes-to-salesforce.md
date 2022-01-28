---
description: Razones de la llamada de registro y resultados de la llamada a Salesforce - Marketo Docs - Documentación del producto
title: Razones de la llamada de registro y resultados de la llamada a Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
source-git-commit: d2d6d4389f5a480afdfae6bfb62b9f48f0a2d88e
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Razones de la llamada de registro y resultados de la llamada a Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Si desea registrar los resultados de las llamadas y llamar a Salesforce por motivos de informes o visibilidad, puede crear un campo de actividad personalizado para cada uno. Cada campo debe utilizar un nombre de API específico (denominado &quot;Nombre de campo&quot; en Salesforce).

* Nombre del campo Resultados de la llamada: mktosales_call_result
* Nombre del campo Razones de la llamada: mktosales_call_reason

Para utilizar estos campos, primero debe crear el campo como campo de actividad personalizado. Para que los usuarios puedan verlo, deberá agregarlo al diseño de página del objeto de tarea.

## Salesforce Classic {#salesforce-classic}

### Crear campo de actividad personalizado en Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Escriba &quot;Actividades&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Haga clic en **Campos personalizados de actividad**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Haga clic en **Nuevo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Seleccione el tipo de datos &quot;Texto&quot; y haga clic en **Siguiente**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Asigne al campo personalizado el nombre del campo tal como se ha definido anteriormente. La longitud del campo tiene un límite de 255 caracteres. Field Label será el campo visible para su equipo de ventas y puede personalizarse para satisfacer las necesidades de su equipo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. El resto de los ajustes son opcionales. Una vez completada la configuración, haga clic en **Siguiente**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Seleccione la configuración de seguridad de nivel de campo que desee para este campo y haga clic en **Siguiente** (la imagen siguiente es solo un ejemplo).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Asegúrese de que el campo personalizado sea visible para el perfil que utilizan los usuarios de Sales Connect, junto con cualquier otro lugar en el que desee que sea visible.

1. Seleccione a qué diseños de página desea añadir el campo y haga clic en **Guardar** (opcionalmente, puede hacer clic en **Guardar y nuevo** y repita el proceso para el campo Razón de la llamada ).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Agregar campo de actividad personalizado al diseño de página de tarea en Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Solo tendrá que seguir estos pasos si no ha seleccionado el diseño de página deseado en el paso 9 anterior.

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Escriba &quot;Tarea&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Haga clic en **Diseños de páginas de tareas**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Haga clic en **Editar** junto al diseño de la página de tareas a la que desea añadir este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Arrastre y suelte el campo en la sección deseada del diseño de página Tarea .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Haga clic en **Guardar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Crear campo de actividad personalizado en el relámpago de Salesforce {#create-custom-activity-field-in-salesforce-lightning}

1. En Salesforce, haga clic en el icono de engranaje en la parte superior derecha y seleccione **Configuración**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Haga clic en **Administrador de objetos**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Escriba &quot;Actividad&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Haga clic en el **Actividad** etiqueta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Haga clic en **Campos y relaciones**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Haga clic en **Nuevo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Agregar campo de actividad personalizado al diseño de página de tarea en el relámpago de Salesforce {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. En Salesforce, haga clic en el icono de engranaje en la parte superior derecha y seleccione **Configuración**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Haga clic en **Administrador de objetos**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Escriba &quot;Tarea&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Haga clic en el **Tarea** etiqueta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Haga clic en **Diseños de página**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Haga clic en el diseño de página de la tarea al que desee agregar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Arrastre y suelte el campo en la sección deseada del diseño de página Tarea .

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Haga clic en **Guardar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Instalar campos de evento de conexión de ventas en el historial de actividades](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
