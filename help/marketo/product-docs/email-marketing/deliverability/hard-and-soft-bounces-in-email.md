---
unique-page-id: 1147328
description: 'Devoluciones duras y leves en correos electrónicos: Documentos de Marketo: Documentación del producto'
title: Devoluciones duras y leves en correo electrónico
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Devoluciones duras y leves en correo electrónico {#hard-and-soft-bounces-in-email}

Un rechazo grave puede hacer que la dirección de correo electrónico de una persona no sea válida cuando un servidor de correo le indica a Marketo que el correo electrónico de la persona no se puede entregar. Un rechazo leve significa que algo salió mal al enviar el correo electrónico a la persona; esto se resuelve automáticamente y a veces puede tardar días. Tanto los rechazos graves como los leves consisten en [varias categorías](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Clasificación de devoluciones {#bounce-classification}

Hay 5 cadenas de personas en Marketo que están relacionadas con la entrega de correo electrónico con problemas.

1. **Correo electrónico suspendido** - Configúrelo en True cuando se produce un determinado tipo de devolución.
1. **Causa de suspensión de correo electrónico** - Puede haber muchas razones. Este campo intenta explicar la causa.
1. **Correo electrónico suspendido en** - Cuando se produce el rechazo ofensivo, Marketo suspenderá el envío a la persona durante 24 horas desde esta marca de tiempo.
1. **Correo electrónico no válido** - Configúrelo en True cuando se produce un determinado tipo de devolución.
1. **Causa no válida de correo electrónico** - La razón de la fuerte devolución.

>[!NOTE]
>
>Después de que una persona alcance **correo electrónico suspendido** , no hay forma de borrar la casilla de verificación de correo electrónico suspendido. Sin embargo, la persona seguirá siendo enviada 24 horas después de la suspensión inicial.
>
>Cuando una persona está marcada como **correo electrónico no válido**, solo se pueden restablecer manualmente (lo que solo se recomienda hacer si sabe que su correo electrónico es válido) desmarcando el cuadro &quot;Correo electrónico no válido&quot; en la pestaña Información de persona de su registro.

>[!PREREQUISITES]
>
>Seguir [estos pasos](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para crear un informe de rendimiento del correo electrónico, que generará datos de devoluciones.

Después de crear el informe Rendimiento del correo electrónico, la pantalla debería tener este aspecto:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Los filtros de correo no deseado a veces crean rechazos graves. Estos &quot;falsos positivos&quot; no indican la verdadera validez de la dirección de correo electrónico de la persona.
