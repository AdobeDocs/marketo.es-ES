---
unique-page-id: 7505310
description: Suscripción a una lista inteligente - Documentos de Marketo - Documentación del producto
title: Suscripción a una lista inteligente
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# Suscripción a una lista inteligente {#subscribe-to-a-smart-list}

La suscripción a listas inteligentes es una buena forma de realizar un seguimiento de las personas, y los informes se envían directamente a la bandeja de entrada.

Puede crear una suscripción a una lista inteligente en dos lugares independientes:

* Actividades de marketing
* Base de datos

Las suscripciones utilizan la lista completa de personas en el momento en que se ejecuta la suscripción.

Las suscripciones están activas donde se encuentra la lista inteligente, en las actividades de marketing o en la base de datos.

Puede crear varias suscripciones desde la misma lista inteligente.

Las suscripciones son específicas del espacio de trabajo. Por ejemplo, esta lista de suscripciones se encuentra en un espacio de trabajo diferente de los que se muestran en el resto de este artículo:

![](assets/one.png)

>[!NOTE]
>
>Está limitado a 100 suscripciones y a un máximo de 100 000 personas por suscripción, entre espacios de trabajo y por instancia de Marketo. Si la lista inteligente contiene más de 100 000 nombres, Marketo ejecutará la suscripción durante los primeros 100 000.

## Crear una suscripción a una lista inteligente {#create-a-smart-list-subscription}

1. Vaya a la **Base de datos** o **Actividades de marketing**.

   ![](assets/db.png)

1. Seleccione la lista inteligente para la que desea crear una suscripción. Haga clic en **Acciones de lista** y seleccione **Nueva suscripción a listas inteligentes**.

   ![](assets/three.png)

1. Asigne una suscripción a **Nombre** y, a continuación, seleccione o introduzca las direcciones de correo electrónico del **Destinatarios**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Haga clic en el **Frecuencia** y seleccione una frecuencia.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Configure las variables **Finalizar entrega** fecha. Puede seleccionar **Nunca** o una fecha de calendario.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Haga clic en **Formato** y seleccione en la lista.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Haga clic en **Crear**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. La nueva suscripción a la lista inteligente aparece en la parte superior de la lista, en la pestaña Subscriptions . Haga clic en **Enviar** si desea enviar ahora y no esperar hasta el envío de correo electrónico programado.

   ![](assets/eight.png)

1. Se recomienda desactivar la casilla de verificación Activo para desactivar una suscripción a una lista inteligente si nadie está suscrito a ella.

   ![](assets/nine.png)

   Eso fue fácil, ¿no?

## Mensaje de correo electrónico {#email-message}

Los destinatarios recibirán un correo electrónico con una opción para descargar el informe, así como un vínculo directamente a la lista dentro de la instancia de Marketo. El vínculo de descarga caduca en cuatro días.

>[!NOTE]
>
>Si la variable [Administrador de suscripciones seguro](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) está configurada en **Sí**, solo las personas con acceso a la instancia de Marketo podrán descargar el informe.

![](assets/image2015-4-17-15-3a46-3a47.png)

Si un informe tiene 0 personas, los destinatarios seguirán recibiendo un correo electrónico. Sin embargo, el correo electrónico simplemente indica que no hay personas para informar.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Al modificar un filtro de lista inteligente en el que ha basado una suscripción, también se actualiza el informe.

El correo electrónico también proporciona información adicional sobre los filtros utilizados para crear la lista.

## Eliminar una suscripción {#delete-a-subscription}

Para eliminar una suscripción, selecciónela en la pestaña suscripciones y haga clic en Eliminar suscripción.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Editar una suscripción a una lista inteligente](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Asegurar la configuración del administrador de suscripciones](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)

