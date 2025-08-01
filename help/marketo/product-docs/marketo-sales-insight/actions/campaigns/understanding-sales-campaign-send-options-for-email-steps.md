---
description: Explicación de las opciones de envío de campañas de ventas para pasos de correo electrónico - Documentos de Marketo - Documentación del producto
title: Explicación de las opciones de envío de campañas de ventas para pasos de correo electrónico
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 2%

---

# Explicación de las opciones de envío de campañas de ventas para pasos de correo electrónico {#understanding-sales-campaign-send-options-for-email-steps}

Al crear una campaña de ventas, tiene varias opciones sobre cómo se crean los pasos de correo electrónico en [!DNL Sales Insight Actions]. Y, dependiendo de dónde se encuentre su correo electrónico en la campaña de ventas, sus opciones también difieren.

## Opciones de envío del primer paso {#first-step-send-options}

Si es su primer paso y el primer día de su campaña de ventas, tendrá las siguientes opciones:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Elegiré cuándo enviar este correo electrónico {#first-step-i-will-choose}

* Esta opción le permite elegir la hora de envío en el primer correo electrónico de la campaña de ventas cuando esta se inicia añadiendo personas.

### Enviar este correo electrónico a la siguiente hora {#first-step-following-time}

* Cuando inicie su campaña de ventas agregando personas, programaremos el correo electrónico para este momento.
* Siempre tiene la opción de elegir una nueva hora de envío cuando inicie la campaña de ventas.

### Crear una tarea. Enviaré este email por mi cuenta {#first-step-create-a-task}

* Esta opción creará una tarea de correo electrónico (y la sincronizará con [!DNL Salesforce]) que podrá enviar según le convenga.
* Una vez que haya realizado esta selección, cuando inicie la campaña de ventas, pondremos en cola estas tareas en el Centro de comandos y en la Fuente en directo. A continuación, puede personalizar y enviar (o programar) cada correo electrónico antes de que se publique.

   * Si abre esta tarea en nuestra aplicación web, se abrirá una ventana de composición con la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.
   * Si abre esta tarea en Gmail o [!DNL Outlook], se abrirá una ventana de redacción nativa y se rellenará dinámicamente la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.

## Opciones de envío de pasos posteriores {#subsequent-step-send-options}

Para los días o pasos siguientes de la campaña de ventas, tiene las siguientes opciones:

### Envíe este correo electrónico al mismo tiempo que el correo electrónico anterior en esta campaña de ventas {#subsequent-send-at-same-time}

* Esta opción enviará el correo electrónico al mismo tiempo que el correo electrónico directamente antes de él.
* Se enviará el día en que esté asociado.

>[!IMPORTANT]
>
>El envío de un correo electrónico al mismo tiempo que el correo electrónico anterior no es compatible con los correos electrónicos enviados el mismo día. En su lugar, el correo electrónico se enviará en el momento del correo electrónico enviado el día anterior. Si se selecciona esta opción para un correo electrónico el primer día de la campaña (no recomendado), ese correo electrónico se envía inmediatamente al inicio de la campaña.

### Enviar este correo electrónico a la siguiente hora {#subsequent-send-at-following-time}

* Cuando inicie su campaña de ventas agregando personas, programaremos el correo electrónico para este momento.
* Siempre tiene la opción de elegir una nueva hora de envío cuando inicie la campaña de ventas.

### Crear una tarea. Enviaré este email por mi cuenta {#subsequent-create-a-task}

* Esta opción creará una tarea de correo electrónico (y la sincronizará con [!DNL Salesforce]) que podrá enviar según le convenga.
* Una vez que haya hecho esta selección, cuando inicie su campaña de ventas, [!DNL Sales Insight Actions] pondrá en cola estas tareas por usted en el Centro de comandos y en la Fuente en vivo. A continuación, puede personalizar y enviar (o programar) cada correo electrónico antes de que se publique.

   * Si abre esta tarea en nuestra aplicación web, se abrirá una ventana de composición con la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.
   * Si abre esta tarea en Gmail o [!DNL Outlook], se abrirá una ventana de redacción nativa y se rellenará dinámicamente la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.

### Cree este correo electrónico como seguimiento del correo electrónico anterior en esta campaña {#subsequent-create-this-email}

* Active esta casilla de verificación si desea que el correo electrónico anterior de la campaña de ventas se adjunte al siguiente correo electrónico que envía la campaña de ventas.
* Para la copia adjunta del correo electrónico, la plantilla de correo electrónico de la campaña de ventas siempre se envía. Las ediciones que el usuario haya realizado antes de enviarlo no se incluirán en el envío.

>[!NOTE]
>
>Esta opción para crear un correo electrónico como seguimiento solo estará disponible en un paso de correo electrónico, cuando el paso anterior también sea un correo electrónico. Si el paso anterior es Llamada, EnMail o Personalizado, la opción para crear un seguimiento no aparecerá.

>[!MORELIKETHIS]
>
>[Crear una campaña de ventas](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>&#x200B;>[Tipos de pasos de campañas de ventas y tareas de recordatorio](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>&#x200B;>[Configuración de campañas de ventas](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}

