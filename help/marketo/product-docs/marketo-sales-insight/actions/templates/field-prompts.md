---
description: Obtenga información sobre las solicitudes de campo en las plantillas de correo electrónico. Agregue marcadores de posición que pidan al remitente que rellene contenido personalizado al enviar.
title: Indicaciones de campo
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
TQID: https://experienceleague.adobe.com/ahVbX8SGxaVUjSPsU-1uVc36ecIW60lwYXxDZSxC0kU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 2%

---

# Indicaciones de campo {#field-prompts}

Las indicaciones de campo le permiten añadir una cadena de texto a los correos electrónicos que deben eliminarse o reemplazarse antes de que se puedan enviar. Esta es una buena manera de recordar a los usuarios que deben añadir personalización adicional.

Para agregar un indicador de campo, escriba el texto deseado. Delante de la imagen hay un signo de exclamación y lo rodea con llaves (ver más abajo).

**Ejemplos:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Los usuarios deberán reemplazar este texto con su propia personalización antes de poder enviar el correo electrónico.

![](assets/field-prompts-1.png)

>[!NOTE]
>
>Cuando se utilizan indicaciones con campañas de ventas, es mejor utilizarlas con pasos de correo electrónico manuales. Estos pasos asignarán a un usuario una tarea de recordatorio para enviar el correo electrónico, lo que le ofrece la oportunidad de reemplazar las indicaciones por texto personalizado. Los pasos automáticos del correo electrónico en Campañas de ventas intentarán enviarse automáticamente, sin permitir que el usuario reemplace las indicaciones. Los mensajes que no se sustituyan provocarán que los mensajes de correo electrónico no se envíen.
