---
unique-page-id: 12976798
description: Configuración de LinkedIn Lead Gen Forms - Documentos de marketing - Documentación del producto
title: Configuración de LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---


# Configurar el Forms de LinkedIn Lead Gen {#set-up-linkedin-lead-gen-forms}

Utilice LinkedIn Lead Gen Forms para ejecutar campañas de publicidad en LinkedIn y generar leads para Marketing.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya a Administrador de mercadotecnia ****.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **LaunchPoint**, haga clic en **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **Nombre para mostrar** para el servicio, seleccione el servicio **Generación de posibles clientes de LinkedIn** en la lista desplegable y haga clic en **Siguiente**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo abre una nueva ficha en el mismo explorador para [linkedin.com](https://www.linkedin.com). Inicie sesión en LinkedIn con la cuenta que desee utilizar para la integración.

   >[!NOTE]
   >
   >La cuenta de LinkedIn necesita tener acceso a todas las cuentas comerciales de LinkedIn para las que esté creando campañas patrocinadas.

   ![](assets/linkedin-login.png)

1. Una vez que haya iniciado sesión en LinkedIn, vuelva a Marketo y haga clic en **Autorizar**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Cuando se le solicite, haga clic en **Permitir** para aceptar la instalación de la aplicación de Marketing to en LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Notará que ahora está autorizado. Haga clic en **Siguiente**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >El servicio caduca automáticamente un año después de la autorización. Para recuperar el acceso, haga clic en **Volver a autorizar**. Es posible que tenga que volver a introducir la contraseña de LinkedIn, según la configuración del explorador.

1. Seleccione las cuentas desde las que desea que LinkedIn Lead Gen incluya los leads en Marketing y haga clic en **Siguiente**.

   >[!TIP]
   >
   >Si no ve las cuentas de negocio que espera, asegúrese de que la cuenta de LinkedIn del usuario que se está autorizando tenga permisos de administrador de formularios de generación de posibles clientes para la cuenta de negocio en LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Para aceptar las asignaciones de campo predeterminadas de LinkedIn a Marketing, haga clic en **Crear**. Si desea cambiar la asignación de campo predeterminada, quitar una asignación de campo o agregar una nueva asignación de campo, puede hacerlo por campo a través del modo siguiente.

   >[!CAUTION]
   >
   >Marketo admite la asignación de dos campos de LinkedIn a un solo campo de marketing, **pero solo cuando** los dos campos de LinkedIn no están en el mismo formulario. Si asigna dos campos del mismo formulario LinkedIn a un solo campo de marketing, es posible que las personas no puedan introducir la base de datos de marketing.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo los campos de LinkedIn que ya se han guardado en una [plantilla de formulario](https://www.linkedin.com/help/lms/answer/79634) en el Administrador de Campañas de LinkedIn se mostrarán como campos de LinkedIn que se pueden asignar a los campos de Marketo.

   ![](assets/linkedin-installed-services.png)

¡Bien hecho! Las personas que envíen formularios de LinkedIn Lead Gen tendrán inicios al ingresar a Marketing mientras ejecuta campañas correctas en el lado de LinkedIn.

>[!NOTE]
>
>Solo puede autorizar una única cuenta de usuario de LinkedIn. Si tiene varias cuentas de negocio que desea vincular a MarketingTo, asegúrese de que la cuenta de LinkedIn del usuario que está siendo autorizada tenga permisos de administrador de formularios de generación de posibles clientes para la cuenta de negocio en LinkedIn.

>[!MORELIKETHIS]
>
>[Usar Filtros y Déclencheur de formulario de generación de posibles clientes de LinkedIn en una Campaña inteligente](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
