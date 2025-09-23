---
description: Indicadores de campo - Documentos de Marketo - Documentación del producto
title: Indicaciones de campo
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 3%

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
>Cuando se utilizan avisos con campañas de ventas, es mejor usarlos con pasos manuales de correo electrónico. Estos pasos asignarán a un usuario una tarea de recordatorio para enviar el correo electrónico, lo que le ofrece la oportunidad de reemplazar las indicaciones por texto personalizado. Los pasos automáticos del correo electrónico en Campañas de ventas intentarán enviarse automáticamente, sin permitir que el usuario reemplace las indicaciones. Los mensajes que no se sustituyan provocarán que los mensajes de correo electrónico no se envíen.
