---
unique-page-id: 13795727
description: Anular la entrega de programas de correo electrónico programados con el huso horario del destinatario - Marketo Docs - Documentación del producto
title: Anular la entrega de programas de correo electrónico programados con el huso horario del destinatario
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Anular la entrega de programas de correo electrónico programados con el huso horario del destinatario {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

En casos de emergencia, puede anular la entrega de un programa de correo electrónico que ya se haya empezado a ejecutar con la zona horaria del destinatario habilitada.

Dado que los programas de correo electrónico programados con la zona horaria del destinatario pueden ejecutarse durante un máximo de 24 horas, al cancelar la entrega del programa se cancelarán los envíos subsiguientes después de ese punto.

1. Seleccione el programa de correo electrónico que desea cancelar y haga clic en **Anular entrega** en el mosaico Aprobación del panel de control.

   ![](assets/ptz-abortdelivery.png)

1. Confirme que desea cancelar la entrega haciendo clic en **Anular**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Tras la cancelación, la variable **Resultados** de su programa de correo electrónico se parecerá a la de abajo. Los envíos subsiguientes se cancelan y se mostrarán como &quot;Correo electrónico rechazado leve&quot; en la variable **Tipo de actividad** para abrir el Navegador.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Los correos electrónicos cancelados **not** mostrar como un rebote suave *hasta* la hora a la que se programó originalmente para enviarse en sus respectivas zonas horarias. Hasta ese momento, se mostrarán como &quot;Enviar correo electrónico&quot;.

1. Desde la cuadrícula, puede hacer clic en cualquier correo electrónico para ver los detalles de la actividad. Para un envío cancelado, la ventana emergente de detalles tendrá este aspecto:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Programar programas de correo electrónico con la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

