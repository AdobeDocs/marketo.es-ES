---
description: Consentimiento de concesión para el ID de cliente y el registro de aplicaciones - Documentos de Marketo - Documentación del producto
title: Conceder consentimiento para el ID de cliente y el registro de la aplicación
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Concesión de consentimiento para el ID de cliente y el registro de aplicación {#grant-consent-for-client-id-and-app-registration}

## Otorgar permisos de usuario delegados para el usuario de sincronización {#grant-delegated-user-permissions-for-the-sync-user}

1. Utilice un programa de texto limpio (Bloc de notas para Windows, Edición de texto para Mac) para crear un identificador uniforme de recursos (URI) para la autorización pegando el texto siguiente y sustituyendo los valores client_id, redirect_uri y state.

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>valor client_id</strong></td> 
      <td>debe ser client_id generado en el proceso de registro de la aplicación</td> 
     </tr> 
     <tr> 
      <td><strong>valor de redirect_uri</strong></td> 
      <td>debe ser el mismo que el valor introducido en el momento del registro de la aplicación &gt; URI de redireccionamiento</td> 
     </tr> 
     <tr> 
      <td><strong>valor de estado</strong></td> 
      <td>puede ser cualquier ID (por ejemplo, 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   La dirección URL final debería tener un aspecto similar al siguiente: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Abra el URI que ha creado en cualquier explorador.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Inicie sesión como usuario de sincronización para el que concede permisos.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Si ya ha iniciado sesión en Azure como administrador en otra ficha, deberá utilizar un explorador diferente o modo Incognito para iniciar sesión como usuario de sincronización.

1. Haga clic en **Accept**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Conceder consentimiento a todos los usuarios {#grant-consent-for-all-users}

Como administrador, también puede dar su consentimiento a los permisos delegados de una aplicación en nombre de todos los usuarios del inquilino. El consentimiento administrativo evita que aparezca el cuadro de diálogo de consentimiento para cada usuario del inquilino y los usuarios con la función de administrador pueden hacerlo en el portal de Azure. Aprenda qué funciones de administrador pueden [dar su consentimiento a los permisos delegados aquí](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. En su portal de Azure, vaya a la página principal de la aplicación.

1. En Administrar, haga clic en **Permisos de API**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Haga clic en el botón **Grant admin permission** (para el inquilino).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Haga clic en **Yes** para confirmar.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[Configuración de la aplicación Microsoft Dynamics CRM para On-Premim](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
