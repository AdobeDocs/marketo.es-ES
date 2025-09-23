---
unique-page-id: 14352484
description: Corrección del problema "No se pudo autenticar la solicitud" al conectarse a Salesforce - Documentos de Marketo - Documentación del producto
title: Cómo corregir «No hemos podido autenticar su solicitud» al conectarse a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 8%

---

# Cómo corregir &quot;No se pudo autenticar su solicitud&quot; al conectarse a [!DNL Salesforce] {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No pudimos autenticar su solicitud&quot; al intentar conectar [!DNL Sales Connect] a [!DNL Salesforce], podría haber una restricción en su acceso a la API de [!DNL Salesforce]. Consulte con su administrador de [!DNL Salesforce] para asegurarse de que se cumplan los siguientes requisitos.

## Habilitar API en permisos de usuario {#enable-api-in-user-permissions}

1. Haga que un administrador de [!DNL Salesforce] inicie sesión en SFDC.
1. Seleccione **[!UICONTROL Configuración]**.
1. Seleccione **[!UICONTROL Administrar usuarios]**.
1. Seleccione **[!UICONTROL Perfiles]**.
1. Busque el perfil en el que se encuentran los usuarios de ToutApp y haga clic en **[!UICONTROL Editar]**.
1. Desplácese hacia abajo hasta **[!UICONTROL Permisos administrativos]** y asegúrese de que la **[!UICONTROL API habilitada]** esté seleccionada.

## Comprobar si [!DNL Salesforce] está bloqueando la conexión de [!DNL Sales Connect] {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Haga que un administrador de [!DNL Salesforce] inicie sesión en SFDC.
1. Seleccione **[!UICONTROL Configuración]**.
1. Seleccione **[!UICONTROL Administrar aplicaciones]**.
1. Seleccione **[!UICONTROL Uso de OAuth para aplicaciones conectadas]**.
1. Asegúrese de que [!DNL Sales Connect] muestre &quot;[!UICONTROL Bloque]&quot; junto a él. Si ve &quot;[!UICONTROL Desbloquear]&quot;, haga clic en el botón para desbloquear el acceso de [!DNL Sales Connect] a [!DNL Salesforce].
