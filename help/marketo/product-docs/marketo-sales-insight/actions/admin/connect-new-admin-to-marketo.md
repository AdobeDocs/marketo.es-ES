---
description: 'Conectar nuevo administrador a Marketo: Documentos de Marketo: Documentación del producto'
title: Conectar nuevo administrador a Marketo
hide: true
hidefromtoc: true
source-git-commit: 0ed5981470998dadd5f42384cd2e9572fec94ef6
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Conectar nuevo administrador a Marketo {#connect-new-admin-to-marketo}

Si el otro administrador ya está conectado a Marketo, solo tiene que realizar el paso 1.

Si el segundo administrador no está conectado a Marketo como administrador...

1. El administrador principal debe desconectar el segundo administrador de Marketo desde Configuración > Marketo > Acceso de usuario

1. El administrador secundario inicia sesión en su cuenta MSC, va a Configuración > Marketo y hace clic en **Connect**.

1. Ahora el usuario secundario está conectado a Marketo como administrador.

1. El administrador principal ahora puede iniciar sesión y desconectarse de Marketo.

>[!NOTE]
>
>Los demás usuarios permanecerán conectados mientras el usuario B esté conectado como administrador antes de que el usuario A se desconecte.

## Actualizar la conexión de Marketo {#update-your-marketo-connection}

Si decide eliminar el administrador que configuró la integración de Marketo, consulte este artículo para obtener información sobre cómo hacerlo.

La integración de Marketo estará vinculada a un usuario administrador de Conexión/Acciones de ventas. Normalmente, este es el administrador que primero hizo clic en el botón &quot;Conectar&quot; de la página de conexión de Marketo y estableció la conexión.

Para eliminar el administrador que estableció la conexión de Marketo, primero debe establecer una nueva conexión otro usuario administrador. Hemos enumerado las tareas siguientes que deberán completarse para hacerlo.

Para simplificar las instrucciones, nos referiremos al administrador conectado actualmente como administrador A y al administrador con el que desea establecer una nueva conexión a Marketo como administrador B:

1. El administrador A (administrador conectado actualmente) deberá eliminar el acceso a la integración con Marketo del administrador B (nuevo administrador).

1. Pida al administrador B (nuevo administrador) que establezca una nueva conexión con Marketo.

1. Desconecte el administrador A (administrador conectado originalmente).

>[!NOTE]
>
>El administrador original responsable de la integración de Marketo verá una opción &quot;Desconectar&quot; en la que se puede hacer clic al navegar a la página de integración de Marketo. Otros administradores (que no hayan establecido una conexión) no lo harán. Además, los administradores a los que se ha concedido acceso a la integración de Marketo no podrán hacer clic en Connect, por lo que primero debe seguir los pasos para eliminar el acceso a la integración.

**Eliminar el acceso a Marketo del administrador B**

El administrador A (originalmente responsable de la conexión) debe seguir estos pasos.

1. Vaya a la configuración .

1. Haga clic en **Marketo**.

1. Haga clic en **Acceso de usuarios**.

1. Busque el administrador para el que desea establecer la nueva conexión de Marketo.

1. Elimine el acceso.

**Establecer nueva conexión para el administrador B**

Estos pasos debe seguir el administrador B (nuevo administrador)

1. Vaya a la configuración .

1. Haga clic en **Marketo**.

1. Haga clic en **Desconectar**.

**Desconectar la integración de Marketo para el administrador A**

Estos pasos debe seguirlos el administrador A (administrador conectado originalmente)

1. Vaya a la configuración .

1. Haga clic en **Marketo**.

1. Haga clic en **Desconectar**.

Ahora que un nuevo administrador ha establecido una conexión con Marketo y que el administrador original ha sido desconectado, el administrador conectado originalmente se puede eliminar de forma segura de la instancia de Conexión/Acciones de ventas.
