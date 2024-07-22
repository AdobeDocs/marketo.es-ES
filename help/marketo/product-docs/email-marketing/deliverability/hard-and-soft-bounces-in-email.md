---
unique-page-id: 1147328
description: 'Devoluciones graves y leves en correos electrónicos: documentos de Marketo, documentación del producto'
title: Devoluciones graves y leves en correos electrónicos
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Devoluciones graves y leves en correos electrónicos {#hard-and-soft-bounces-in-email}

Una devolución grave puede hacer que la dirección de correo electrónico de una persona no sea válida cuando un servidor de correo indica a Marketo que el correo electrónico de la persona no se puede enviar. Un rebote suave significa que hubo un problema al enviar el correo electrónico a la persona; esto se resuelve automáticamente y a veces puede tardar días. Las devoluciones suaves y duras constan de [varias categorías](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Clasificación de rechazo {#bounce-classification}

Hay cadenas de 5 personas en Marketo relacionadas con envíos de correo electrónico con problemas.

1. **Correo electrónico suspendido** - Se establece como Verdadero cuando se produce un determinado tipo de devolución.
1. **Causa suspendida de correo electrónico**: puede haber muchas razones. Este campo intenta explicar la causa.
1. **Correo electrónico suspendido a las**: cuando se produzca el rebote ofensivo, Marketo suspenderá los correos a la persona durante 24 horas a partir de esta marca de tiempo.
1. **Correo electrónico no válido** - Se establece en True cuando se produce un determinado tipo de devolución.
1. **Causa no válida de correo electrónico** - El motivo del rechazo grave.

>[!NOTE]
>
>Una vez que una persona alcanza el estado **correo electrónico suspendido**, no hay forma de borrar la casilla de verificación de correo electrónico suspendido. Sin embargo, la persona seguirá siendo enviada 24 horas después de la suspensión inicial.
>
>Cuando una persona está marcada como **correo electrónico no válido**, solo se puede restablecer de forma manual (lo que recomendamos que lo haga únicamente si sabe con seguridad que su correo electrónico es válido) si desmarca la casilla &quot;Correo electrónico no válido&quot; en la pestaña Información de persona de su registro.

>[!PREREQUISITES]
>
>Siga [estos pasos](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para crear un informe de rendimiento de correo electrónico, el cual generará datos de devoluciones.

Después de crear el informe de rendimiento de correo electrónico, la pantalla debería tener un aspecto similar al siguiente:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Los filtros de correo no deseado a veces crean rechazos graves. Estos &quot;falsos positivos&quot; no indican la verdadera validez de la dirección de correo electrónico de la persona.
