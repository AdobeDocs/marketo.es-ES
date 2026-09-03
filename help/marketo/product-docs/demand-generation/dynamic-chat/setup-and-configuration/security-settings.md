---
description: Obtenga información sobre cómo configurar la seguridad de Dynamic Chat con dominios bloqueados o permitidos. Restrinja qué dominios de correo electrónico ven los agentes y qué sitios pueden utilizar el script de chat.
title: Configuración de seguridad
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# Configuración de seguridad {#security-settings}

En Configuración de seguridad, puede agregar dominios a una lista de permitidos bloqueada o bloqueada.

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>El filtrado Bloquear y Permitir dominio del correo electrónico solo se aplica cuando un visitante introduce su dirección de correo electrónico directamente en Dynamic Chat, ya sea en el bot de chat o en un flujo conversacional. No se aplica a las direcciones de correo electrónico que Dynamic Chat recibe de productos integrados, como Marketo Engage. Para obtener más información, consulte la tabla siguiente.

| Escenario | ¿Se aplica el filtrado? |
|---|---|
| El visitante escribe su correo electrónico directamente en el bot de chat de Dynamic Chat | Sí |
| El visitante escribe su correo electrónico directamente en un flujo conversacional de Dynamic Chat | Sí |
| El correo electrónico se rellena previamente desde un envío de formulario de Marketo (el flujo de conversación aparece después de rellenar el formulario) | No |
| El correo electrónico se pasa a Dynamic Chat desde cualquier otro sistema integrado | No |

## Dominios de correo electrónico bloqueados {#blocked-email-domains}

Si hay visitantes con dominios de correo electrónico con los que no desea que interactúen sus agentes (por ejemplo, un competidor), agregue su dominio de correo electrónico a la lista de bloqueados.

1. Seleccione el regulador **Habilitar validación** para activar la lista de bloqueados. Introduce hasta 50 dominios y haz clic en **Guardar**.

   ![](assets/security-settings-2.png)

## Dominios permitidos {#allowed-domains}

Añadir los dominios permitidos garantiza que terceros no puedan crear secuencias de comandos de JavaScript desde el sitio ni añadirlas a las suyas.

1. Seleccione el regulador **Habilitar validación** para activar la lista de permitidos. Introduce los dominios permitidos y haz clic en **Guardar**.

   ![](assets/security-settings-3.png)
