---
unique-page-id: 45417322
description: Comprender cómo funciona la eliminación de contactos y posibles clientes entre Microsoft Dynamics y Marketo. Utilice el indicador Microsoft is Deleted y la acción de flujo Delete Person según sea necesario.
title: Eliminación de un posible cliente o contacto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 6%

---

# Eliminación de un posible cliente o contacto {#deleting-a-lead-or-contact}

Hay algunas cosas que se deben saber a la hora de eliminar posibles clientes o contactos en [!DNL Microsoft Dynamics].

* Marketo no elimina a las personas automáticamente solo porque se eliminaron posibles clientes en [!DNL Dynamics]. En su lugar, el indicador del campo &quot;Microsoft is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminar el registro en Marketo.

* Acción de flujo &quot;Eliminar persona&quot;: esto solo elimina una persona en Marketo (no está disponible una opción para eliminarla también en Dynamics).

* Si se elimina un posible cliente en Marketo (pero no en [!DNL Dynamics]) y se actualiza en [!DNL Dynamics] posteriormente, se crearía una nueva persona en Marketo (la misma dirección de correo electrónico, nuevo ID de persona).

* Si se elimina un posible cliente en [!DNL Dynamics] (pero no en Marketo) y posteriormente se ejecuta la acción de flujo &quot;Sincronizar persona con Microsoft&quot;, se crearía un nuevo posible cliente en [!DNL Dynamics].
