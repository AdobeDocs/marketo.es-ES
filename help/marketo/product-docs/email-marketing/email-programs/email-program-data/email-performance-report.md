---
unique-page-id: 2359467
description: Informe de rendimiento de correo electrónico - Documentos de Marketo - Documentación del producto
title: Informe de rendimiento de correo electrónico
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 1%

---

# Informe de rendimiento de correo electrónico {#email-performance-report}

Para ver el rendimiento de los correos electrónicos con estadísticas como enviado, abierto, hecho clic, etc., cree un informe de rendimiento de correo electrónico.

1. [Creación de un informe en un programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) y seleccione la **Rendimiento de correo electrónico** [Tipo de informe](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Cambio del intervalo de tiempo del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) y haga clic en **Informe** pestaña.
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
   >Un informe de rendimiento de correo electrónico incluye actividades para todas las personas, incluidas las que se han eliminado desde que se envió el correo electrónico. A veces, desea ver actividades solo para personas activas. En ese caso, debe filtrar las personas eliminadas para que no estén en el informe. Utilice el **Lista inteligente** pestaña a [crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para el informe. Si no está filtrando en ningún campo específico, establezca el filtro Dirección de correo electrónico en: **is not empty**.

   [Seleccionar columnas del informe](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) Para un informe de rendimiento de correo electrónico, incluya:

   | Columna | Descripción |
   |---|---|
   | Se rechazó permanentemente | El correo electrónico se rechazó debido a una condición permanente, como una dirección de correo electrónico inexistente. |
   | Rechazado suave | El correo electrónico se rechazó debido a una condición temporal, como que un servidor esté inactivo o que la bandeja de entrada esté llena. |
   | Pendiente | Este número se calcula restando el número de correos electrónicos entregados, rechazados y rechazados en blanco del número total de enviados. |
   | Vínculo en el que se hizo clic | Número de destinatarios de correo electrónico que hicieron clic en un vínculo del correo electrónico. |
   | Suscripción cancelada | Número de destinatarios de correo electrónico que hicieron clic en **Cancelar suscripción** vínculo en el correo electrónico y rellene el formulario. |

   >[!NOTE]
   >
   >Los vínculos de cancelación de suscripción y las direcciones de correo electrónico en las que se haga clic en un correo electrónico no se registrarán como Vínculos en los que se hizo clic en el informe.

En general, tratamos de usar el sentido común para registrar estas estadísticas. Por ejemplo, si alguien hace clic en un vínculo de un correo electrónico, obviamente, abre primero el correo electrónico. Seguimos estas reglas específicas para el informe de rendimiento de correo electrónico:

* **Regla 1**: cada registro de actividad de correo electrónico se establece en uno y solo en uno de los siguientes: _Entregado_, _Rechazado duro_, _Rechazado suave_, o _Pendiente_.

* **Regla 2**: Si se muestra el registro de correo electrónico *Abierto*, se cuenta como *Entregado*.

* **Regla 3**: Si se muestra el registro de correo electrónico _Correo electrónico clicado_ o _Cancelado_, se cuenta como _Entregado_ y _Abierto_.

* **Regla 4**: Si el correo electrónico es _Abierto_, las devoluciones se ignoran. Si no se ha abierto el correo electrónico, _Rechazado duro_ tiene prioridad sobre _Rechazado suave_ y _Entregado_.

>[!NOTE]
>
>Varios envíos de la misma campaña a la misma persona se cuentan solo una vez.

>[!MORELIKETHIS]
>
>* [Filtrado de recursos en informes de correo electrónico de Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Informe de rendimiento del vínculo de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
