---
unique-page-id: 14746177
description: 'Suscripción de una cancelación de suscripción: Documentos de Marketo: Documentación del producto'
title: Volver a suscribirse
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Volver a suscribirse {#resubscribing-an-unsubscribe}

A veces, las personas desean volver a recibir correos electrónicos. A continuación se explica cómo volver a enviar las cancelaciones de suscripción.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!CAUTION]
>
>Antes de volver a suscribirse a alguien, debe poder demostrar que la autorización para volver a suscribirlos está documentada y que cumple con todas las leyes aplicables.

>[!NOTE]
>
>Si tiene activada la sincronización de cancelación de suscripción, debe eliminar la cancelación de suscripción de ToutApp y desmarcar la opción de exclusión en Salesforce para que el registro de persona no se sincronice de nuevo.

1. Vaya a la [aplicación web](https://toutapp.com/login) y haga clic en **People**.

1. Seleccione la persona para abrir la vista de detalles de la persona.

   ![](assets/two.png)

1. Haga clic en los tres puntos de la vista de detalles de la persona y seleccione **Eliminar cancelación de suscripción**.

   ![](assets/three.png)

1. Seleccione el motivo por el que la persona está siendo elegida de nuevo para recibir correos electrónicos y haga clic en **Eliminar cancelación de suscripción**.

   ![](assets/four.png)

>[!NOTE]
>
>Si tiene activada la sincronización de cancelación de suscripción, debe desmarcar también la casilla de exclusión en el registro de Salesforce o la sincronización nocturna volverá a cancelar la suscripción de la persona en Conexión de ventas, ya que detectará que la persona está excluida en Salesforce. Si alguno de los registros se excluye o cancela la suscripción, la sincronización marcará el registro vinculado como tal.
