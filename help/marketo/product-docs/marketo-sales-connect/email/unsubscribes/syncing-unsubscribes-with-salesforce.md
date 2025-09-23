---
unique-page-id: 14746188
description: 'Sincronización de cancelaciones de suscripción con Salesforce: documentos de Marketo, documentación del producto'
title: Sincronizar cancelaciones de suscripción con Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 2%

---

# Sincronizando cancelaciones de suscripción con [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelar la suscripción a la sincronización con [!DNL Salesforce] {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronización de cancelación de suscripción debe estar habilitada (para sincronización nocturna)
* El campo de exclusión debe estar instalado en [!DNL Salesforce]
* Los registros de persona de [!DNL Sales Connect] deben tener un identificador de [!DNL Salesforce]

**Cancelaciones de suscripción push**

Cuando se recopila una cancelación de suscripción en [!DNL Sales Connect], se inserta en [!DNL Salesforce] en tiempo real y se actualiza cualquiera de los campos de exclusión seleccionados para sincronizar. Si deshabilitaste la sincronización de [!DNL Salesforce], la cancelación de la suscripción se enviará al correo electrónico de exclusión.

**Cancelar la suscripción a la sincronización**

Cuando haya habilitado la sincronización de cancelación de suscripción (Paso 3 a continuación), activará la sincronización nocturna. La sincronización se produce una vez al día alrededor de las 20:00 PST. :00 Sincronizará bidireccionalmente todas las cancelaciones de suscripción en Marketo Sales con el campo de exclusión de Salesforce.

## Configurar la sincronización de cancelación de suscripción a [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Los usuarios pueden decidir si desean sincronizar sus cancelaciones de suscripción con el campo de exclusión de correo electrónico estándar con el que Marketo también puede sincronizarse, o pueden sincronizar con el campo de exclusión de ventas de Marketo para poder diferenciar las cancelaciones de suscripción de ventas y las de marketing.

1. Vaya a la [aplicación web](https://toutapp.com/login), haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-1.png)

1. En [!UICONTROL Configuración de administración], seleccione **[!UICONTROL Anular la suscripción]**.

   ![](assets/two-2.png)

1. Haga clic en **[!UICONTROL Sincronizando con Salesforce]** y, a continuación, habilite la sincronización nocturna.

   ![](assets/three-2.png)

1. Seleccione el campo con el que desea sincronizar.

   ![](assets/4.png)

   | Campo | Descripción |
   |---|---|
   | **[!UICONTROL Campo de exclusión de sincronización con Salesforce]** | Seleccionado de forma predeterminada, solo actualiza el campo de exclusión [!DNL Salesforce]. |
   | **[!UICONTROL Campo de no participación en la sincronización con Marketo Sales]** | Si desea separar las cancelaciones de suscripción de ventas y marketing, elija esta opción para actualizar el campo [Exclusión de ventas de Marketo adicional.](#msoo) |

## Instalación del campo de exclusión en el diseño de página {#installing-the-opt-out-field-in-the-page-layout}

**Exclusión por correo electrónico**

Exclusión de correo electrónico es un campo estándar en [!DNL Salesforce] que está disponible para la instalación desde [!DNL Salesforce]. Debe ser administrador de [!DNL Salesforce] para instalarlo.

1. Vaya a [Salesforce.com](https://salesforce.com) e inicie sesión.

   ![](assets/five-1.png)

1. Haga clic en su nombre de usuario y seleccione **[!UICONTROL Configuración]**.

   ![](assets/six-1.png)

1. En el cuadro de búsqueda rápida, busque Contacto o Posible cliente. En esta situación, se está instalando el campo en el diseño de página Contacto, pero es recomendable instalar para ambos registros de persona.

   ![](assets/seven-1.png)

1. Seleccione **[!UICONTROL Diseños de página]**.

   ![](assets/eight-1.png)

1. Seleccione **[!UICONTROL Editar]** junto al diseño de página al que desee agregar el campo.

   ![](assets/nine.png)

1. Seleccione **[!UICONTROL Campos]**.

   ![](assets/ten.png)

1. Arrastre y suelte [!UICONTROL Exclusión por correo electrónico] en el diseño de página.

   ![](assets/11.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/twelve.png)

## No participar de las Marketo Sales {#marketo-sales-opt-out}

El campo Exclusión de ventas de Marketo es un campo personalizado disponible para los usuarios que han instalado las personalizaciones de Marketo [!DNL Sales Connect].

Una vez que haya instalado correctamente las personalizaciones de Marketo [!DNL Sales Connect] en [!DNL Salesforce], verá el campo Exclusión de ventas de Marketo disponible para usted.
