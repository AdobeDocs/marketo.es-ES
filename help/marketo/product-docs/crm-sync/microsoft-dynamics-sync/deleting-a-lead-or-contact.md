---
unique-page-id: 45417322
description: Eliminación de un posible cliente o contacto - Documentos de marketing - Documentación del producto
title: Eliminación de un posible cliente o contacto
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Eliminación de un posible cliente o contacto {#deleting-a-lead-or-contact}

Hay algunas cosas que saber a la hora de eliminar leads/contactos en Microsoft Dynamics.

-Marketing no elimina automáticamente a las personas solo porque se eliminaron los leads en Dynamics. En su lugar, el indicador de campo &quot;Microsoft se elimina&quot; se establece en true. Si lo desea, puede activar este campo para eliminar el registro en Marketing.

- Acción de flujo &quot;Eliminar persona&quot;: Esto solo elimina a una persona de Marketing (no hay una opción disponible para eliminarlos también en Dynamics).

-Si se elimina un posible cliente en Marketing (pero no en Dynamics) y se actualiza en Dynamics después, se creará una nueva persona en Marketing (misma dirección de correo electrónico, nuevo ID de persona).

-Si se elimina un posible cliente en Dynamics (pero no en Marketing) y luego se ejecuta mediante la acción de flujo &quot;Sincronizar persona con Microsoft&quot;, se crearía un nuevo posible cliente en Dynamics.
