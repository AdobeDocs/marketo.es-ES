---
unique-page-id: 2360364
description: Paso 2 de 3 -Crear un usuario de Salesforce para el marketing (Enterprise/Unlimited) - Documentos de marketing - Documentación del producto
title: 'Paso 2 de 3: Crear un usuario de Salesforce para el marketing (Enterprise/Unlimited)'
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Paso 2 de 3: Crear un usuario de Salesforce para el marketing (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estos pasos deben ser completados por un administrador de Salesforce

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Añadir campos de marketing a Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

>



En este artículo, configurará los permisos de usuario en Salesforce perfil y creará una cuenta de integración de Marketing-Salesforce.

## Crear un Perfil {#create-a-profile}

1. Haga clic en **Configuración**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de Nav y haga clic en el vínculo **Perfiles** .

   ![](assets/sfdc-profiles-hands.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleccione Usuario **** estándar, asigne al perfil el nombre &quot;Marketo-Salesforce Sync&quot; y haga clic en **Guardar**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definir permisos de Perfil {#set-profile-permissions}

1. Haga clic en **Editar** para definir los permisos de seguridad.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. En la sección Permisos **** administrativos, asegúrese de marcar las siguientes casillas:

   * API habilitada
   * Editar plantillas HTML
   * Administrar Documentos públicos
   * Administrar plantillas públicas

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Asegúrese de marcar la casilla **Contraseña nunca caduca** .

1. En la sección Permisos generales de usuario, asegúrese de marcar las siguientes casillas:

   * Convertir leads
   * Editar Eventos
   * Editar Tareas

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. En la sección Permisos de objeto estándar, asegúrese de que los permisos de lectura, creación, edición y eliminación están marcados para:

   * Cuentas
   * Campañas
   * Contactos
   * Posibles clientes
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permisos a las Campañas, si planea utilizar la sincronización de Campañas.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Cuando termine, haga clic en **Guardar** en la parte inferior de la página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permisos de campo {#set-field-permissions}

1. Analice con los especialistas en mercadotecnia para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite que aparezcan en Marketing Cloud, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a la sección Seguridad **en el nivel de** campo. Haga clic en **Vista** para editar la accesibilidad de los objetos:

   * `Lead`
   * `Contact`
   * `Account`
   * `Opportunity`

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, haga clic en **Editar**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Busque los campos no necesarios, asegúrese de que **Acceso de lectura **** y Editar acceso **están desactivados. Haga clic en **Guardar** cuando haya terminado.

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Editar sólo la accesibilidad para los campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Una vez que haya terminado de desactivar todos los campos innecesarios, debe comprobar **Acceso de lectura y Editar acceso **para los siguientes campos de objeto. Haga clic en **Guardar** cuando haya terminado.

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

## Crear cuenta de sincronización de Marketing-to-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Cree una cuenta de Salesforce dedicada (p. ej. [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#89e4e8fbe2ecfde6c9f0e6fcfbeae6e4f9e8e7f0a7eae6e4)) para distinguir los cambios realizados por Marketing con respecto a otros usuarios de Salesforce.

1. Escriba &quot;Administrar usuarios&quot; en la barra de búsqueda de Nav y, a continuación, haga clic en **Usuarios**. Haga clic en **Nuevo usuario**.

   ![](assets/sfdc-new-users.png)

1. Rellene los campos obligatorios. A continuación, seleccione la licencia **de usuario: Salesforce** y el Perfil que creó anteriormente. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Se ha completado el paso 2 de 2.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Paso 3 de 3: Connect Marketing y Salesforce (Enterprise/Unlimited)](step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)

>



