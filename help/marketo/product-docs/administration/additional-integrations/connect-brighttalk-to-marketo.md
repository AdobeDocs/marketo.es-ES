---
unique-page-id: 15695874
description: Connect BrightTALK to Marketing - Documentos de marketing - Documentación del producto
title: Connect BrightTALK to Marketing
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Connect BrightTALK to Marketing {#connect-brighttalk-to-marketo}

Obtenga información sobre cómo conectar el canal BrightTALK con la instancia de Marketing. Para ello, debe ser administrador de ambos.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Pasos en BrightTALK {#steps-in-brighttalk}

1. Inicie sesión en [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login) y haga clic en **Conectar ahora**.
1. En Conector de marketing avanzado, haga clic en **Conectar**.
1. Llegará a la pantalla de credenciales, donde se le pedirá: ID del cliente, Secreto del cliente, URL del servicio de identidad y URL del servicio de descanso. Para obtener esta información, inicie sesión en Marketing Cloud.

## Pasos en el marketing {#steps-in-marketo}

>[!NOTE]
>
>En este punto, deberá configurar una función de usuario y un usuario de API solo de API para restringir los permisos que BrightTALK tendrá en la instancia de Marketing. Porque ya tenemos artículos para esos pasos, los enlazaremos a ellos.

1. Cree una [función de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Cree un usuario](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) de API mediante la función de API BrightTALK que creó durante el paso 4.
1. Vuelva al área Administración.

   ![](assets/one.png)

1. En Integración, haga clic en **LaunchPoint**.

   ![](assets/two.png)

1. Haga clic en la lista desplegable **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/three.png)

1. Introduzca un nombre para mostrar de su elección. Haga clic en la lista desplegable Servicio y seleccione **Personalizado** (haga _no_ seleccione BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Recuerde no seleccionar BrightTALK en la lista desplegable. Se trata de un campo que estamos eliminando y que podría crear problemas significativos con la integración de Marketing/BrightTALK.

1. Introduzca una descripción de su elección. Haga clic en la lista desplegable Solo usuario de API y seleccione el usuario de API BrightTALK que creó durante el paso 5. Haga clic en **Crear**.

   ![](assets/five.png)

1. Haga clic en **Detalles de Vista** para el servicio personalizado que acaba de crear.

   ![](assets/six.png)

1. Copie (y guarde) el **ID del cliente** y **Secreto del cliente**. Haga clic en **Cerrar**.

   ![](assets/eight-1.png)

1. En Integración, seleccione **Servicios Web**.

   ![](assets/nine-1.png)

1. En Rest API, copie (y guarde) el **Extremo** y **Identidad**.

   ![](assets/ten.png)

## Pasos adicionales en BrightTALK {#additional-steps-in-brighttalk}

1. Vuelva a la pantalla de configuración del conector BrightTALK del paso 3 e introduzca las credenciales guardadas en los pasos 12 y 14.

   Una vez autenticadas las credenciales, ha conectado oficialmente BrightTALK a Marketing. El siguiente paso es determinar [los campos de datos que desea sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).
