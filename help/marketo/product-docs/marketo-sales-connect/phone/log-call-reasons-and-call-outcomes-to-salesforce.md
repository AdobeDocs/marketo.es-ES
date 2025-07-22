---
description: 'Registrar motivos de llamada y resultados de llamada a Salesforce: documentos de Marketo, documentación del producto'
title: Registrar motivos de llamada y resultados de llamada a Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Registrar motivos de llamada y resultados de llamada a [!DNL Salesforce] {#log-call-reasons-and-call-outcomes-to-salesforce}

Si desea registrar los resultados de las llamadas y los motivos de la llamada a [!DNL Salesforce] con fines de creación de informes o visibilidad, puede crear un campo de actividad personalizado para cada uno. Cada campo debe usar un Nombre de API específico (conocido como &quot;Nombre de campo&quot; en [!DNL Salesforce]).

* Nombre del campo Resultados de la llamada: mktosales_call_result
* Nombre del campo Razones de la llamada: mktosales_call_reason

Para utilizar estos campos, primero debe crear el campo como un campo de actividad personalizado. Para que sea visible para los usuarios, debe agregarlo al diseño de página del objeto de tarea.

## [!DNL Salesforce] Classic {#salesforce-classic}

### Crear campo de actividad personalizado en [!DNL Salesforce] clásico  {#create-custom-activity-field-in-salesforce-classic}

1. En [!DNL Salesforce], haga clic en **[!UICONTROL Configuración]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Escriba &quot;Actividades&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Haga clic en **[!UICONTROL Campos personalizados de actividad]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Seleccione el tipo de datos &quot;[!UICONTROL Texto]&quot; y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Asigne al campo personalizado el nombre del campo tal como se ha definido anteriormente. La longitud del campo tiene un límite de 255 caracteres. Etiqueta de campo será el campo visible para su equipo de ventas y se puede personalizar para satisfacer las necesidades de su equipo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. El resto de los ajustes son opcionales. Una vez que haya completado la configuración, haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Seleccione la configuración de seguridad de nivel de campo que desee para este campo y haga clic en **[!UICONTROL Siguiente]** (la imagen siguiente es solo un ejemplo).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Asegúrese de que el campo personalizado esté visible para el perfil que utilizan los usuarios de [!DNL Sales Connect], junto con cualquier otro lugar donde desee que esté visible.

1. Seleccione a qué diseños de página desea agregar el campo y haga clic en **[!UICONTROL Guardar]** (opcionalmente, puede hacer clic en **[!UICONTROL Guardar y nuevo]** y repetir el proceso para el campo Motivo de la llamada).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Agregar campo de actividad personalizado al diseño de página de tarea en [!DNL Salesforce] Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Solo tendrá que seguir estos pasos si no seleccionó el diseño de página deseado en el paso 9 anterior.

1. En [!DNL Salesforce], haga clic en **[!UICONTROL Configuración]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Escriba &quot;Tarea&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Haga clic en **[!UICONTROL Diseños de página de tareas]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Haga clic en **[!UICONTROL Editar]** junto al diseño de página de tarea al que desee agregar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Arrastre y suelte el campo en la sección deseada del diseño de página de la tarea.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce] relámpagos {#salesforce-lightning}

### Crear campo de actividad personalizado en [!DNL Salesforce] Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. En [!DNL Salesforce], haga clic en el icono de engranaje en la parte superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Haga clic en **[!UICONTROL Administrador de objetos]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Escriba &quot;[!UICONTROL Actividad]&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Haga clic en la etiqueta **[!UICONTROL Actividad]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Haga clic en **[!UICONTROL Campos y relaciones]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Agregar campo de actividad personalizado al diseño de página de tarea en [!DNL Salesforce] Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. En [!DNL Salesforce], haga clic en el icono de engranaje en la parte superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Haga clic en **[!UICONTROL Administrador de objetos]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Escriba &quot;[!UICONTROL Tarea]&quot; en el cuadro Búsqueda rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Haga clic en la etiqueta **[!UICONTROL Tarea]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Haga clic en **[!UICONTROL Diseños de página]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Haga clic en el diseño de página de la tarea al que desee agregar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Arrastre y suelte el campo en la sección deseada del diseño de página de la tarea.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Instalar campos de evento de Sales Connect en el historial de actividades](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
