---
unique-page-id: 11386358
description: Obtenga información sobre la zona protegida de Marketo Engage para pruebas antes de la producción. Utilice una instancia de zona protegida para probar sin afectar a la producción.
title: Zona protegida de Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 3%

---

# Zona protegida de Marketo {#marketo-sandbox}

Una zona protegida de Marketo Engage es una instancia adicional que se utiliza con fines de prueba antes de la implementación en el entorno de producción.

>[!AVAILABILITY]
>
>No todos han comprado esta función. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

No se puede sincronizar una zona protegida de Marketo con su CRM normal si ya está sincronizada con su instancia de producción. Utilice la zona protegida de su CRM para la sincronización y siga los mismos pasos que en la sincronización original.

## Cosas que hay que saber sobre Sandboxes {#things-to-know-about-sandboxes}

* Si desea agregar usuarios, el proceso es el mismo que [agregar usuarios en producción](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). De nuevo, deben utilizar una dirección de correo electrónico diferente si ya han iniciado sesión en Marketo.
* La zona protegida de Marketo empezará vacía, pero tendrá las mismas funciones disponibles que la de producción.
* Si crea un programa en su zona protegida y desea moverlo a producción, puede realizar una [importación de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Las zonas protegidas se limitan para que las instancias de producción no se vean afectadas negativamente por los entornos de prueba. Puede enviar hasta 20 correos electrónicos por campaña ejecutada.

>[!CAUTION]
>
>En este momento no se admite la actualización de la zona protegida para la sincronización de Salesforce de Marketo Dynamics _o_. Si necesita actualizar la zona protegida de CRM, se requiere una nueva zona protegida de Marketo. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Copia de instancia {#instance-copy}

Puede enviar un caso de asistencia técnica solicitando una copia de instancia única para rellenar el espacio aislado. Sin embargo, la copia de instancia no llevará _todo_. Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obtener más detalles.

>[!NOTE]
>
>Si está cambiando su CRM nativo, se necesitaría una nueva instancia de Marketo y no sería posible realizar una copia de la instancia en la nueva instancia de Marketo. En su lugar, trabaje con el Soporte de Marketo para explorar la funcionalidad del Programa de importación.
