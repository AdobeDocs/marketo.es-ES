---
unique-page-id: 2359467
description: Obtenga información sobre cómo crear y utilizar el informe Rendimiento de correo electrónico. Rastrear aperturas, clics, devoluciones y otras métricas de correo electrónico.
title: Informe de rendimiento de los correos electrónicos
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 95%

---

# Informe de rendimiento de los correos electrónicos {#email-performance-report}

Para ver el rendimiento de los correos electrónicos con estadísticas como enviados, abiertos, hechos clic, etc., cree un informe de rendimiento de correo electrónico.

1. [Cree un informe en un programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) y seleccione **[!UICONTROL Rendimiento de correo electrónico]** [Tipo de informe](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Cambie el lapso de tiempo del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) y haga clic en la pestaña **[!UICONTROL Informe]**.
1. ¡Estás ahí! Ahora explore el informe para ver el rendimiento de sus correos electrónicos.

   >[!NOTE]
   >
   >El filtro Fecha de envío se basa en la primera fecha en que se envió el correo electrónico.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Haga clic en el nombre de un correo electrónico para abrirlo en la vista previa del correo electrónico.

   >[!NOTE]
   >
   >Un informe de rendimiento de correo electrónico incluye actividades para todas las personas, incluidas las que se han eliminado desde que se envió el correo electrónico. A veces, es posible que solo desee ver las actividades de personas activas. En ese caso, debe filtrar las personas eliminadas para excluirlas del informe. Use la pestaña **[!UICONTROL Lista inteligente]** para [crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para el informe. Si no está aplicando un filtro por un campo específico, establezca el filtro Dirección de correo electrónico en: **[!UICONTROL no está vacío]**.

   [La seleccion de columnas del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para un informe de rendimiento de correo electrónico incluye lo siguiente:

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
    <td>Este número se calcula restando el número de correos electrónicos entregados, rechazados y rechazados temporalmente del número total de enviados.</td>
  </tr>
  <tr>
    <td>Se hizo clic en el vínculo</td>
    <td>Número de destinatarios del correo electrónico que hicieron clic en el vínculo incluido en él.</td>
  </tr>
  <tr>
    <td>Suscripción cancelada</td>
    <td>Número de destinatarios de correo electrónico que hicieron clic en el vínculo Cancelar suscripción del correo electrónico y rellenaron el formulario.</td>
  </tr>
  <tr>
    <td>Anulado</td>
    <td>Número de correos electrónicos que no se pudieron entregar y de los que no se recibió ningún evento de rechazo. Un correo electrónico se clasifica automáticamente como Anulado si no se recibe una respuesta en un plazo de tres días desde el envío del correo electrónico.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Los vínculos de cancelación de suscripción y las direcciones de correo electrónico en los que se haga clic en un correo electrónico no se registrarán como Vínculos en los que se hizo clic en el informe.

En general, tratamos de usar el sentido común para registrar estas estadísticas. Por ejemplo, si alguien hace clic en un vínculo de un correo electrónico, es evidente que primero tuvieron que abrir el correo electrónico. Seguimos estas reglas específicas para el informe de rendimiento de correo electrónico:

* **Regla 1**: cada registro de actividad de correo electrónico se establece en uno, y solo uno, de los siguientes: _Entregado_, _Rechazado permanentemente_, _Rechazado temporalmente_ o _Pendiente_.

* **Regla 2**: si el registro de correo electrónico muestra _[!UICONTROL Abierto]_, se cuenta como _Entregado_.

* **Regla 3**: si el registro de correo electrónico muestra _[!UICONTROL Correo electrónico en el que se ha hecho clic]_ o _[!UICONTROL Suscripción cancelada]_, se cuenta como _Entregado_ y _Abierto_.

* **Regla 4**: si el correo electrónico consta como _[!UICONTROL Abierto]_, se ignoran los rechazos. Si el correo electrónico no se ha abierto, _Rechazado permanentemente_ tiene prioridad sobre _Rechazado temporalmente_ y _Entregado_.

* **Regla 5**: si no se recibe ninguna actividad de correo electrónico en los tres días posteriores a su envío, se considera como _Anulado_.

>[!NOTE]
>
>* Varios envíos de la misma campaña a la misma persona se cuentan solo una vez.
>
>* Varios envíos de diferentes campañas a la misma persona se cuentan por separado.

>[!MORELIKETHIS]
>
>* [Filtrar recursos en informes por correo electrónico de campaña](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrar registros eliminados o combinados en un informe de rendimiento de correo electrónico](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Informe de rendimiento de vínculos de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
