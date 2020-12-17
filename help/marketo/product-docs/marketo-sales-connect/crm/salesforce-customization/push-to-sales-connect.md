---
unique-page-id: 14352477
description: Conexión push a ventas - Documentos de marketing - Documentación del producto
title: Conexión push a ventas
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Conexión push a ventas {#push-to-sales-connect}

Nuestro botón Push to Tout tomará una lista de sus posibles clientes/contactos en Salesforce y los insertará en un grupo en Sales Connect. A continuación, puede enviar rápidamente un correo electrónico de grupo personalizable con el seguimiento Tout adjunto.

## Requisitos {#requirements}

* Sales Connect [Paquete de Salesforce](http://docs.marketo.com/x/C4PS) instalado por `Salesforce Admin`

* `Push to Sales Connect`botón instalado en la vista de lista por  `Salesforce Admin`

* Conexión de Salesforce realizada con Sales Connect para que el usuario realice la inserción

## Cómo {#how-to}

1. Haga clic en la ficha **Posible cliente/contacto** en Salesforce.
1. Cambie a la Vista de Lista que desea que Push to Sales Connect junto al botón Ir.
1. Haga clic en **Ir**.
1. Seleccione todos los leads/contactos a los que desee insertar.
1. Seleccione **Insertar en MSE**.
1. Aparecerá una nueva ventana que verifica el número de leads/contactos que desea insertar. Seleccione **Continuar con el grupo**. Sales Connect `will not push over` cualquier contacto marcado como `Email Opt Out` en Salesforce o `Unsubscribed` en Sales Connect.

   >[!NOTE]
   >
   >Sales Connect agregará este grupo llamado &quot;SFDC-...&quot; a la página Relaciones en la [aplicación Web](http://toutapp.com/login).

1. Seleccione **Enviar correo electrónico a todo el grupo** para enviar el correo electrónico de este grupo.

