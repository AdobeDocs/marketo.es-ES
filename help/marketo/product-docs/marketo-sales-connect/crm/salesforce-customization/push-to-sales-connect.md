---
unique-page-id: 14352477
description: 'Push to Sales Connect: documentación de Marketo: documentación del producto'
title: Insertar en Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Insertar en Sales Connect {#push-to-sales-connect}

Nuestro botón Push to Tout llevará una lista de sus posibles clientes/contactos en Salesforce y los incluirá en un grupo en Sales Connect. A continuación, puede enviar rápidamente un correo electrónico de grupo personalizable con seguimiento de Tout adjunto.

## Requisitos {#requirements}

* Paquete de Salesforce de Sales Connect instalado por el administrador de Salesforce

* Pulse el botón Conexión de ventas instalado en la vista de lista por el administrador de Salesforce

* Conexión de Salesforce realizada con Sales Connect para que el usuario realice la notificación push

## Cómo. {#how-to}

1. Haga clic en la ficha **posible cliente/contacto** de Salesforce.
1. Cambie a la vista de lista que desee insertar en Sales Connect junto al botón Ir.
1. Haga clic en **Ir**.
1. Seleccione todos los posibles clientes o contactos a los que desee enviar un mensaje de exclusión.
1. Seleccione **Insertar en MSE**.
1. Aparecerá una nueva ventana que verifica el número de posibles clientes/contactos que desea insertar. Seleccione **Continuar con el grupo**. Sales Connect no inserta ningún contacto marcado como Exclusión por correo electrónico en Salesforce o Cancelación de la suscripción en Sales Connect.

   >[!NOTE]
   >
   >Sales Connect agregará este grupo denominado &quot;SFDC-...&quot; a la página Relaciones de la [aplicación web](https://toutapp.com/login).

1. Seleccione **Enviar correo electrónico a todo el grupo** para enviar este correo electrónico de grupo.
