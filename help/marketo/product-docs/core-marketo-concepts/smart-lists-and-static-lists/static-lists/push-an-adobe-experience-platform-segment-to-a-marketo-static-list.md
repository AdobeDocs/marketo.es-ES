---
description: 'Inserción de un segmento de Adobe Experience Platform en una lista estática de Marketo: documentos de Marketo, documentación del producto'
title: Insertar un segmento de Adobe Experience Platform en una lista estática de Marketo
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Insertar un segmento de Adobe Experience Platform en una lista estática de Marketo {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Esta función le permite insertar segmentos ubicados en su Adobe Experience Platform en Marketo en forma de lista estática.

>[!PREREQUISITES]
>
>* [Editar la función de API](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) para asegurarse de que tiene el **Persona de lectura-escritura** (que se encuentra en la lista desplegable API de acceso).
>* [Creación de un usuario de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) en Marketo.
>* Ir a **Administrador** > **Launchpoint**. Busque el nombre de la función que acaba de crear y haga clic en **Ver detalles**. Copie y guarde la información en **ID de cliente** y **Secreto del cliente**, ya que podría necesitarlo para el paso 7.
>* En Marketo, cree una lista estática o busque y seleccione una que ya haya creado. Necesitará su ID...

1. Iniciar sesión en [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Haga clic en el icono de cuadrícula y seleccione **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. En la navegación izquierda, haga clic en **Destinos**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Clic **Catálogo**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Busque el mosaico del Marketo Engage y haga clic en **Activar**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Clic **Configurar nuevo destino**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. En Tipo de cuenta, seleccione el botón de opción Cuenta existente o Cuenta nueva (en este ejemplo, elegimos **Cuenta existente**). Haga clic en el icono Seleccionar cuenta.

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Si elige Nueva cuenta, puede encontrar su ID de Munchkin en **Administrador** > **Munchkin** (también forma parte de la URL de Marketo una vez que se ha iniciado sesión). ID/secreto de cliente que debe tener de seguir los requisitos previos de la parte superior de este artículo.

1. Seleccione la cuenta de destino y haga clic en **Seleccionar**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Introduzca un destino **Nombre** y una Descripción opcional. Haga clic en el menú desplegable Creación de personas y elija &quot;Hacer coincidir personas de Marketo existentes y crear personas que faltan en Marketo&quot; _o_ &quot;Coincidir solo con personas de Marketo existentes&quot; (en este ejemplo, se elige la primera). También debe elegir una **Workspace**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Si elige &quot;Asignar solo personas de Marketo existentes&quot;, solo necesita asignar el correo electrónico o el ECID, para poder omitir los pasos 13-16.

1. Esta sección es opcional. Clic **Crear** para omitir.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Seleccione el destino que ha creado y haga clic en **Siguiente**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Seleccione el segmento que desea enviar a Marketo y haga clic en **Siguiente**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Si elige varios segmentos, tendrá que asignar cada segmento a una lista estática especificada en la pestaña Programación de segmentos.

   >[!IMPORTANT]
   >
   >Después de activar un segmento en el destino de Marketo por primera vez, los perfiles de relleno que ya existían en el segmento antes de la activación del destino de Marketo pueden tardar **hasta 24 horas**. En adelante, cada vez que se añadan perfiles al segmento, se añadirán a Marketo inmediatamente.

1. Clic **Añadir nueva asignación**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Haga clic en el icono de asignación.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Seleccione los atributos que desee y haga clic en **Seleccionar**. En este ejemplo, se elige el nombre, los apellidos y la dirección de correo electrónico.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >Puede asignar atributos de Experience Platform a cualquiera de los atributos a los que su organización tiene acceso en Marketo Engage. Utilice el [Describir solicitud de API](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} para recuperar campos de atributos a los que su organización tiene acceso.

1. Asigne los apellidos y el nombre de la empresa haciendo clic en **Añadir nueva asignación** y repitiendo el paso 15 dos veces, eligiendo **lastName** y luego **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Es hora de asignar la dirección de correo electrónico. Clic **Añadir nueva asignación** otra vez.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Haga clic en el icono de asignación.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Haga clic en el botón de radio Seleccionar área de nombres de identidad y elija  **Correo electrónico**, luego haga clic en **Seleccionar**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Asignación de correo electrónico o ECID desde el **Área de nombres de identidad** es lo más importante que hay que hacer para garantizar que la persona coincida en Marketo. Asignar correo electrónico garantizará la tasa de coincidencia más alta.

1. Ahora es el momento de elegir los campos de origen. Para el correo electrónico, haga clic en el icono del cursor.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Haga clic en el botón de radio Seleccionar área de nombres de identidad, busque y seleccione **Correo electrónico**, luego haga clic en **Seleccionar**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Para elegir el campo de origen Nombre de la compañía, haga clic en el icono de cursor en su fila.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Deje activado el botón de opción Seleccionar atributos. Busque &quot;empresa&quot; y seleccione **companyName**, luego haga clic en **Seleccionar**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Asigne los campos de origen de Apellido y Nombre haciendo clic en el icono de cursor de cada uno y repitiendo el paso 23 dos veces, eligiendo **lastName** y luego **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Clic **Siguiente**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Revise los cambios y haga clic en **Finalizar**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
