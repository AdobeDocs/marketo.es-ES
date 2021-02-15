---
unique-page-id: 11375827
description: Campos requeridos para sincronizar el marketing con Dynamics - Documentos de marketing - Documentación del producto
title: Campos requeridos para sincronizar el marketing con Dynamics
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Campos requeridos para sincronizar el marketing con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Estos campos *deben* sincronizarse con Marketing para que funcionen tanto el posible cliente como el contacto para la perspectiva de ventas:

* Prioridad
* Urgencia
* Puntuación relativa

Si falta alguno de estos campos, verá un mensaje de error en el menú de marketing con el nombre de los campos que faltan. Para solucionarlo, desproteja la instancia para asegurarse de que los campos están sincronizados para **posible cliente** y **contacto**. Si no, agréguelas.

A continuación se muestra cómo comprobar y agregar campos de sincronización.

1. Vaya a Administración y haga clic en **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. En Posible cliente, marque la casilla Prioridad.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ahora, desplácese hacia abajo y marque la casilla Urgencia...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...y la casilla Puntuación relativa.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. A continuación, marque las casillas de verificación Prioridad, Urgencia y Puntuación relativa para el contacto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Haga clic en **Guardar**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Asegúrese de esperar al menos 10 minutos para que se ejecute una sincronización antes de comprobar que ha solucionado el problema.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contacto/posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
