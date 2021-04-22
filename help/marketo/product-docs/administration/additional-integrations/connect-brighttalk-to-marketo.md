---
unique-page-id: 15695874
description: Conexión de BrightTALK a Marketo - Marketo Docs - Documentación del producto
title: Conectar BrightTALK a Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Conectar BrightTALK a Marketo {#connect-brighttalk-to-marketo}

Aprenda a conectar el canal BrightTALK a la instancia de Marketo. Para ello, debe ser administrador de ambos.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Pasos en BrightTALK {#steps-in-brighttalk}

1. Inicie sesión en [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login) y haga clic en **Conectar ahora**.
1. En Conector Marketo avanzado, haga clic en **Conectar**.
1. Llegará a la pantalla de credenciales, pidiendo lo siguiente: ID del cliente, Secreto del cliente, URL del servicio de identidad y URL del servicio de descanso. Para obtener esta información, inicie sesión en Marketo.

## Pasos en Marketo {#steps-in-marketo}

>[!NOTE]
>
>En este punto, deberá configurar una función de usuario y un usuario de API solo de API para restringir los permisos que BrightTALK tendrá en su instancia de Marketo. Como ya tenemos artículos para esos pasos, los enlazaremos a ellos.

1. Cree una [función de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Cree un usuario](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) de API mediante la función de API BrightTALK que creó durante el paso 4.
1. Vuelva al área de administración.

   ![](assets/one.png)

1. En Integración, haga clic en **LaunchPoint**.

   ![](assets/two.png)

1. Haga clic en la lista desplegable **New** y seleccione **New Service**.

   ![](assets/three.png)

1. Introduzca un nombre para mostrar de su elección. Haga clic en la lista desplegable Servicio y seleccione **Personalizado** (haga _not_ seleccionar BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Recuerde no seleccionar BrightTALK en la lista desplegable. Se trata de un campo que estamos eliminando y que, si lo seleccionamos, podría crear problemas importantes con la integración de Marketo/BrightTALK.

1. Introduzca una descripción de su elección. Haga clic en la lista desplegable Solo usuario de API y seleccione el usuario de API BrightTALK que creó durante el paso 5. Haga clic en **Crear**.

   ![](assets/five.png)

1. Haga clic en **Ver detalles** para el servicio personalizado que acaba de crear.

   ![](assets/six.png)

1. Copie (y guarde) el **Client ID** y el **Client Secret**. Haga clic en **Cerrar**.

   ![](assets/eight-1.png)

1. En Integración, seleccione **Servicios Web**.

   ![](assets/nine-1.png)

1. En la API de Rest, copie (y guarde) los **Endpoint** y **Identity**.

   ![](assets/ten.png)

## Pasos adicionales en BrightTALK {#additional-steps-in-brighttalk}

1. Vuelva a la pantalla de configuración del conector BrightTALK del paso 3 e introduzca las credenciales que guardó en los pasos 12 y 14.

   Una vez autenticadas las credenciales, ha conectado oficialmente BrightTALK a Marketo. El siguiente paso es determinar [qué campos de datos desea sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).
