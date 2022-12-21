---
unique-page-id: 2953373
description: Configurar la cancelación de la suscripción de los pies de página en Marketo Sales Insight - Marketo Docs - Documentación del producto
title: Configurar la cancelación de la suscripción de pies de página en Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Configurar la cancelación de la suscripción de pies de página en Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Los correos electrónicos de ventas colocan automáticamente el pie de página de cancelación de suscripción en la parte inferior. Sin embargo, puede ajustar la configuración para adaptarla a sus necesidades.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>**Definición**
>
>**Correos electrónicos de ventas** son los enviados desde Sales Insight (no incluye los enviados desde el complemento de Marketo Outlook).

1. Vaya a la **Administrador** .

   ![](assets/one-1.png)

1. Haga clic en **Perspectiva de ventas**, luego **Editar configuración**.

   ![](assets/two-1.png)

   Hay varias opciones. Primero echemos un vistazo a los tipos de correos electrónicos para los que puede cambiar la configuración.

   ![](assets/three-1.png)

   * **Sin plantilla** - Compuesto manualmente por el usuario de ventas.
   * **Correo electrónico estándar** - Correos electrónicos basados en una plantilla.
   * **Correo electrónico operativo** - Correos electrónicos que omiten la cancelación de la suscripción, el marketing suspendido y los límites de comunicación (envían lo que sea).

   Tiene la opción de establecer un comportamiento diferente para cada tipo.

   >[!CAUTION]
   >
   >**Respetar la configuración de cancelación de suscripción**: los posibles clientes no suscritos NO recibirán el correo electrónico aunque el correo publicado sea &quot;operativo&quot;
   >
   >**Ignorar configuración de cancelación de suscripción**: posibles clientes que se hayan dado de baja recibirán un correo electrónico

1. Realice los cambios que desee y haga clic en **Guardar**.

   >[!TIP]
   >
   >Las dos últimas opciones permiten incluir/excluir dinámicamente el pie de página de cancelación de suscripción según el número de destinatarios (Bueno de 1 o Bueno de 5).

   ![](assets/four-1.png)

¡Guau! Un poco complicado, pero bastante flexible, ¿verdad?
