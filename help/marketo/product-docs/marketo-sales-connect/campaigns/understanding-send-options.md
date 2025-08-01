---
unique-page-id: 14352621
description: 'Explicación de las opciones de envío: documentos de Marketo, documentación del producto'
title: Descripción de opciones de envío
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Descripción de opciones de envío {#understanding-send-options}

Al crear una campaña, tiene varias opciones sobre cómo se crean los pasos del correo electrónico en [!DNL Sales Connect]. Y, según dónde se encuentre el correo electrónico en la campaña, las opciones también difieren.

Si es el primer paso y el primer día de la campaña, tiene las siguientes opciones:

![](assets/image2019-10-25-10-43-19.png)

**Elegiré cuándo enviar este correo electrónico**

* Esta opción le permite elegir el momento &quot;enviar a las&quot; para el primer correo electrónico de la campaña cuando esta se inicia añadiendo personas.

**Enviar este correo electrónico a la siguiente hora**

* Cuando inicie su campaña añadiendo personas a ella, programaremos el correo electrónico para esta hora.
* Siempre tiene la opción de elegir un nuevo momento &quot;Enviar a las&quot; al iniciar la campaña.

**Crear una tarea; yo mismo enviaré este correo electrónico**

* Esta opción creará una [!UICONTROL tarea de correo electrónico] (y se sincronizará con [!DNL Salesforce]) que podrá enviar según le convenga.
* Una vez que haya realizado esta selección, cuando inicie la campaña, pondremos en cola estas tareas en el Centro de comandos y en la Fuente en directo. A continuación, puede personalizar y enviar (o programar) cada correo electrónico antes de que se publique.

   * Si abre esta tarea en nuestra aplicación web, se abrirá una ventana de composición con la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.
   * Si abre esta tarea en [!DNL Gmail] o [!DNL Outlook], se abrirá una ventana de redacción nativa y se rellenará dinámicamente la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.

Para cualquier día o paso posterior de la campaña, tendrá las siguientes opciones:

**Envíe este correo electrónico al mismo tiempo que el anterior en esta campaña**

* Esta opción enviará el correo electrónico al mismo tiempo que el correo electrónico directamente antes de él.
* Se enviará el día en que esté asociado.

>[!IMPORTANT]
>
>El envío de un correo electrónico al mismo tiempo que el correo electrónico anterior no es compatible con los correos electrónicos enviados el mismo día. En su lugar, el correo electrónico se enviará en el momento del correo electrónico enviado el día anterior. Si se selecciona esta opción para un correo electrónico el primer día de la campaña (no recomendado), ese correo electrónico se envía inmediatamente al inicio de la campaña.

**Enviar este correo electrónico a la siguiente hora**

* Cuando inicie su campaña añadiendo personas a ella, programaremos el correo electrónico para esta hora.
* Siempre tiene la opción de elegir un nuevo momento &quot;Enviar a las&quot; al iniciar la campaña.

**Crear una tarea; yo mismo enviaré este correo electrónico**

* Esta opción creará una [!UICONTROL tarea de correo electrónico] (y se sincronizará con [!DNL Salesforce]) que podrá enviar según le convenga.
* Una vez que haya hecho esta selección, cuando inicie la campaña, Tout pondrá en cola estas tareas por usted en el Centro de comandos y en la Fuente en directo. A continuación, puede personalizar y enviar (o programar) cada correo electrónico antes de que se publique.

   * Si abre esta tarea en nuestra aplicación web, se abrirá una ventana de composición con la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.
   * Si abre esta tarea en [!DNL Gmail] o [!DNL Outlook], se abrirá una ventana de redacción nativa y se rellenará dinámicamente la dirección de correo electrónico del contacto, la línea de asunto del correo electrónico y la plantilla que haya elegido.

**Enviar este correo electrónico al correo electrónico anterior**

* Esta opción de envío es un &quot;seguimiento&quot; del correo electrónico anterior y adjunta el cuerpo del correo electrónico anterior al final de este correo electrónico.

