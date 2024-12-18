---
unique-page-id: 2953373
description: Configuración de los pies de página para cancelar la suscripción en Marketo Sales Insight - Documentos de Marketo - Documentación del producto
title: Configuración de los pies de página para cancelar suscripción en Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Configuración de los pies de página para cancelar suscripción en Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Los correos electrónicos de ventas sitúan automáticamente el pie de página de cancelación de suscripción en la parte inferior. Sin embargo, puede ajustar la configuración para satisfacer sus necesidades.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>**Definición**
>
>**Correos electrónicos de ventas** son los enviados desde Sales Insight (no incluye los enviados desde el Complemento de Outlook de Marketo).

1. Vaya al área de **Admin**.

   ![](assets/one-1.png)

1. Haga clic en **Información de ventas** y luego en **Editar configuración**.

   ![](assets/two-1.png)

   Hay varias opciones. Primero vamos a echar un vistazo a los tipos de correos electrónicos para los que puede cambiar la configuración.

   ![](assets/three-1.png)

   * **Sin plantilla** - Compuesto manualmente por el usuario de ventas.
   * **Correo electrónico estándar**: correos electrónicos basados en una plantilla.
   * **Correo electrónico operativo**: Correos electrónicos que omiten los límites de cancelación de suscripción, marketing suspendido y comunicaciones (se envían independientemente de qué).

   Tiene la opción de establecer un comportamiento diferente para cada tipo.

   >[!CAUTION]
   >
   >**Respetar la configuración de cancelación de suscripción**: los posibles clientes no suscritos NO recibirán el correo electrónico aunque el correo electrónico publicado esté &quot;operativo&quot;
   >
   >**Ignorar configuración de cancelación de suscripción**: los posibles clientes no suscritos recibirán el correo electrónico

1. Realice los cambios que desee y haga clic en **Guardar**.

   >[!TIP]
   >
   >Las dos últimas opciones permiten incluir o excluir dinámicamente el pie de página de cancelación de suscripción en función del número de destinatarios (mayor que 1 o mayor que 5).

   ![](assets/four-1.png)

¡Uy! Un poco complicado, pero bastante flexible, ¿verdad?
