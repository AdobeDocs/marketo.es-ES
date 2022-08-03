---
unique-page-id: 2360407
description: 'Creación de un informe de análisis de correo electrónico que enumere posibles clientes: Documentos de Marketo: Documentación del producto'
title: Creación de un informe de análisis de correo electrónico que enumere los posibles clientes
exl-id: f431610c-6570-4df0-9d64-d37d21010604
source-git-commit: 62f46579b9275f30938b9c57e7fb98ca6dca0ae1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creación de un informe de análisis de correo electrónico que enumere los posibles clientes {#build-an-email-analysis-report-that-lists-leads}

Siga estos pasos para crear un informe de análisis de correo electrónico que le muestre todos los posibles clientes a los que se ha enviado un correo electrónico específico. Este informe también incluirá las estadísticas de clics y aperturas.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con el administrador de éxito del cliente para obtener más información.

>[!NOTE]
>
>El motor de datos que respalda el análisis de correo electrónico RCA ignora los buenos 12 clics por persona si proceden del mismo correo electrónico y campaña. Tenga esto en cuenta al comparar los informes de análisis de correo electrónico con los informes estándar de Marketo Analytics.

1. Launch **Explorador de ingresos**.

   ![](assets/report-that-lists-leads-1.png)

1. Haga clic en **Crear nuevo** then **Informe**.

   ![](assets/report-that-lists-leads-2.png)

1. Seleccione Análisis de correo electrónico y haga clic en **OK**.

   ![](assets/report-that-lists-leads-3.png)

1. Busque el punto amarillo Nombre del correo electrónico, haga clic con el botón derecho en él y seleccione **Filtro**.

   ![](assets/report-that-lists-leads-4.png)

1. Haga doble clic en el correo electrónico de su elección en la lista y haga clic en **OK**.

   ![](assets/report-that-lists-leads-5.png)

1. Arrastre el **Nombre del correo electrónico** punto amarillo a **Columnas**.

   ![](assets/report-that-lists-leads-6.png)

   >[!TIP]
   >
   >Hay muchos atributos de cliente o empresa que puede agregar como columnas, ¡desprotéjelas!

1. Busque la **Nombre completo** punto amarillo y arrástrelo a **Filas**.

   ![](assets/report-that-lists-leads-7.png)

1. Ahora, agregue la variable **Medidas** le interesa hacer doble clic en ellos.

   ![](assets/report-that-lists-leads-8.png)

>[!NOTE]
>
>En función de la cantidad de datos que tenga, este informe podría tardar un rato en actualizarse.

¡Misión completa!
