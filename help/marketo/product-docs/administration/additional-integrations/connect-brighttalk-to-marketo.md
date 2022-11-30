---
unique-page-id: 15695874
description: Conexión de BrightTALK a Marketo - Marketo Docs - Documentación del producto
title: Conectar BrightTALK a Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Conectar BrightTALK a Marketo {#connect-brighttalk-to-marketo}

Aprenda a conectar el canal BrightTALK a la instancia de Marketo. Para ello, debe ser administrador de ambos.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Pasos en BrightTALK {#steps-in-brighttalk}

1. Iniciar sesión en [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} y haga clic en **Conectar ahora**.
1. En Conector de Marketo avanzado, haga clic en **Connect**.
1. Llegará a la pantalla de credenciales, pidiendo lo siguiente: ID del cliente, Secreto del cliente, URL del servicio de identidad y URL del servicio de descanso. Para obtener esta información, inicie sesión en Marketo.

## Pasos en Marketo {#steps-in-marketo}

>[!NOTE]
>
>En este punto, deberá configurar una función de usuario y un usuario de API solo de API para restringir los permisos que BrightTALK tendrá en su instancia de Marketo. Como ya tenemos artículos para esos pasos, los enlazaremos a ellos.

1. Cree un [Función de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Crear un usuario de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}, utilizando la función de API BrightTALK que creó durante el paso 4.

1. Vuelva al área de administración.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. En Integración, haga clic en **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Haga clic en el **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Introduzca un nombre para mostrar de su elección. Haga clic en la lista desplegable Service y seleccione **Personalizado** (do _not_ seleccione BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Recuerde no seleccionar BrightTALK en la lista desplegable. Se trata de un campo que estamos eliminando y que, si lo seleccionamos, podría crear problemas importantes con la integración de Marketo/BrightTALK.

1. Introduzca una descripción de su elección. Haga clic en la lista desplegable Solo usuario de API y seleccione el usuario de API BrightTALK que creó durante el paso 5. Haga clic en **Crear**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Haga clic en **Ver detalles** para el servicio personalizado que acaba de crear.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copie (y guarde) el **ID de cliente** y **Secreto del cliente**. Haga clic en **Cerrar**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. En Integración, seleccione **Servicios Web**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. En la API de Rest, copie (y guarde) la variable **Punto final** y **Identidad**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Pasos adicionales en BrightTALK {#additional-steps-in-brighttalk}

1. Vuelva a la pantalla de configuración del conector BrightTALK del paso 3 e introduzca las credenciales que guardó en los pasos 12 y 14.

   Una vez autenticadas las credenciales, ha conectado oficialmente BrightTALK a Marketo. El siguiente paso es determinar [qué campos de datos desea sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
