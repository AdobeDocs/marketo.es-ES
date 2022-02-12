---
description: Configuración de administración de inicio de sesión - Documentos de Marketo - Documentación del producto
title: Configuración de administración de inicio de sesión
hide: true
hidefromtoc: true
source-git-commit: e3d175d9f6131ec9798c4047ccf79858c254c745
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configuración de administración de inicio de sesión {#login-management-settings}

La configuración de Administración de inicio de sesión permite a los administradores establecer las preferencias de autenticación para los usuarios de las acciones de perspectiva de ventas a nivel global.

>[!NOTE]
>
>De forma predeterminada, la opción Solo Salesforce está seleccionada para las instancias Acciones de perspectiva de ventas. Recomendamos esta configuración para que los usuarios puedan [inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) de Salesforce.

## Actualizar configuración de administración de inicio de sesión {#update-login-management-settings}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Siga estos pasos para actualizar las preferencias de administración de inicio de sesión.

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/login-management-settings-1.png)

1. En Configuración de administración, haga clic en **General**.

   ![](assets/login-management-settings-2.png)

1. Desplácese hacia abajo hasta la tarjeta Administración de inicio de sesión y seleccione la configuración deseada (en este ejemplo elegimos Solo Salesforce). Haga clic en **Guardar** cuando haya terminado.

   ![](assets/login-management-settings-3.png)

## Preguntas frecuentes sobre Salesforce Only {#salesforce-only-faq}

Sólo Salesforce significa que los usuarios solo pueden autenticarse para utilizar las acciones de perspectiva de ventas con Salesforce. Es la selección predeterminada para instancias de acciones de perspectiva de ventas y se recomienda debido a su capacidad de permitir que los usuarios se autentiquen sin problemas sin tener que administrar un nombre de usuario y una contraseña.

### ¿Cómo activa su cuenta un nuevo usuario en mi instancia cuando está seleccionado &quot;Solo Salesforce&quot;? {#activate-when-salesforce-only-is-selected}

Al hacer clic en el botón **Introducción** en el correo electrónico de invitación, los nuevos usuarios se enviarán a una pantalla de activación de cuenta en la que se les pedirá que conecten su instancia de Salesforce para activar su cuenta de acciones de perspectiva de ventas.

![](assets/login-management-settings-4.png)

### ¿Con qué métodos de autenticación pueden autenticarse mis usuarios cuando se selecciona &quot;Solo Salesforce&quot;? {#what-authentication-methods}

Al navegar a nuestra pantalla de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. A continuación, harán clic en el botón Salesforce One Click Login , donde podrán autenticarse con la cuenta de Salesforce en la que iniciaron sesión.

>[!NOTE]
>
>Esto solo se aplica a los usuarios que navegan directamente a la pantalla de inicio de sesión. Los usuarios que accedan a Acciones desde Salesforce iniciarán sesión con [Inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### ¿Cómo se gestiona la autenticación de usuarios para las acciones cuando un usuario accede a una función de Acciones desde Salesforce y se selecciona &quot;Solo Salesforce&quot;? {#how-is-user-authentication-handled}

Cuando un usuario hace clic en una de las acciones (llamada, correo electrónico, campaña, tareas, lista de campañas, etc.), utilizamos su autenticación SFDC para registrarlas automáticamente en su cuenta de acciones de perspectiva de ventas. Llamamos a esta autenticación [Inicio de sesión automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Preguntas frecuentes sobre todos los métodos de inicio de sesión {#all-login-methods-faq}

### ¿Cómo activa la cuenta un nuevo usuario en mi instancia cuando se selecciona &quot;Todos los métodos de inicio de sesión&quot;? {#activate-when-all-login-methods-is-selected}

Cuando se invite a un nuevo usuario a una instancia, recibirá un correo electrónico de activación de cuenta. Harán clic en el botón que dice &quot;Introducción&quot;, que luego los llevará a una página que les pedirá que creen y confirmen una contraseña. Una vez creada esta opción, su cuenta se activará y se tomarán a través del flujo de trabajo de incorporación.

![](assets/login-management-settings-6.png)

### ¿Con qué se permite a los usuarios de mi instancia iniciar sesión cuando se selecciona &quot;Todos los métodos de inicio de sesión&quot;? {#what-are-users-allowed-to-log-in-with-all-login}

Al utilizar nuestra página de inicio de sesión, los usuarios introducirán primero su dirección de correo electrónico. A continuación, se enviarán a una página que les proporcione todas las opciones de inicio de sesión (nombre de usuario/contraseña, SFDC, Gmail, SSO) con las que se autenticarán.
