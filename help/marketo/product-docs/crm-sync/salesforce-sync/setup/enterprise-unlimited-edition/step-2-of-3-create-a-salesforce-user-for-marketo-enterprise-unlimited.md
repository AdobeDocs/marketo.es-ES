---
unique-page-id: 2360364
description: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (empresarial/ilimitado): Documentos de Marketo: documentación del producto'
title: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (empresarial/ilimitado)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# Paso 2 de 3: Crear un usuario de [!DNL Salesforce] para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estos pasos debe completarlos un administrador de [!DNL Salesforce]

>[!PREREQUISITES]
>
>[Paso 1 de 3: Agregar campos de Marketo a [!DNL Salesforce] (Empresa/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

En este artículo, configurará los permisos de usuario en el perfil [!DNL Salesforce] y creará una cuenta de integración Marketo-[!DNL Salesforce].

## Crear un perfil {#create-a-profile}

1. Haga clic en **[!UICONTROL Configuración]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de navegación y haga clic en el vínculo **[!UICONTROL Perfiles]**.

   ![](assets/sfdc-profiles-hands.png)

1. Haz clic en **[!UICONTROL Nuevo]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleccione **[!UICONTROL Usuario estándar]**, asigne al perfil el nombre &quot;Sincronización de Marketo-Salesforce&quot; y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definición de permisos de perfil {#set-profile-permissions}

1. Haga clic en **[!UICONTROL Editar]** para establecer los permisos de seguridad.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. En la sección **[!UICONTROL Permisos administrativos]**, asegúrese de marcar las siguientes casillas:

   * [!UICONTROL API habilitada]
   * [!UICONTROL Editar plantillas de HTML]
   * [!UICONTROL Administrar documentos públicos]
   * [!UICONTROL Administrar plantillas públicas]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Asegúrese de marcar la casilla **[!UICONTROL La contraseña nunca caduca]**.

1. En la sección [!UICONTROL Permisos generales de usuario], asegúrese de marcar las siguientes casillas:

   * [!UICONTROL Convertir posibles clientes]
   * [!UICONTROL Editar eventos]
   * [!UICONTROL Editar tareas]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. En la sección [!UICONTROL Permisos de objeto estándar], asegúrese de comprobar los permisos de [!UICONTROL Leer, Crear, Editar y Eliminar] para:

   * [!UICONTROL Cuentas]
   * [!UICONTROL Campañas]
   * [!UICONTROL Contactos]
   * [!UICONTROL Posibles clientes]
   * [!UICONTROL Oportunidades]

   >[!NOTE]
   >
   >Conceda permisos a [!UICONTROL Campañas] si planea usar la sincronización de campañas.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Cuando termine, haga clic en **[!UICONTROL Guardar]** en la parte inferior de la página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permisos de campo {#set-field-permissions}

1. Hable con los especialistas en marketing para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite se muestren en Marketo, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a la sección **[!UICONTROL Seguridad de nivel de campo]**. Haga clic en **[!UICONTROL Ver]** para editar la accesibilidad de los objetos:

   * [!UICONTROL Posible cliente]
   * [!UICONTROL Contacto]
   * [!UICONTROL Cuenta]
   * [!UICONTROL Oportunidad]

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, haga clic en **[!UICONTROL Editar]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Busque los campos que no necesite, asegúrese de que las opciones **[!UICONTROL Acceso de lectura]** y **[!UICONTROL Editar acceso]** estén desactivadas. Haz clic en **[!UICONTROL Guardar]** cuando hayas terminado.

   >[!NOTE]
   >
   >Editar solo la accesibilidad de los campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Una vez que termine de deshabilitar todos los campos innecesarios, debe comprobar **[!UICONTROL Acceso de lectura y acceso de edición]** para los siguientes campos de objeto. Haz clic en **[!UICONTROL Guardar]** cuando hayas terminado.

<table>
 <tbody>
  <tr>
   <th>Objeto</th>
   <th>Campos</th>
  </tr>
  <tr>
   <td>Cuenta</td>
   <td>Campo Tipo</td>
  </tr>
  <tr>
   <td>Evento</td>
   <td>Todos los campos</td>
  </tr>
  <tr>
   <td>Tarea</td>
   <td>Todos los campos</td>
  </tr>
 </tbody>
</table>

![](assets/sfdc-check-the-boxes.png)

## Crear cuenta de sincronización de Marketo y Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Cree una cuenta [!DNL Salesforce] específica (por ejemplo, <marketo@yourcompany.com>) para distinguir los cambios realizados por Marketo en comparación con otros usuarios de [!DNL Salesforce].

1. Escriba &quot;Administrar usuarios&quot; en la barra de búsqueda de navegación y luego haga clic en **[!UICONTROL Usuarios]**. Haz clic en **[!UICONTROL Nuevo usuario]**.

   ![](assets/sfdc-new-users.png)

1. Rellene los campos obligatorios. A continuación, seleccione la **[!UICONTROL licencia de usuario: Salesforce]** y el perfil que creó anteriormente. Haz clic en **[!UICONTROL Guardar]** cuando hayas terminado.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Se ha completado el paso 2 de 3.

>[!NOTE]
>
>[Paso 3 de 3: conectar Marketo y [!DNL Salesforce] (empresa/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
