---
unique-page-id: 11375827
description: Campos obligatorios para sincronizar Marketo con Dynamics - Documentos de Marketo - Documentación del producto
title: Campos obligatorios para sincronizar Marketo con Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 3%

---

# Campos obligatorios para sincronizar Marketo con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Estos campos *deben* sincronizarse con Marketo tanto para el posible cliente como para que funcione la perspectiva del contacto de ventas:

* Prioridad
* Urgencia
* Puntaje relativo

Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, proteja su instancia para asegurarse de que los campos estén sincronizados para **Lead** y **Contact**. Si no es así, agréguelos.

A continuación, se indica cómo verificar y agregar campos de sincronización.

1. Vaya a Administración y haga clic en **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haz clic en **Editar** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. En Posible cliente, marque la casilla Prioridad.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ahora, desplácese hacia abajo y marque la casilla Urgencia...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ... y la casilla de verificación Puntuación relativa.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. A continuación, marque las casillas de verificación Prioridad, Urgencia y Puntuación relativa para Contacto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Haga clic en **Guardar**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Asegúrese de esperar al menos 10 minutos para que se ejecute una sincronización antes de comprobar que ha corregido el problema.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
