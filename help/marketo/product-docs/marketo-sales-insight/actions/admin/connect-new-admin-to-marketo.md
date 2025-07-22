---
description: 'Conectar nuevos administradores a Marketo: documentos de Marketo: documentación del producto'
title: Conectar el nuevo administrador a Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Conectar el nuevo administrador a Marketo {#connect-new-admin-to-marketo}

Si el otro administrador ya está conectado a Marketo, solo necesita realizar el paso 1.

Si el segundo administrador no está conectado a Marketo como administrador...

1. El administrador principal debe desconectar al segundo administrador de Marketo de [!UICONTROL Configuración] > Marketo > [!UICONTROL Acceso de usuario].

1. El administrador secundario inicia sesión en su cuenta MSC, va a [!UICONTROL Configuración] > Marketo y hace clic en **[!UICONTROL Conectar]**.

1. Ahora el usuario secundario está conectado a Marketo como administrador.

1. El administrador principal ahora puede iniciar sesión y desconectarse de Marketo.

>[!NOTE]
>
>Los demás usuarios permanecerán conectados mientras el usuario B esté conectado como administrador antes de que el usuario A se desconecte.

## Actualizar la conexión de Marketo {#update-your-marketo-connection}

Si decide eliminar el administrador que configuró la integración de Marketo, consulte este artículo para obtener más información.

La integración de Marketo se vinculará a un usuario administrador de [!DNL Sales Connect]/acciones. Normalmente, es el administrador que primero hizo clic en el botón **[!UICONTROL Conectar]** de la página de conexión de Marketo y estableció la conexión.

Para eliminar el administrador que estableció la conexión de Marketo, otro usuario administrador debe establecer primero una nueva conexión. Hemos enumerado las tareas siguientes que deben completarse para poder realizar esta acción.

Con el fin de simplificar las instrucciones, nos referiremos al administrador conectado actualmente como administrador A y al administrador con el que desea establecer una nueva conexión a Marketo como administrador B:

1. El administrador A (administrador conectado actualmente) deberá eliminar el acceso a la integración con Marketo del administrador B (nuevo administrador).

1. Pida al administrador B (nuevo administrador) que establezca una nueva conexión con Marketo.

1. Desconecte el administrador A (administrador conectado originalmente).

>[!NOTE]
>
>El administrador original responsable de la integración de Marketo verá una opción &quot;Desconectar&quot; en la que se puede hacer clic al navegar a la página de integración de Marketo. Otros administradores (que no han establecido una conexión) no lo harán. Además, los administradores a los que se les haya concedido acceso a la integración de Marketo no podrán hacer clic en Conectar, por lo que debe seguir primero los pasos para eliminar el acceso a la integración.

**Quitar el acceso a Marketo del administrador B**

El administrador A (administrador originalmente responsable de la conexión) debe seguir estos pasos.

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **[!UICONTROL Configuración]**.

1. Haga clic en **Marketo**.

1. Haga clic en **[!UICONTROL Acceso de usuario]**.

1. Busque el administrador para el que desee establecer la nueva conexión de Marketo.

1. Eliminar acceso.

**Establecer nueva conexión para el administrador B**

Estos pasos deben ir seguidos por el administrador B (nuevo administrador)

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **[!UICONTROL Configuración]**.

1. Haga clic en **Marketo**.

1. Haga clic en **[!UICONTROL Desconectar]**.

**Desconectar la integración de Marketo para el administrador A**

Estos pasos deben ir seguidos por el administrador A (administrador conectado originalmente).

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **[!UICONTROL Configuración]**.

1. Haga clic en **Marketo**.

1. Haga clic en **[!UICONTROL Desconectar]**.

Ahora que un nuevo administrador ha establecido una conexión con Marketo y se ha desconectado el administrador original, el administrador conectado originalmente se puede eliminar de forma segura de la instancia [!DNL Sales Connect]/Actions.
