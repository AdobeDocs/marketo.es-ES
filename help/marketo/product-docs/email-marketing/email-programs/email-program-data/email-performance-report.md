---
unique-page-id: 2359467
description: Informe Rendimiento del correo electrónico - Documentos de Marketo - Documentación del producto
title: Informe Rendimiento del correo electrónico
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 1%

---

# Informe Rendimiento del correo electrónico {#email-performance-report}

Para ver el rendimiento de los correos electrónicos con estadísticas como entregadas, abiertas, en las que se hace clic, etc., cree un informe de rendimiento de correo electrónico.

1. [Crear un informe en un programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) y seleccione **Rendimiento del correo electrónico** [Tipo de informe](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Cambio del intervalo de tiempo del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) y haga clic en el botón **Informe** pestaña .
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
   >Un informe de rendimiento de correo electrónico incluye actividades para todas las personas, incluidas las que se han eliminado desde que se envió el correo electrónico. A veces, solo desea ver las actividades para personas activas. En ese caso, debe filtrar las personas eliminadas del informe. Utilice la variable **Lista inteligente** para [crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para el informe. Si no está filtrando en ningún campo específico, establezca el filtro Dirección de correo electrónico en: **no está vacío**.

   [Seleccionar columnas de informes](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para un informe Rendimiento del correo electrónico, incluya:

   | Columna | Descripción |
   |---|---|
   | Se rechazó permanentemente | El correo electrónico se rechazó debido a una condición permanente, como una dirección de correo electrónico inexistente. |
   | Rechazado leve | El correo electrónico se rechazó debido a una condición temporal, como que un servidor estuviera inactivo o una bandeja de entrada completa. |
   | Pendiente | Este número se calcula restando el número de correos electrónicos entregados, devueltos y rechazados leves del número total de correos enviados. |
   | Vínculo en el que se hizo clic | Número de destinatarios de correo electrónico que hicieron clic en un vínculo del correo electrónico. |
   | Suscripción cancelada | Número de destinatarios de correo electrónico que hicieron clic en la variable **Cancelar suscripción** en el correo electrónico y rellenó el formulario. |

   >[!NOTE]
   >
   >Los vínculos de cancelación de suscripción y las direcciones de correo electrónico en los que se hace clic en un mensaje de correo electrónico no se registrarán en Vínculos en los que se hizo clic en el informe.

En general, tratamos de usar el sentido común para registrar estas estadísticas. Por ejemplo, si alguien hizo clic en un vínculo de un correo electrónico, obviamente lo abrió primero. Seguimos estas reglas específicas para el informe Rendimiento del correo electrónico:

* **Regla 1**: Cada registro de actividad de correo electrónico se establece en uno, y solo en uno, de los siguientes: _Entrega_, _Grave rechazado_, _Rechazado leve_ o _Pendiente_.

* **Regla 2**: Si se muestra el registro de correo electrónico *Abierto*, se cuenta como *Entrega*.

* **Regla 3**: Si se muestra el registro de correo electrónico _Correo electrónico en el que se hizo clic_ o _Cancelación de suscripción_, se cuenta como _Entrega_ y _Abierto_.

* **Regla 4**: Si el correo electrónico es _Abierto_, las devoluciones se ignoran. Si el correo electrónico no se ha abierto, _Grave rechazado_ tiene prioridad sobre _Rechazado leve_ y _Entrega_.

>[!NOTE]
>
>Los envíos múltiples desde la misma campaña a la misma persona se cuentan solo una vez.

>[!MORELIKETHIS]
>
>* [Filtrado de recursos en informes de correo electrónico de campaña](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Informe de rendimiento de los vínculos de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

