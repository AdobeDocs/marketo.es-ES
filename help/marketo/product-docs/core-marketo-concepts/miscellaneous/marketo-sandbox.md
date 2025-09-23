---
unique-page-id: 11386358
description: Zona protegida de Marketo - Documentos de Marketo - Documentación del producto
title: Zona protegida de Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Zona protegida de Marketo {#marketo-sandbox}

Una zona protegida de Marketo Engage es una instancia adicional que se utiliza con fines de prueba antes de la implementación en el entorno de producción.

>[!AVAILABILITY]
>
>No todos han comprado esta función. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

No se puede sincronizar una zona protegida de Marketo con su CRM normal si ya está sincronizada con su instancia de producción. Utilice la zona protegida de su CRM para la sincronización y siga los mismos pasos que en la sincronización original.

## Cosas que hay que saber sobre Sandboxes {#things-to-know-about-sandboxes}

* Si desea agregar usuarios, el proceso es el mismo que [agregar usuarios en producción](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). De nuevo, deben utilizar una dirección de correo electrónico diferente si ya han iniciado sesión en Marketo.
* La zona protegida de Marketo empezará vacía, pero tendrá las mismas funciones disponibles que la de producción.
* Si crea un programa en su zona protegida y desea moverlo a producción, puede realizar una [importación de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Las zonas protegidas se limitan para que las instancias de producción no se vean afectadas negativamente por los entornos de prueba. Puede enviar hasta 20 correos electrónicos por campaña ejecutada.

>[!CAUTION]
>
>No se admite la actualización de la zona protegida para la sincronización de Salesforce de Marketo Dynamics _o_ en este momento. Si necesita actualizar la zona protegida de CRM, se requiere una nueva zona protegida de Marketo. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Copia de instancia {#instance-copy}

Puede enviar un caso de asistencia técnica solicitando una copia de instancia única para rellenar el espacio aislado. Sin embargo, la copia de instancia no llevará _todo_. Consulte [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obtener más información.

>[!NOTE]
>
>Si está cambiando su CRM nativo, se necesitaría una nueva instancia de Marketo y no sería posible realizar una copia de la instancia a la nueva instancia de Marketo. En su lugar, trabaje con el Soporte de Marketo para explorar la funcionalidad del Programa de importación.
