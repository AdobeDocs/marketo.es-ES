---
unique-page-id: 3571819
description: 'Paso 3 de 3: Conexión de Marketo y Dynamics (2013 On-Premies) - Documentos de Marketo: Documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Dynamics (local 2013)'
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: f130fa1187ccead6573f76ff947e55d42f6962e4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo y Dynamics (local de 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

¡Bien! Hemos instalado la solución y configurado el usuario de sincronización. A continuación, es necesario conectar Marketo y Dynamics.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalación de la solución de Marketo en Dynamics (local 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [Paso 2 de 3: Configuración del usuario de sincronización para Marketo (locales de 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)


>[!NOTE]
>
>**Se requieren permisos de administrador**

## Introducir información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **Administrador**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Select **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Haga clic en **Editar** en **Paso 1: Introducir credenciales**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, deberá obtener una nueva suscripción a Marketo.

1. Introduzca la variable **Nombre de usuario**, **Contraseña** y Microsoft Dynamics **URL** a continuación, haga clic en **Guardar**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* El nombre de usuario en Marketo debe coincidir con el nombre de usuario para sincronizar el usuario en CRM. El formato puede ser user@domain.com o DOMINIO\usuario.
   >* Si no conoce la dirección URL, [aprenda a encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Seleccionar campos para sincronizar {#select-fields-to-sync}

Ahora necesitamos seleccionar los campos que queremos sincronizar.

1. Haga clic en **Editar** en **Paso 2: Seleccionar campos para sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleccione los campos que desea sincronizar con Marketo, de modo que se preseleccionarán. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la variable [sincronizar desactivado](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando el [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Campos de sincronización para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en **Paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Microsoft Dynamics o cuando introduzca manualmente personas o posibles clientes.

1. Lea todo en la ventana emergente, introduzca su correo electrónico y haga clic en **Iniciar sincronización**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez finalizado, recibirá una notificación por correo electrónico.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

¡Excelente trabajo! Acaba de liberar la potencia de la sincronización bidireccional entre Marketo y Microsoft Dynamics. Si ha comprado Marketo Sales Insight, puede ser más divertido:

>[!MORELIKETHIS]
>
>[Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
