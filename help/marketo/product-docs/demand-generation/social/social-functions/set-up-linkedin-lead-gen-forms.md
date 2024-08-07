---
unique-page-id: 12976798
description: Configuración de LinkedIn Lead Gen Forms - Documentos de Marketo - Documentación del producto
title: Configuración de LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Configuración de LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilice LinkedIn Lead Gen Forms para ejecutar campañas publicitarias en LinkedIn y generar posibles clientes para Marketo.

>[!IMPORTANT]
>
>LinkedIn está actualizando sus API de marketing utilizadas por las integraciones de Marketo Engage LinkedIn. Estos cambios requerirán la reautenticación de todos los servicios LaunchPoint de LinkedIn en su menú de **Admin** > **LaunchPoint** entre el 7 de junio y el 15 de diciembre de 2024 para evitar la interrupción del servicio. Para obtener más información, consulte las [Preguntas frecuentes sobre la migración](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>Un posible cliente de LinkedIn no se considerará Marketo Engage si coincide con un registro de persona existente en Marketo asociado a un registro de empresa creado mediante las API de empresa y si la suscripción de Marketo no está conectada a un CRM.

1. Vaya a Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **LaunchPoint**, haga clic en **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **Nombre para mostrar** para su servicio, seleccione el servicio **LinkedIn Lead Gen** en la lista desplegable y haga clic en **Siguiente**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo abre una nueva ficha en el mismo explorador en [linkedin.com](https://www.linkedin.com). Inicie sesión en LinkedIn con la cuenta que desee utilizar para la integración.

   >[!NOTE]
   >
   >La cuenta de LinkedIn necesita acceder a todas las cuentas empresariales de LinkedIn para las que está creando campañas patrocinadas.

   ![](assets/linkedin-login.png)

1. Cuando haya iniciado sesión en LinkedIn, vuelva a Marketo y haga clic en **Autorizar**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Cuando se le solicite, haga clic en **Permitir** aceptar la instalación de la aplicación Marketo en LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Verá que ahora está autorizado. Haga clic en **Siguiente**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >El servicio caduca automáticamente un año después de la autorización. Para recuperar el acceso, simplemente haga clic en **Volver a autorizar**. Es posible que tenga que volver a introducir la contraseña de LinkedIn, según la configuración del explorador.

1. Seleccione las cuentas desde las que desea que los posibles clientes de LinkedIn Lead Gen entren en Marketo y haga clic en **Siguiente**.

   >[!TIP]
   >
   >Si no ve las cuentas empresariales que espera, asegúrese de que la cuenta de LinkedIn del usuario que se está autorizando tenga permisos de administrador de formularios de generación de clientes potenciales para la cuenta empresarial en LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Para aceptar las asignaciones de campo predeterminadas de LinkedIn a Marketo, simplemente haga clic en **Crear**. Si desea cambiar la asignación de campo predeterminada, quitar una asignación de campo o agregar una nueva asignación de campo, puede hacerlo por campo a través del modal siguiente.

   >[!CAUTION]
   >
   >Marketo admite la asignación de dos campos de LinkedIn a un único campo de Marketo, **pero solo cuando** los dos campos de LinkedIn no están en el mismo formulario. Si asigna dos campos del mismo formulario de LinkedIn a un único campo de Marketo, es posible que no se pueda introducir la base de datos de Marketo.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo los campos de LinkedIn que ya se hayan guardado en una [plantilla de formulario](https://www.linkedin.com/help/lms/answer/79634) en el Administrador de LinkedIn Campaign se mostrarán como campos de LinkedIn que se pueden asignar a campos de Marketo.

   ![](assets/linkedin-installed-services.png)

¡Bien hecho! Las personas que envíen formularios de LinkedIn Lead Gen empezarán a fluir a Marketo a medida que ejecute campañas exitosas en el lado de LinkedIn.

>[!NOTE]
>
>Solo puede autorizar una sola cuenta de usuario de LinkedIn. Si tiene varias cuentas empresariales que desea vincular a Marketo, asegúrese de que la cuenta de LinkedIn del usuario autorizado tenga permisos de administrador de formularios de generación de clientes potenciales para la cuenta empresarial en LinkedIn.

>[!MORELIKETHIS]
>
>[Usar Déclencheur y filtros de formularios de generación de clientes potenciales de LinkedIn en una campaña inteligente](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
