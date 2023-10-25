---
unique-page-id: 45417322
description: 'Eliminación de un posible cliente o contacto: documentos de Marketo, documentación del producto'
title: Eliminación de un posible cliente o contacto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Eliminación de un posible cliente o contacto {#deleting-a-lead-or-contact}

Hay algunas cosas que hay que saber cuando se trata de eliminar posibles clientes o contactos en Microsoft Dynamics.

* El Marketo Engage no elimina automáticamente a las personas solo porque se eliminaron posibles clientes en Dynamics. En su lugar, el indicador del campo &quot;Microsoft is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminar el registro en Marketo.

* Acción de flujo &quot;Eliminar persona&quot;: esto solo elimina una persona en Marketo (no está disponible una opción para eliminarla también en Dynamics).

* Si un posible cliente se elimina en Marketo (pero no en Dynamics) y se actualiza en Dynamics después, se crearía una nueva persona en Marketo (la misma dirección de correo electrónico, nuevo ID de persona).

* Si un posible cliente se elimina en Dynamics (pero no en Marketo) y luego se ejecuta a través de la acción de flujo &quot;Sincronizar persona con Microsoft&quot;, se crearía un nuevo posible cliente en Dynamics.
