---
description: "Cambiar límites personalizados de recuperación de objetos en  [!DNL Velocity Scripting] : documentos de Marketo: documentación del producto"
title: "Cambiar los límites personalizados de recuperación de objetos en  [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Cambiar límites personalizados de recuperación de objetos en [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Si usa [!DNL Velocity Script] para mostrar datos de objetos personalizados en mensajes de correo electrónico, esta característica podría ser la adecuada para usted. De forma predeterminada, se le permite acceder a 10 objetos personalizados principales desde Secuencia de comandos de Velocity. Si necesita acceder a más, siga leyendo.

## Qué es [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) es un lenguaje creado en [!DNL Java] y diseñado para crear plantillas y scripts de contenido de HTML. Marketo permite utilizarlo en el contexto de los correos electrónicos mediante el uso de [tokens de scripts](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Entre otras cosas, esto da acceso a los datos almacenados en objetos personalizados.

Puede hacer referencia a objetos personalizados primarios y secundarios que estén conectados directamente al posible cliente o contacto, pero no a objetos personalizados de tercer nivel. Para cada objeto personalizado, los 10 registros actualizados más recientemente por persona/contacto están disponibles en tiempo de ejecución y se ordenan desde los actualizados más recientemente (en 0) a los actualizados más antiguos (en 9).

## Cómo cambiar el límite {#how-to-change-the-limit}

1. Vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. En la tabla [!UICONTROL Límites personalizados de recuperación de objetos], escriba un nuevo [!UICONTROL Límite de recuperación principal] y haga clic en **[!UICONTROL Guardar cambios]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>El valor de [!UICONTROL Límite de recuperación principal] debe estar entre 10 y 100. El [!UICONTROL límite de recuperación de elementos secundarios] se ha establecido automáticamente. Esto se hace dividiendo 1000 entre [!UICONTROL Límite de recuperación principal]. Por ejemplo, si establece el límite Principal en 50, el límite Secundario se convierte en 20 (1000 ÷ 50 = 20).

¡Bonito! Ahora puede tener acceso a más objetos personalizados desde [!DNL Velocity script].
