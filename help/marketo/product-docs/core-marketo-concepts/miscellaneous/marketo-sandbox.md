---
unique-page-id: 11386358
description: Marketo Sandbox - Marketo Docs - Documentación del producto
title: Marketo Sandbox
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Marketo Sandbox {#marketo-sandbox}

Un entorno limitado de Marketo es una instancia adicional que se utiliza para realizar pruebas antes de la implementación en el entorno de producción.

>[!AVAILABILITY]
>
>No todos los clientes han comprado esta función. Póngase en contacto con el gestor de éxito de los clientes para obtener más información.

Un simulador para pruebas de Marketo no se puede sincronizar con su CRM normal si ya está sincronizado con su instancia de producción. Utilice el simulador para pruebas de CRM para la sincronización y siga los mismos pasos que la sincronización original.

## Aspectos importantes sobre los entornos limitados {#things-to-know-about-sandboxes}

* Una vez que el gestor de éxito del cliente ha configurado el simulador de pruebas y le envía la invitación, debe utilizar una dirección de correo electrónico diferente para iniciar sesión que la instancia de producción de Marketo.
* Si desea agregar usuarios, el proceso es el mismo que [agregar usuarios en producción](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). De nuevo, deben utilizar una dirección de correo electrónico diferente si ya tienen un inicio de sesión de Marketo.
* El simulador para pruebas de Marketo comenzará vacío, pero tendrá las mismas funciones disponibles que la instancia de producción.
* Si crea un programa en el simulador para pruebas y desea moverlo a producción, puede realizar una [importación de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Los entornos limitados están restringidos para que las instancias de producción no se vean afectadas negativamente por los entornos de prueba. Puede enviar hasta 30 correos electrónicos por ejecución de campaña.

>[!CAUTION]
>
>Actualmente no se admite la actualización del simulador para pruebas simultáneas de Marketo Dynamics. Si necesita actualizar el entorno limitado de Dynamics CRM, se necesitará un nuevo entorno limitado de Marketo. Póngase en contacto con el administrador de éxito de los clientes para obtener más información.

## Copia de instancia {#instance-copy}

Puede enviar un caso de asistencia que solicite una copia de instancia única para rellenar el simulador para pruebas. Sin embargo, la copia de instancia no traerá _todo_. Consulte [Compatibilidad con Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obtener más información.

>[!NOTE]
>
>* La copia de instancia es **no** compatible si la instancia de origen está integrada con Microsoft Dynamics.
>* Si está cambiando su CRM nativo, se necesitaría una nueva instancia de Marketo y no sería posible una copia de la instancia a la nueva instancia de Marketo. En su lugar, trabaje con la asistencia de Marketo para explorar la funcionalidad Importar programa .

