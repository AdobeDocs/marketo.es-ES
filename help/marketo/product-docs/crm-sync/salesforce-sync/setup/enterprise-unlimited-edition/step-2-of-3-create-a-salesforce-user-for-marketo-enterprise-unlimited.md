---
unique-page-id: 2360364
description: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (Enterprise/Unlimited), documentos de Marketo: documentación del producto'
title: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 4%

---

# Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estos pasos debe completarlos un administrador de Salesforce

>[!PREREQUISITES]
>
>[Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

En este artículo, configurará los permisos de usuario en el perfil de Salesforce y creará una cuenta de integración de Marketo-Salesforce.

## Crear un perfil {#create-a-profile}

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de navegación y haga clic en **[!UICONTROL Perfiles]** vínculo.

   ![](assets/sfdc-profiles-hands.png)

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleccionar **[!UICONTROL Usuario estándar]**, asigne un nombre al perfil &quot;Marketo-Salesforce Sync&quot; y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definición de permisos de perfil {#set-profile-permissions}

1. Clic **[!UICONTROL Editar]** para establecer los permisos de seguridad.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. En el **[!UICONTROL Permisos administrativos]** , asegúrese de que las siguientes casillas estén marcadas:

   * API habilitada
   * Editar plantillas de HTML
   * Administrar documentos públicos
   * Administrar plantillas públicas

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Asegúrese de comprobar el **[!UICONTROL La contraseña nunca caduca]** cuadro.

1. En la sección Permisos generales de usuario, asegúrese de que las siguientes casillas estén marcadas:

   * Convertir posibles clientes
   * Editar eventos
   * Editar tareas

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. En la sección Permisos de objeto estándar, asegúrese de que los permisos Leer, Crear, Editar y Eliminar están marcados para:

   * Cuentas
   * Campañas
   * Contactos
   * Clientes potenciales
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permisos a las campañas si planea utilizar la sincronización de campañas.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Cuando termine, haga clic en **[!UICONTROL Guardar]** en la parte inferior de la página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permisos de campo {#set-field-permissions}

1. Hable con los especialistas en marketing para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite se muestren en Marketo, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a **[!UICONTROL Seguridad de nivel de campo]** sección. Clic **[!UICONTROL Ver]** para editar la accesibilidad de los objetos:

   * Posible cliente
   * Contacto
   * Cuenta
   * Oportunidad

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Haga clic en cada objeto **[!UICONTROL Editar]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Busque los campos innecesarios, asegúrese de que **[!UICONTROL Acceso de lectura]** y **[!UICONTROL Editar acceso]** están desmarcadas. Clic **[!UICONTROL Guardar]** cuando termine.

   >[!NOTE]
   >
   >Editar solo la accesibilidad de los campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Una vez que termine de deshabilitar todos los campos innecesarios, debe comprobar **[!UICONTROL Acceso de lectura y acceso de edición]** para los siguientes campos de objeto. Clic **[!UICONTROL Guardar]** cuando termine.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Objeto</p></th> 
   <th colspan="1" rowspan="1"><p>Campos</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Cuenta</p></td> 
   <td colspan="1" rowspan="1"><p>Campo Tipo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Evento</p></td> 
   <td colspan="1" rowspan="1"><p>Todos los campos</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tarea</p></td> 
   <td colspan="1" rowspan="1"><p>Todos los campos</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Crear cuenta de sincronización de Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Cree una cuenta de Salesforce dedicada (por ejemplo, `marketo@yourcompany.com`) para distinguir los cambios realizados por Marketo frente a otros usuarios de Salesforce.

1. Escriba &quot;Administrar usuarios&quot; en la barra de búsqueda de navegación y haga clic en **[!UICONTROL Usuarios]**. Clic **[!UICONTROL Nuevo usuario]**.

   ![](assets/sfdc-new-users.png)

1. Rellene los campos obligatorios. A continuación, seleccione la **[!UICONTROL Licencia de usuario: Salesforce]** y el perfil que ha creado anteriormente. Clic **[!UICONTROL Guardar]** cuando hayas terminado.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Se ha completado el paso 2 de 2.

>[!NOTE]
>
>[Paso 3 de 3: Conectar Marketo y Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
