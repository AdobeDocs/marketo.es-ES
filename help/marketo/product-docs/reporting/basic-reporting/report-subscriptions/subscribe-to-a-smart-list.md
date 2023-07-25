---
unique-page-id: 7505310
description: 'Suscripción a una lista inteligente: documentos de Marketo, documentación del producto'
title: Suscripción a una lista inteligente
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# Suscripción a una lista inteligente {#subscribe-to-a-smart-list}

La suscripción a listas inteligentes es una buena manera de realizar un seguimiento de las personas, con informes enviados directamente a la bandeja de entrada.

Puede crear una suscripción a una lista inteligente en dos lugares independientes:

* Actividades de marketing
* Base de datos

Las suscripciones utilizan la lista completa de personas en el momento en que se ejecuta la suscripción.

Las suscripciones se almacenan donde se encuentra su lista inteligente, en las actividades de marketing o en la base de datos.

Puede crear varias suscripciones a partir de la misma lista inteligente.

Las suscripciones son específicas de Workspace. Por ejemplo, esta lista de suscripciones está en un espacio de trabajo diferente de las que se muestran en el resto de este artículo:

![](assets/one.png)

>[!NOTE]
>
>Tiene un límite de 100 suscripciones y un máximo de 100 000 personas por suscripción, en espacios de trabajo y por instancia de Marketo. Si la lista inteligente contiene más de 100 000 nombres, Marketo ejecutará la suscripción para los primeros 100 000.

## Crear una suscripción a una lista inteligente {#create-a-smart-list-subscription}

1. Vaya a la **Base de datos** o **Actividades de marketing**.

   ![](assets/db.png)

1. Seleccione la lista inteligente para la que desea crear una suscripción. Clic **Enumerar acciones** y seleccione **Nueva suscripción a lista inteligente**.

   ![](assets/three.png)

1. Asigne un a su suscripción **Nombre**, luego seleccione o introduzca las direcciones de correo electrónico del **Destinatarios**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Haga clic en **Frecuencia** y seleccione una frecuencia.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Configure las variables **Finalizar envío** fecha. Puede seleccionar **Nunca** o una fecha de calendario.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Clic **Formato** y elija en la lista.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Haga clic en **Crear**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. La nueva suscripción a la lista inteligente aparece en la parte superior de la lista de la pestaña Suscripciones. Clic **Enviar** si desea realizar el envío ahora y no esperar hasta la entrega de correo electrónico programada.

   ![](assets/eight.png)

1. Se recomienda desactivar la casilla de verificación Activo para desactivar una suscripción a una lista inteligente si nadie está suscrito a ella.

   ![](assets/nine.png)

   Eso fue fácil, ¿no?

## Mensaje de correo electrónico {#email-message}

Los destinatarios recibirán un correo electrónico con una opción para descargar el informe, así como un vínculo directamente a la lista dentro de la instancia de Marketo. El vínculo de descarga caduca en cuatro días.

>[!NOTE]
>
>Si la variable [Administrador de suscripción segura](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) se establece en **Sí**, solo las personas con acceso a la instancia de Marketo podrán descargar el informe.

![](assets/image2015-4-17-15-3a46-3a47.png)

Si un informe no contiene ninguna persona, los destinatarios seguirán recibiendo un correo electrónico. Sin embargo, el correo electrónico simplemente indica que no hay personas de las que informar.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Al modificar un filtro de lista inteligente en el que se basa una suscripción, también se actualiza el informe.

El correo electrónico también proporciona información adicional sobre los filtros utilizados para crear la lista.

## Eliminar una suscripción {#delete-a-subscription}

Para eliminar una suscripción, selecciónela en la pestaña Subscriptions y haga clic en Delete Subscription.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Editar una suscripción a una lista inteligente](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Protección de la configuración de administración de suscripciones](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
