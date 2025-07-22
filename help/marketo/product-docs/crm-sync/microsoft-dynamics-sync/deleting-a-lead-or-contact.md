---
unique-page-id: 45417322
description: 'Eliminación de un posible cliente o contacto: documentos de Marketo, documentación del producto'
title: Eliminación de un posible cliente o contacto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Eliminación de un posible cliente o contacto {#deleting-a-lead-or-contact}

Hay algunas cosas que se deben saber a la hora de eliminar posibles clientes o contactos en [!DNL Microsoft Dynamics].

* Marketo no elimina a las personas automáticamente solo porque se eliminaron posibles clientes en [!DNL Dynamics]. En su lugar, el indicador del campo &quot;Microsoft is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminar el registro en Marketo.

* Acción de flujo &quot;Eliminar persona&quot;: esto solo elimina una persona en Marketo (no está disponible una opción para eliminarla también en Dynamics).

* Si se elimina un posible cliente en Marketo (pero no en [!DNL Dynamics]) y se actualiza en [!DNL Dynamics] posteriormente, se crearía una nueva persona en Marketo (la misma dirección de correo electrónico, nuevo ID de persona).

* Si se elimina un posible cliente en [!DNL Dynamics] (pero no en Marketo) y posteriormente se ejecuta la acción de flujo &quot;Sincronizar persona con Microsoft&quot;, se crearía un nuevo posible cliente en [!DNL Dynamics].
