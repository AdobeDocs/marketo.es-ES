---
unique-page-id: 2359467
description: Informe de rendimiento de correo electrónico - Documentos de Marketo - Documentación del producto
title: Informe de rendimiento de correo electrónico
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 6133a04124d9d4b829d092943753c7bb530dd374
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 2%

---

# Informe de rendimiento de correo electrónico {#email-performance-report}

Para ver el rendimiento de los correos electrónicos con estadísticas como enviado, abierto, hecho clic, etc., cree un informe de rendimiento de correo electrónico.

1. [Cree un informe en un programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) y seleccione **Rendimiento de correo electrónico** [Tipo de informe](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Cambie el intervalo de tiempo del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) y haga clic en la ficha **Informe**.
1. ¡Tú estás ahí! Ahora explore el informe para ver el rendimiento de sus correos electrónicos.

   >[!NOTE]
   >
   >El filtro Fecha de envío se basa en la primera fecha en que se envió el correo electrónico.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Haga clic en el nombre de un correo electrónico para abrirlo en el previsualizador de correo electrónico.

   >[!NOTE]
   >
   >Un informe de rendimiento de correo electrónico incluye actividades para todas las personas, incluidas las que se han eliminado desde que se envió el correo electrónico. A veces, desea ver actividades solo para personas activas. En ese caso, debe filtrar las personas eliminadas para que no estén en el informe. Use la ficha **Lista inteligente** para [crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para el informe. Si no está filtrando en ningún campo específico, establezca el filtro Dirección de correo electrónico en: **no está vacío**.

   [Seleccionar columnas de informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para un informe de rendimiento de correo electrónico incluye:

   <table><thead>
<tr>
    <th>Columna</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Se rechazó permanentemente</td>
    <td>El correo electrónico se rechazó debido a una condición permanente, como una dirección de correo electrónico inexistente.</td>
  </tr>
  <tr>
    <td>Rechazado temporalmente</td>
    <td>El correo electrónico se rechazó debido a una condición temporal, como que un servidor esté inactivo o que la bandeja de entrada esté llena.</td>
  </tr>
  <tr>
    <td>Pendiente</td>
    <td>Este número se calcula restando el número de correos electrónicos entregados, rechazados y rechazados en blanco del número total de enviados.</td>
  </tr>
  <tr>
    <td>Se hizo clic en el vínculo</td>
    <td>Número de destinatarios de correo electrónico que hicieron clic en un vínculo del correo electrónico.</td>
  </tr>
  <tr>
    <td>Suscripción cancelada</td>
    <td>Número de destinatarios de correo electrónico que hicieron clic en el vínculo Cancelar suscripción del correo electrónico y rellenaron el formulario.</td>
  </tr>
  <tr>
    <td>Anulado</td>
    <td>Número de correos electrónicos que no se pudieron enviar y que no se recibió ningún evento de devolución. Un correo electrónico se denomina automáticamente Anulado si no se recibe una respuesta en un plazo de tres días a partir del envío del correo electrónico.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Los vínculos de cancelación de suscripción y las direcciones de correo electrónico en las que se haga clic en un correo electrónico no se registrarán como Vínculos en los que se hizo clic en el informe.

En general, tratamos de usar el sentido común para registrar estas estadísticas. Por ejemplo, si alguien hace clic en un vínculo de un correo electrónico, obviamente, abre primero el correo electrónico. Seguimos estas reglas específicas para el informe de rendimiento de correo electrónico:

* **Regla 1**: Cada registro de actividad de correo electrónico se establece en uno y solo en uno de los siguientes: _Entregado_, _Rebote duro_, _Rebote suave_ o _Pendiente_.

* **Regla 2**: Si el registro de correo electrónico muestra *Abierta*, se cuenta como *Entregada*.

* **Regla 3**: Si el registro de correo electrónico muestra _Correo electrónico en el que se hizo clic_ o _Se canceló la suscripción_, se cuenta como _Entregado_ y _Abierto_.

* **Regla 4**: Si el correo electrónico es _Abierto_, se omiten las devoluciones. Si el correo electrónico no se ha abierto, _Devuelto fuerte_ tiene prioridad sobre _Devuelto leve_ y _Entregado_.

* **Regla 5**: Si no se recibe ninguna actividad de correo electrónico tres días después de su envío, se considera _Anulada_.

>[!NOTE]
>
>* Varios envíos de la misma campaña a la misma persona se cuentan solo una vez.
>
>* Los envíos múltiples de diferentes campañas a la misma persona se cuentan por separado.

>[!MORELIKETHIS]
>
>* [Filtrar Assets en los informes de correo electrónico de Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrar registros eliminados o combinados en un informe de rendimiento de correo electrónico](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Informe de rendimiento de vínculos de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
