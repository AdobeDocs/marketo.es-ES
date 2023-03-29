---
unique-page-id: 11386358
description: 'Simulador para pruebas de Marketo: Documentos de Marketo: Documentación del producto'
title: Simulador para pruebas de Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Simulador para pruebas de Marketo {#marketo-sandbox}

Un simulador para pruebas de Marketo es una instancia adicional que se utiliza con fines de prueba antes de la implementación en el entorno de producción.

>[!AVAILABILITY]
>
>No todos han comprado esta función. Póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas) para obtener más información.

Un simulador para pruebas de Marketo no se puede sincronizar con el CRM normal si ya está sincronizado con la instancia de producción. Utilice el simulador para pruebas de CRM para la sincronización y siga los mismos pasos que la sincronización original.

## Aspectos importantes de los entornos limitados {#things-to-know-about-sandboxes}

* Una vez que el equipo de cuentas de Adobe ha configurado el simulador para pruebas y le envía la invitación, debe utilizar una dirección de correo electrónico diferente para iniciar sesión que la instancia de producción de Marketo.
* Si desea agregar usuarios, el proceso es el mismo que [adición de usuarios en producción](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). De nuevo, deben utilizar una dirección de correo electrónico diferente si ya tienen un inicio de sesión en Marketo.
* El simulador para pruebas de Marketo comenzará vacío, pero tendrá las mismas funciones disponibles que la instancia de producción.
* Si crea un programa en el simulador para pruebas y desea moverlo a producción, puede realizar una [importación de programas](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Los entornos limitados están restringidos para que las instancias de producción no se vean afectadas negativamente por los entornos de prueba. Puede enviar hasta 20 correos electrónicos por ejecución de campaña.

>[!CAUTION]
>
>Actualmente no se admite la actualización de entornos limitados para Marketo Dynamics Sync. Si necesita actualizar el simulador para pruebas de Dynamics CRM, se necesitará un nuevo simulador para pruebas de Marketo. Póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas) para obtener más información.

## Copia de instancia {#instance-copy}

Puede enviar un caso de asistencia que solicite una copia de instancia única para rellenar el simulador para pruebas. La copia de instancia no se recuperará _todo_, sin embargo. Consulte [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obtener más información.

>[!NOTE]
>
>Si está cambiando su CRM nativo, se necesitaría una nueva instancia de Marketo y no sería posible una copia de instancia a la nueva instancia de Marketo. En su lugar, trabaje con el equipo de asistencia de Marketo para explorar la funcionalidad Importar programa .
