---
unique-page-id: 45417322
description: 'Eliminación de un posible cliente o contacto: Documentos de Marketo: Documentación del producto'
title: Eliminación de un posible cliente o contacto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Eliminación de un posible cliente o contacto {#deleting-a-lead-or-contact}

Hay algunas cosas que hay que saber cuando se trata de eliminar posibles clientes o contactos en Microsoft Dynamics.

* Marketo no elimina automáticamente a las personas solo porque se eliminaron posibles clientes en Dynamics. En su lugar, el indicador de campo &quot;Microsoft es eliminado&quot; se establece en verdadero. Puede desactivar este campo para eliminar el registro en Marketo si lo desea.

* Acción de flujo &quot;Eliminar persona&quot;: Esto solo elimina a una persona en Marketo (una opción para eliminarla también en Dynamics no está disponible).

* Si un posible cliente se elimina en Marketo (pero no en Dynamics) y se actualiza en Dynamics después de eso, se crearía una nueva persona en Marketo (misma dirección de correo electrónico, nuevo ID de persona).

* Si se elimina un posible cliente en Dynamics (pero no en Marketo) y luego se ejecuta a través de la acción de flujo &quot;Sincronizar persona con Microsoft&quot;, se crearía un nuevo posible cliente en Dynamics.
