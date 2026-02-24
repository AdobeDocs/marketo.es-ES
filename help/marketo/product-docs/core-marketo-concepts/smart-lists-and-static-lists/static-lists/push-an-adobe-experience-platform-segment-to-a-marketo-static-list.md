---
description: 'Inserción de un segmento de Adobe Experience Platform en una lista estática de Marketo: documentos de Marketo, documentación del producto'
title: Insertar un segmento de Adobe Experience Platform en una lista estática de Marketo
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 7f8968210659ed2c51640966115f22da47e42ebf
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 3%

---

# Insertar un segmento de Adobe Experience Platform en una lista estática de Marketo {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Esta función le permite insertar segmentos ubicados en su Adobe Experience Platform en Marketo Engage en forma de lista estática.

>[!PREREQUISITES]
>
>* [Edite la función de la API](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role){target="_blank"} para asegurarse de que tiene el permiso **Persona de lectura y escritura** (que se encuentra en la lista desplegable de la API de acceso).
>* [Crear un usuario de API](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"} en Marketo.
>* Vaya a **[!UICONTROL Administración]** > **[!UICONTROL Punto de inicio]**. Busque el nombre de la función que acaba de crear y haga clic en **[!UICONTROL Ver detalles]**. Copie y guarde la información en **[!UICONTROL ID de cliente]** y **[!UICONTROL Secreto de cliente]**, ya que podría necesitarla para el paso 7.
>* En Marketo, cree una lista estática o busque y seleccione una que ya haya creado. Necesitará su ID...

1. Inicie sesión en [Adobe Experience Platform](https://experience.adobe.com/){target="_blank"}.

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Haga clic en el icono de cuadrícula y seleccione **[!UICONTROL Experience Platform]**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. En la navegación izquierda, haga clic en **[!UICONTROL Destinos]**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Haga clic en **[!UICONTROL Catálogo]**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Busque el mosaico de Marketo Engage y haga clic en **[!UICONTROL Activar]**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Haga clic en **[!UICONTROL Configurar nuevo destino]**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)

1. En Tipo de cuenta, seleccione el botón de opción Cuenta existente o Cuenta nueva (en este ejemplo, elegimos **[!UICONTROL Cuenta existente]**). Haga clic en el icono Seleccionar cuenta.

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Si estás eligiendo Nueva cuenta, puedes encontrar tu Munchkin ID en **[!UICONTROL Administración]** > **[!UICONTROL Munchkin]** (también forma parte de tu URL de Marketo una vez que iniciaste sesión). ID/secreto de cliente que debe tener de seguir los requisitos previos de la parte superior de este artículo.

1. Elija la cuenta de destino y haga clic en **[!UICONTROL Seleccionar]**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Escriba un destino **[!UICONTROL Name]** y una descripción opcional. Haga clic en el menú desplegable Creación de personas y elija &quot;Coincidir con personas de Marketo existentes y crear personas que faltan en Marketo&quot; _o_ &quot;Coincidir solo con personas de Marketo existentes&quot; (en este ejemplo, elegimos la primera). También debe elegir un **[!UICONTROL Workspace]**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Si elige &quot;[!UICONTROL Coincidir solo con personas de Marketo existentes]&quot;, solo necesita asignar el correo electrónico o el ECID, para poder omitir los pasos 13-16.

1. Esta sección es opcional. Haga clic en **[!UICONTROL Crear]** para omitirlo.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Seleccione el destino que creó y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Elija el segmento que desea enviar a Marketo y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Si elige varios segmentos, tendrá que asignar cada segmento a una lista estática especificada en la ficha [!UICONTROL Programación de segmentos].

   >[!IMPORTANT]
   >
   >Después de activar un segmento en el destino de Marketo por primera vez, los perfiles de relleno que ya existían en el segmento antes de la activación del destino de Marketo pueden tardar _hasta 24 horas_. En adelante, cada vez que se añadan perfiles al segmento, se añadirán a Marketo inmediatamente.

1. Haga clic en **[!UICONTROL Agregar nueva asignación]**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Haga clic en el icono de asignación.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Elija los atributos que desee y haga clic en **[!UICONTROL Seleccionar]**. En este ejemplo, se elige el nombre, los apellidos y la dirección de correo electrónico.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >Puede asignar atributos de Experience Platform a cualquiera de los atributos a los que su organización tiene acceso en Marketo Engage. Use [Describir solicitud de API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database#describe){target="_blank"} para recuperar los campos de atributo a los que su organización tiene acceso.

1. Asigne los apellidos y el nombre de la compañía haciendo clic en **[!UICONTROL Agregar nueva asignación]** de nuevo y repitiendo el paso 15 dos veces, eligiendo **[!UICONTROL lastName]** y luego **[!UICONTROL companyName]**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Es hora de asignar la dirección de correo electrónico. Vuelva a hacer clic en **[!UICONTROL Agregar nueva asignación]**.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Haga clic en el icono de asignación.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Haga clic en el botón de radio Seleccionar área de nombres de identidad, elija **[!UICONTROL Correo electrónico]** y, a continuación, haga clic en **[!UICONTROL Seleccionar]**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Asignar un correo electrónico o un ECID desde la ficha **[!UICONTROL Área de nombres de identidad]** es lo más importante para garantizar que la persona coincida en Marketo. Asignar correo electrónico garantizará la tasa de coincidencia más alta.

1. Ahora es el momento de elegir los campos de origen. Para el correo electrónico, haga clic en el icono del cursor.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Haga clic en el botón de opción Seleccionar área de nombres de identidad, busque y seleccione **[!UICONTROL Correo electrónico]** y, a continuación, haga clic en **[!UICONTROL Seleccionar]**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Para elegir el campo de origen Nombre de la compañía, haga clic en el icono de cursor en su fila.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Deje activado el botón de opción Seleccionar atributos. Busque &quot;empresa&quot; y seleccione **[!UICONTROL companyName]**; a continuación, haga clic en **[!UICONTROL Seleccionar]**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Asigne los campos de origen de Apellido y Nombre haciendo clic en el icono de cursor de cada uno y repitiendo el paso 23 dos veces, eligiendo **[!UICONTROL lastName]** y luego **[!UICONTROL firstName]**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Haga clic en **[!UICONTROL Next]**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Revise los cambios y haga clic en **[!UICONTROL Finalizar]**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
