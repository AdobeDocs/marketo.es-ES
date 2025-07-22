---
unique-page-id: 2360407
description: Creación de un informe de análisis de correo electrónico que enumere los posibles clientes - Documentos de Marketo - Documentación del producto
title: Crear un informe de análisis de correo electrónico que enumere los posibles clientes
exl-id: f431610c-6570-4df0-9d64-d37d21010604
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Crear un informe de análisis de correo electrónico que enumere los posibles clientes {#build-an-email-analysis-report-that-lists-leads}

Siga estos pasos para crear un informe de análisis de correo electrónico que le mostrará todos los posibles clientes a los que se ha enviado un mensaje de correo electrónico específico. Este informe también incluirá las estadísticas de Clics y Aperturas.

>[!AVAILABILITY]
>
>No todos han comprado esta función. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>El motor de datos que respalda el análisis de correo electrónico de RCA ignora los más de 12 clics por persona si proceden del mismo correo electrónico y campaña. Tenga esto en cuenta al comparar los informes de análisis de correo electrónico con los informes estándar de Marketo Analytics.

1. Iniciar **[!UICONTROL Explorador de ingresos]**.

   ![](assets/report-that-lists-leads-1.png)

1. Haga clic en **[!UICONTROL Crear nuevo]** y luego en **[!UICONTROL Informe]**.

   ![](assets/report-that-lists-leads-2.png)

1. Seleccione **[!UICONTROL Email Analysis]** y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/report-that-lists-leads-3.png)

1. Busque el punto amarillo de **[!UICONTROL Nombre de correo electrónico]**, haga clic con el botón derecho y seleccione **[!UICONTROL Filtrar...]**.

   ![](assets/report-that-lists-leads-4.png)

1. Haga doble clic en el correo electrónico que desee en la lista y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/report-that-lists-leads-5.png)

1. Arrastre el punto amarillo **[!UICONTROL Email Name]** a **[!UICONTROL Columns]**.

   ![](assets/report-that-lists-leads-6.png)

   >[!TIP]
   >
   >Hay muchos atributos de cliente potencial/empresa que puede agregar como columnas, compruébelos.

1. Busque el punto amarillo **[!UICONTROL Nombre completo]** y arrástrelo a **[!UICONTROL Filas]**.

   ![](assets/report-that-lists-leads-7.png)

1. Ahora agregue las **[!UICONTROL Medidas]** que le interesan haciendo doble clic en ellas.

   ![](assets/report-that-lists-leads-8.png)

>[!NOTE]
>
>En función de la cantidad de datos que tenga, este informe puede tardar unos minutos en actualizarse.

¡Misión completa!
