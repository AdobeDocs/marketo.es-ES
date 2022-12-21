---
unique-page-id: 11375827
description: Campos requeridos para sincronizar Marketo con Dynamics - Marketo Docs - Documentación del producto
title: Campos requeridos para sincronizar Marketo con Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 2%

---

# Campos requeridos para sincronizar Marketo con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Estos campos *must* sincronice con Marketo para que funcione tanto el posible cliente como Contacto para la perspectiva de ventas:

* Prioridad
* Urgencia
* Puntaje relativo

Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para arreglarlo, compruebe la instancia para asegurarse de que los campos están sincronizados para **Posible cliente** y **Contacto**. Si no es así, agréguelos.

A continuación se explica cómo verificar y agregar campos de sincronización.

1. Vaya a Administración y haga clic en **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. En Posible cliente, marque la casilla Prioridad .

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ahora, desplácese hacia abajo y marque la casilla Urgencia ...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...y la casilla Puntuación relativa .

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. A continuación, marque las casillas de verificación Prioridad, Urgencia y Puntuación relativa para el contacto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Haga clic en **Guardar**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Asegúrese de esperar al menos 10 minutos para que se ejecute una sincronización antes de comprobar que ha corregido el problema.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de posible cliente/contacto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
