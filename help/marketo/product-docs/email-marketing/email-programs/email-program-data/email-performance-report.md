---
unique-page-id: 2359467
description: Informe Rendimiento del correo electrónico - Documentos de marketing - Documentación del producto
title: Informe de rendimiento de correo electrónico
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# Informe de rendimiento de correo electrónico {#email-performance-report}

Para ver el rendimiento de los mensajes de correo electrónico con estadísticas como entregados, abiertos, en los que se hizo clic, etc., cree un informe de rendimiento de correo electrónico.

1. [Cree un informe en un Programa](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) y seleccione el tipo **de** informe Rendimiento [de](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)correo electrónico.
1. [Cambie el intervalo](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) de tiempo del informe y haga clic en la ficha **Informe** .
1. ¡Estás ahí! Ahora explore el informe para ver el rendimiento de sus correos electrónicos.

   >[!NOTE]
   >
   >El filtro Fecha de envío se basa en la primera fecha en que se envió el correo electrónico.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Haga clic en el nombre de un correo electrónico para abrirlo en la vista previa de correo electrónico.

   >[!NOTE]
   >
   >
   >Un informe de rendimiento de correo electrónico incluye actividades para todas las personas, incluidas las que se han eliminado desde que se envió el correo electrónico. A veces, desea ver actividades solo para personas activas. En ese caso, debe filtrar las personas eliminadas del informe. Utilice la ficha Lista **** inteligente para [crear una lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) inteligente para el informe. Si no está filtrando ningún campo específico, establezca el filtro Dirección de correo electrónico en: **no está vacío**.

   [Las columnas](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) de informes seleccionadas para un informe de rendimiento de correo electrónico incluyen:

   | Columna | Descripción |
   |---|---|
   | Devuelto | El correo electrónico se rechazó debido a una condición permanente, como una dirección de correo electrónico inexistente. |
   | Suave devuelta | El correo electrónico se rechazó debido a una condición temporal, como un servidor que no funciona o una bandeja de entrada completa. |
   | Pendiente | Este número se calcula restando el número de correos electrónicos entregados, devueltos y no entregados del número total enviado. |
   | Vínculo en el que se hizo clic | Número de destinatarios de correo electrónico que hicieron clic en un vínculo del correo electrónico. |
   | No suscrito | Número de destinatarios de correo electrónico que hicieron clic en el vínculo **Cancelar suscripción** en el correo electrónico y rellenaron el formulario. |

   >[!NOTE]
   >
   >Los vínculos de cancelación de suscripciones y las direcciones de correo electrónico en las que se hace clic en un mensaje de correo electrónico no se registrarán en Vínculos en los que se hizo clic en el informe.

En general, tratamos de usar el sentido común para registrar estas estadísticas. Por ejemplo, si alguien hizo clic en un vínculo de un mensaje de correo electrónico, obviamente lo abrió primero. Seguimos estas reglas específicas para el informe Rendimiento del correo electrónico:

* **Artículo 1**: Cada registro de actividad de correo electrónico se establece en uno, y solo uno, de los siguientes valores: *Entregado*, *Abandonado* duro, Abandonado ** suave o *Pendiente*.

* **Artículo 2**: Si el registro de correo electrónico muestra *Abierto*, se cuenta como *Enviado*.

* **Artículo 3**: Si el registro de correo electrónico muestra Correo electrónico ** en el que se hizo clic o *Suscrito*, se cuenta como *Enviado* y *Abierto*.

* **Artículo 4**: Si el correo electrónico está *abierto*, se omiten las devoluciones. Si el correo electrónico no se ha abierto, la opción *Rebotado* tiene prioridad sobre *Rebotado* suave y *Enviado*.

>[!NOTE]
>
>Los envíos múltiples desde la misma campaña a la misma persona se cuentan sólo una vez.

>[!MORELIKETHIS]
>
>* [Filtrar recursos en informes de correo electrónico de Campaña](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Informe de rendimiento de vínculo de correo electrónico](email-link-performance-report.md)

>



>[!NOTE]
>
>**Buceo profundo**
>
>Obtenga más información en Sistema de informes [](http://docs.marketo.com/display/docs/basic+reporting)básico.

