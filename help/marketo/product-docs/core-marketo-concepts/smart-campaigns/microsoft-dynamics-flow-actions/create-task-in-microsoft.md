---
unique-page-id: 37356429
description: Crear Tarea en Microsoft - Documentos de marketing - Documentación del producto
title: Crear Tarea en Microsoft
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Crear Tarea en Microsoft {#create-task-in-microsoft}

Como especialista en mercadotecnia, tiene información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan qué deben hacer y cuándo deben hacerlo.

Crear Tarea en Microsoft crea una tarea en Actividades relacionadas con la Persona (posible cliente o contacto) en Microsoft.

>[!NOTE]
>
>Este paso de flujo **solo funcionará cuando se utilice con activadores**, no filtros, en la campaña inteligente.

De forma predeterminada, el paso de flujo tendrá este aspecto:   ![](assets/msd1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de marketing está creando tareas, **Vence en **es un campo obligatorio para la tarea que se va a crear en Microsoft. Marketo ingresará cinco días de forma predeterminada si no se introduce ningún valor.

Personalice todos los campos para crear la tarea como desee.   ![](assets/msd2.png)

>[!NOTE]
>
>El campo &quot;Estado&quot; especificado para la tarea en Acción de flujo actualiza el campo: &quot;Motivo de estado&quot; en Microsoft.

>[!TIP]
>
>Puede utilizar `{{lead.tokens}}`, `{{company.tokens}}``{{campaign.tokens}}` y `{{system.tokens}}` en el **Asunto** y la **Descripción**. Consulte [Tokens para ver los pasos](http://docs.marketo.com/x/c4AR) de flujo para obtener más información.

