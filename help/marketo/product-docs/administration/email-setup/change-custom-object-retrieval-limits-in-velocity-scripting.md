---
description: Cambio de los límites personalizados de recuperación de objetos en las secuencias de comandos de Velocity - Documentos de Marketo - Documentación del producto
title: Cambio de los límites de recuperación de objetos personalizados en las secuencias de comandos de Velocity
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Cambiar los límites personalizados de recuperación de objetos en las secuencias de comandos de Velocity {#change-custom-object-retrieval-limits-in-velocity-scripting}

Si utiliza el Script de Velocity para mostrar los datos de objetos personalizados en los correos electrónicos, esta función puede ser adecuada para usted. De forma predeterminada, se le permite acceder a 10 objetos personalizados principales desde Velocity Script. Si necesita acceder a más, siga leyendo.

## ¿Qué es Velocity {#what-is-velocity}?

[Apache Velocity](https://velocity.apache.org/) es un lenguaje creado en Java diseñado para crear plantillas y crear secuencias de comandos de contenido HTML. Marketo permite utilizarla en el contexto de los correos electrónicos mediante el uso de [tokens de secuencias de comandos](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Entre otras cosas, esto proporciona acceso a los datos almacenados en objetos personalizados.

Puede hacer referencia a objetos personalizados principales y secundarios conectados directamente al posible cliente o al contacto, pero no a objetos personalizados de tercer nivel. Para cada objeto personalizado, los 10 registros actualizados más recientemente por persona/contacto están disponibles en tiempo de ejecución y se ordenan desde la última actualización (en 0) hasta la última actualización (en 9).

## Cómo cambiar el límite {#how-to-change-the-limit}

1. Vaya a la sección **Admin**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Haga clic en **Email**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. En la tabla Límites de recuperación de objetos personalizados, introduzca un nuevo Límite de recuperación principal y haga clic en **Guardar cambios**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>El valor del límite de recuperación principal debe estar en el rango de 10 a 100. El límite de recuperación secundaria se establece automáticamente. Esto se hace dividiendo 1000 por el Límite de recuperación principal. Por ejemplo, si establece el límite Principal en 50, el límite Secundario se convierte en 20 (1000 ÷ 50 = 20).

¡Dulce! Ahora puede acceder a más objetos personalizados desde el script de Velocity.
