---
unique-page-id: 1147328
description: Devoluciones en firme y blandas en correo electrónico - Documentos de marketing - Documentación del producto
title: Devoluciones en firme y blandas en el correo electrónico
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Devoluciones en firme y blandas en el correo electrónico {#hard-and-soft-bounces-in-email}

Una devolución forzada puede hacer que la dirección de correo electrónico de una persona no sea válida cuando un servidor de correo le indica a Marketing que el correo electrónico de la persona no se puede entregar. Una devolución suave significa que algo salió mal al enviar el correo electrónico a la persona; esto se resuelve automáticamente y a veces puede tardar días. Tanto las devoluciones duras como las blandas constan de [varias categorías](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Clasificación de devoluciones {#bounce-classification}

Hay 5 cadenas de personas en Marketing relacionadas con el envío de correo electrónico con problemas.

1. **Correo electrónico suspendido** : defina en True cuando se produzca un determinado tipo de devolución forzada.
1. **Causa** por correo electrónico suspendida: puede haber muchas razones. Este campo intenta explicar la causa.
1. **Correo electrónico suspendido en **- Cuando se produzca la devolución, Marketo suspenderá el envío a la persona durante 24 horas desde esta marca de tiempo.
1. **Correo electrónico no válido** : se establece en True cuando se produce un determinado tipo de devolución forzada.
1. **Causa** no válida de correo electrónico: el motivo de la devolución forzada.

>[!NOTE]
>
>Una vez que una persona llega al estado suspendido **de** correo electrónico, no hay forma de borrar la casilla de verificación suspendida de correo electrónico. Sin embargo, la persona seguirá pudiendo ser enviada 24 horas después de la suspensión inicial.
>
>Cuando una persona se marca como no válida **por** correo electrónico, solo se puede restablecer manualmente (lo que recomendamos que haga sólo si sabe que su correo electrónico es válido) desmarcando el cuadro &quot;Correo electrónico no válido&quot; en la ficha Información de persona de su registro.

>[!PREREQUISITES]
>
>Siga [estos pasos](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para crear un informe de rendimiento de correo electrónico, que generará datos de devoluciones.

Después de crear el informe Rendimiento del correo electrónico, la pantalla debería tener este aspecto: ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Los filtros no deseados a veces crean rebotes duros. Estos &quot;falsos positivos&quot; no son una indicación de la verdadera validez de la dirección de correo electrónico de la persona.

