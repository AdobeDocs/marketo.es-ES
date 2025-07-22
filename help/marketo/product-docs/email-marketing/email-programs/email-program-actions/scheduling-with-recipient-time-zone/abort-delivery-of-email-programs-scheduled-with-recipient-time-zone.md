---
unique-page-id: 13795727
description: Anular la entrega de programas de correo electrónico programados con la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Anular la entrega de programas de correo electrónico programados con la zona horaria del destinatario
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Anular la entrega de programas de correo electrónico programados con la zona horaria del destinatario {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

En casos de emergencia, puede cancelar la entrega de un programa de correo electrónico que ya haya comenzado a ejecutarse con la zona horaria del destinatario habilitada.

Dado que los programas de correo electrónico programados con la zona horaria del destinatario pueden ejecutarse durante un máximo de 24 horas, al cancelar la entrega del programa se cancelarán los envíos posteriores a ese punto.

1. Seleccione el programa de correo electrónico que desea cancelar y, a continuación, haga clic en **[!UICONTROL Anular entrega]** en el mosaico [!UICONTROL Aprobación] del panel de control.

   ![](assets/ptz-abortdelivery.png)

1. Confirme que desea cancelar la entrega haciendo clic en **[!UICONTROL Anular]**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Después de la cancelación, la cuadrícula de **[!UICONTROL Resultados]** de tu programa de correo electrónico se parecerá a la de abajo. Los envíos subsiguientes se cancelarán y se mostrarán como &quot;Correo electrónico rechazado suave&quot; en la columna **[!UICONTROL Tipo de actividad]**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Los correos electrónicos cancelados **no** se mostrarán como mensajes devueltos no entregados *hasta* la hora en que se programó originalmente que se enviaran en sus respectivos husos horarios. Hasta ese momento, se seguirán mostrando como &quot;Enviar correo electrónico&quot;.

1. Desde la cuadrícula, puede hacer clic en cualquier correo electrónico para ver los detalles de la actividad. Para un envío cancelado, la ventana emergente de detalles tendrá este aspecto:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Programar programas de correo electrónico con zona horaria de destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
