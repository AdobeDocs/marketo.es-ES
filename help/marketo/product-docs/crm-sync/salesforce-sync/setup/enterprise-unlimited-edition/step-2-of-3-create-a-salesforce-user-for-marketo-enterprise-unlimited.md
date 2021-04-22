---
unique-page-id: 2360364
description: 'Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited): Documentos de Marketo: Documentación del producto'
title: 'Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estos pasos debe completarlos un administrador de Salesforce

>[!PREREQUISITES]
>
>[Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

En este artículo, debe configurar los permisos de usuario en el perfil de Salesforce y crear una cuenta de integración de Marketo-Salesforce.

## Crear un perfil {#create-a-profile}

1. Haga clic en **Configuración**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de navegación y haga clic en el enlace **Perfiles**.

   ![](assets/sfdc-profiles-hands.png)

1. Haga clic en **New**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleccione **Usuario estándar**, asigne al perfil el nombre &quot;Marketo-Salesforce Sync&quot; y haga clic en **Guardar**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definir permisos de perfil {#set-profile-permissions}

1. Haga clic en **Editar** para establecer los permisos de seguridad.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. En la sección **Permisos administrativos**, asegúrese de que las siguientes casillas estén marcadas:

   * API habilitada
   * Editar plantillas HTML
   * Administrar documentos públicos
   * Administrar plantillas públicas

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Asegúrese de marcar la casilla **Password Never Expires**.

1. En la sección Permisos generales de usuario , asegúrese de que las siguientes casillas estén marcadas:

   * Convertir posibles clientes
   * Editar eventos
   * Editar tareas

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. En la sección Permisos de objeto estándar , asegúrese de que los permisos de lectura, creación, edición y eliminación estén marcados para:

   * Cuentas
   * Campañas
   * Contactos
   * Posibles clientes
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permisos a Campañas si planea utilizar la sincronización de campañas.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Cuando termine, haga clic en **Guardar** en la parte inferior de la página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permisos de campo {#set-field-permissions}

1. Analice con sus especialistas en marketing para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite se muestren en Marketo, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a la sección **Seguridad de nivel de campo**. Haga clic en **Ver** para editar la accesibilidad para los objetos:

   * Posible cliente
   * Contacto
   * Cuenta
   * Oportunidad

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, haga clic en **Editar**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Busque los campos innecesarios, asegúrese de que **Read Access** y **Edit Access** no estén marcados. Haga clic en **Guardar** cuando haya terminado.

   >[!NOTE]
   >
   >Editar solo la accesibilidad para los campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Una vez que haya terminado de deshabilitar todos los campos innecesarios, debe comprobar **Acceso de lectura y Editar acceso** para los siguientes campos de objeto. Haga clic en **Guardar** cuando haya terminado.

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
>Cree una cuenta específica de Salesforce (por ejemplo, marketo@yourcompany.com) para distinguir los cambios realizados por Marketo de otros usuarios de Salesforce.

1. Escriba &quot;Administrar usuarios&quot; en la barra de búsqueda de navegación y haga clic en **Usuarios**. Haga clic en **Nuevo usuario**.

   ![](assets/sfdc-new-users.png)

1. Rellene los campos obligatorios. A continuación, seleccione la **Licencia de usuario: Salesforce** y el perfil que creó anteriormente. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Se ha completado el paso 2 de 2.

>[!NOTE]
>
>[Paso 3 de 3: Conectar Marketo y Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
