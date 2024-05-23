---
unique-page-id: 2359476
description: Uso del tablero del programa de correo electrónico - Documentos de Marketo - Documentación del producto
title: Uso del panel del programa de correo electrónico
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: b2ceefb068005d916027fb71be0dc4e25849ae23
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Uso del panel del programa de correo electrónico {#use-the-email-program-dashboard}

Consulte el rendimiento de sus programas de correo electrónico con esta vista de panel.

>[!CAUTION]
>
>Para obtener un informe preciso, evite _reutilización_ Cree un correo electrónico desde un programa de correo electrónico, ya sea haciendo referencia a él en una campaña inteligente o moviendo el recurso del programa de correo electrónico iniciado a uno nuevo. Al hacerlo, se acumulan todos los datos en cada panel de informes adjunto a ese correo electrónico. Si necesita reutilizar un correo electrónico, [clónelo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"} en su lugar, ya que copia el correo electrónico, pero crea uno nuevo con un nuevo ID de correo electrónico.

>[!NOTE]
>
>Si su programa tiene una prueba A/B, consulte la [Panel del programa de correo electrónico - Vista de prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}.

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>Todos los datos de esta vista son acumulados (incluye la prueba A/B y el envío final por correo electrónico).

## Enviar email {#email-send}

Aquí puede ver cuántos correos electrónicos se enviaron, rechazados y entregados.

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>Debido a los estándares de entrega de correo electrónico que están fuera del control de Marketo, las estadísticas de rechazos y entregas son aproximadas, no exactas.

## Aperturas/Clics {#opens-clicks}

Este gráfico muestra el número de correos electrónicos abiertos o en los que se hizo clic durante períodos de tiempo específicos después de ejecutar el programa de correo electrónico.

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>Observe cómo el número de aperturas/clics disminuye con el paso del tiempo.

## Resumen - Participación {#summary-engagement}

Esto le muestra el total [puntuación de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

![](assets/image2014-9-12-14-3a13-3a11.png)

## Resumen - Resto {#summary-rest}

El resto de los datos se muestran como Aperturas, Clics, Proporción de clics/aperturas y Cancelaciones de suscripción.

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>El **Cancelar suscripción** La tasa del ejemplo anterior era tan pequeña que Marketo amplió para ofrecerle un mejor aspecto. El segundo número dentro de la barra simplemente se agrega para escalar.

>[!NOTE]
>
>**Definición**
>
>**Aperturas** se cuentan cuando el destinatario del correo electrónico descarga las imágenes del correo electrónico, lo que incluye un píxel de seguimiento insertado en Marketo. Si el destinatario ve el correo electrónico pero decide no descargar sus imágenes, no se contará como una apertura. Si las imágenes se cargan en el panel de vista previa del destinatario, generalmente se contará como una apertura, pero variará según el cliente de correo electrónico.
>
>**Haga clic para abrir** mide el porcentaje de correos electrónicos que se abrieron y en los que se hizo clic en un vínculo. Tomamos el número de clics únicos dividido por el número de aperturas únicas y luego lo multiplicamos por 100 para mostrarlo como un porcentaje.

## Actualizar panel {#refresh-dashboard}

Para ver los datos más actualizados, simplemente haga clic en el icono de actualización del panel.

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[Uso del panel del programa de correo electrónico: vista de prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
