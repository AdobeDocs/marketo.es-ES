---
description: Configuración de administración de inicio de sesión - Documentos de Marketo - Documentación del producto
title: Configurar administración de inicio de sesión
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 2%

---

# Configurar administración de inicio de sesión {#login-management-settings}

La configuración de Gestión de inicios de sesión permite a los administradores definir las preferencias de autenticación para los usuarios de las acciones de Sales Insight a nivel global.

>[!NOTE]
>
>De manera predeterminada, la opción [!UICONTROL Solo Salesforce] se seleccionará para [!DNL Sales Insight Actions] instancias. Recomendamos esta configuración para que los usuarios puedan [iniciar sesión automáticamente](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) desde [!DNL Salesforce].

## Actualizar configuración de administración de inicio de sesión {#update-login-management-settings}

>[!NOTE]
>
>**Se requieren permisos de administración**

Para actualizar las preferencias de administración de inicio de sesión, siga estos pasos.

1. Haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/login-management-settings-1.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL General]**.

   ![](assets/login-management-settings-2.png)

1. Desplácese hacia abajo hasta la tarjeta [!UICONTROL Administración de inicio de sesión] y seleccione la configuración que desee (en este ejemplo elegimos Solo Salesforce). Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/login-management-settings-3.png)

## Preguntas frecuentes solo sobre Salesforce {#salesforce-only-faq}

Solo Salesforce significa que los usuarios solo pueden autenticarse para usar [!DNL Sales Insight Actions] con [!DNL Salesforce]. Es la selección predeterminada para [!DNL Sales Insight Actions] instancias y se recomienda debido a su capacidad para permitir a los usuarios autenticarse sin problemas sin tener que administrar un nombre de usuario y una contraseña.

### ¿Cómo activa un nuevo usuario en mi instancia su cuenta cuando se selecciona &quot;[!UICONTROL Solo Salesforce]&quot;? {#activate-when-salesforce-only-is-selected}

Al hacer clic en el botón **[!UICONTROL Introducción]** del correo electrónico de invitación, los nuevos usuarios se enviarán a una pantalla de activación de cuenta, donde deberán conectar su instancia de Salesforce para activar su cuenta de [!DNL Sales Insight Actions].

![](assets/login-management-settings-4.png)

### ¿Con qué métodos de autenticación pueden autenticarse mis usuarios cuando se selecciona &quot;[!UICONTROL Solo Salesforce]&quot;? {#what-authentication-methods}

Al navegar a nuestra pantalla de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. Luego harán clic en el botón [!UICONTROL Iniciar sesión] de Salesforce One Click, donde podrán autenticarse con la cuenta de Salesforce en la que iniciaron sesión.

>[!NOTE]
>
>Esto solo afecta a los usuarios que navegan directamente a la pantalla de inicio de sesión. Los usuarios que estén accediendo a acciones desde [!DNL Salesforce] iniciarán sesión con [Inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### ¿Cómo se gestiona la autenticación de usuarios para las acciones cuando un usuario accede a una función de acciones desde Salesforce y se selecciona &quot;Solo Salesforce&quot;? {#how-is-user-authentication-handled}

Cuando un usuario hace clic en una de las acciones (llamada, correo electrónico, campaña, tareas, lista de campañas, etc.), utilizamos su autenticación de SFDC para registrarla automáticamente en su cuenta de [!DNL Sales Insight Actions]. A esta autenticación la llamamos [inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Preguntas frecuentes sobre todos los métodos de inicio {#all-login-methods-faq}

### ¿Cómo activa un nuevo usuario en mi instancia su cuenta cuando se selecciona &quot;Todos los métodos de inicio de sesión&quot;? {#activate-when-all-login-methods-is-selected}

Cuando se invita a un nuevo usuario a una instancia, recibirá un correo electrónico de activación de la cuenta. Ellos harán clic en el botón que dice &quot;Comenzar&quot;, que luego los llevará a una página que les pedirá que creen y confirmen una contraseña. Una vez creada esta acción, se activa la cuenta y se realiza a través del flujo de trabajo de incorporación.

![](assets/login-management-settings-6.png)

### ¿Qué usuarios de mi instancia pueden iniciar sesión con cuando se selecciona &quot;[!UICONTROL Todos los métodos de inicio de sesión]&quot;? {#what-are-users-allowed-to-log-in-with-all-login}

Al utilizar nuestra página de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. A continuación, se les envía a una página que les proporciona todas las opciones de inicio de sesión (nombre de usuario/contraseña, SFDC, Gmail, SSO) con las que autenticarse.
