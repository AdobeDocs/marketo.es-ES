---
description: Configuración de administración de inicio de sesión - Documentos de Marketo - Documentación del producto
title: Configuración de administración de inicio de sesión
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configuración de administración de inicio de sesión {#login-management-settings}

La configuración de Gestión de inicios de sesión permite a los administradores establecer las preferencias de autenticación para los usuarios de Acciones de información de ventas a nivel global.

>[!NOTE]
>
>De forma predeterminada, la opción Solo de Salesforce estará seleccionada para las instancias de acciones de perspectiva de ventas. Recomendamos esta configuración para que los usuarios puedan [iniciar sesión automáticamente](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) desde Salesforce.

## Actualizar configuración de administración de inicio de sesión {#update-login-management-settings}

>[!NOTE]
>
>**Se requieren permisos de administración**

Para actualizar las preferencias de administración de inicio de sesión, siga estos pasos.

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/login-management-settings-1.png)

1. En Configuración de administración, haga clic en **General**.

   ![](assets/login-management-settings-2.png)

1. Desplácese hacia abajo hasta la tarjeta Administración de inicio de sesión y seleccione la configuración deseada (en este ejemplo, elegimos Solo Salesforce). Haga clic en **Guardar** cuando termine.

   ![](assets/login-management-settings-3.png)

## Preguntas frecuentes sobre Salesforce Only {#salesforce-only-faq}

Solo Salesforce significa que los usuarios solo pueden autenticarse para utilizar acciones de perspectiva de ventas con Salesforce. Es la selección predeterminada para las instancias de acciones de información de ventas, y se recomienda debido a su capacidad para permitir a los usuarios autenticarse sin problemas sin tener que administrar un nombre de usuario y una contraseña.

### ¿Cómo activa un nuevo usuario en mi instancia su cuenta cuando se selecciona &quot;Solo Salesforce&quot;? {#activate-when-salesforce-only-is-selected}

Al hacer clic en el botón **Introducción** del correo electrónico de invitación, los nuevos usuarios se enviarán a una pantalla de activación de cuenta, donde deberán conectar su instancia de Salesforce para activar su cuenta de acciones de información de ventas.

![](assets/login-management-settings-4.png)

### ¿Con qué métodos de autenticación pueden autenticarse mis usuarios cuando se selecciona &quot;Solo Salesforce&quot;? {#what-authentication-methods}

Al navegar a nuestra pantalla de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. A continuación, hará clic en el botón Salesforce One Click Login, donde podrá autenticarse con la cuenta de Salesforce en la que haya iniciado sesión.

>[!NOTE]
>
>Esto solo afecta a los usuarios que navegan directamente a la pantalla de inicio de sesión. Los usuarios que estén accediendo a Acciones desde Salesforce iniciarán sesión con [Inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### ¿Cómo se gestiona la autenticación de usuarios para las acciones cuando un usuario accede a una función de acciones desde Salesforce y se selecciona &quot;Solo Salesforce&quot;? {#how-is-user-authentication-handled}

Cuando un usuario hace clic en una de las acciones (llamada, correo electrónico, campaña, tareas, lista de campañas, etc.), utilizamos su autenticación SFDC para registrarla automáticamente en su cuenta de acciones de Sales Insight. A esta autenticación la llamamos [inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Preguntas frecuentes sobre todos los métodos de inicio {#all-login-methods-faq}

### ¿Cómo activa un nuevo usuario en mi instancia su cuenta cuando se selecciona &quot;Todos los métodos de inicio de sesión&quot;? {#activate-when-all-login-methods-is-selected}

Cuando se invita a un nuevo usuario a una instancia, recibirá un correo electrónico de activación de la cuenta. Ellos harán clic en el botón que dice &quot;Comenzar&quot;, que luego los llevará a una página que les pedirá que creen y confirmen una contraseña. Una vez creada esta acción, se activa la cuenta y se realiza a través del flujo de trabajo de incorporación.

![](assets/login-management-settings-6.png)

### ¿Con qué usuarios de mi instancia pueden iniciar sesión cuando se selecciona &quot;Todos los métodos de inicio de sesión&quot;? {#what-are-users-allowed-to-log-in-with-all-login}

Al utilizar nuestra página de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. A continuación, se envían a una página que les proporciona todas las opciones de inicio de sesión (nombre de usuario/contraseña, SFDC, Gmail, SSO) con las que autenticarse.
