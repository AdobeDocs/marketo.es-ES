---
description: 'Configuración de la integración de ON24 con Marketo: documentos de Marketo, documentación del producto'
title: Configuración de la integración ON24 con Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Configuración de la integración ON24 con Marketo{#set-up-the-on24-integration-with-marketo}

A continuación se muestra cómo configurar la integración de eventos ON24.

## Crear una función solo de API {#create-an-api-only-role}

1. En Mi Marketo, haga clic en **Administrador**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. En Seguridad, haga clic en **Usuarios y funciones**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Haga clic en **Funciones** y luego **Nuevo rol**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Introduzca un nombre de rol. Abra el **API de acceso** y seleccione &quot;Objeto personalizado de lectura y escritura&quot; y &quot;Persona de lectura y escritura&quot;. Haga clic en **Crear**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Crear un nuevo usuario {#create-a-new-user}

1. En Usuarios y funciones, haga clic en **Usuarios** y haga clic en **Invitar nuevo usuario**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Introduzca la información del nuevo usuario y haga clic en **Siguiente**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Seleccione la función Solo API ON24 que acaba de crear. Seleccione el **Solo API** casilla de verificación Clic **Siguiente**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Clic **Enviar**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>No se requiere una invitación para los usuarios solo de API.

## Configuración de la conexión ON24 {#set-up-on24-connection}

1. En la sección Administración, haga clic en **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Clic **Nuevo** entonces **Nuevo servicio**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Elija un nombre para mostrar. Haga clic en **Servicio** y seleccione. **Personalizado**. Introduzca una descripción. Haga clic en la lista desplegable Solo usuario de API y seleccione el usuario que ha creado [en los pasos anteriores](#create-a-new-user). Haga clic en **Crear**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Busque el servicio de LaunchPoint personalizado que acaba de crear y haga clic en Ver detalles.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Resalte, haga clic con el botón derecho, copie y guarde el ID de cliente (lo necesitará más adelante). Repita el proceso para Secreto del cliente.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. En el árbol de la izquierda, haga clic en Servicios Web.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. En &quot;API de REST&quot;, resalte, haga clic con el botón derecho, copie y guarde la primera parte de la identidad (hasta las &quot;m&quot; en .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Con el ID de cliente, el secreto de cliente y la identidad guardados, vaya a la cuenta ON24. El resto de los pasos se realizan allí y son [esbozado aquí](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target="_blank"}.
