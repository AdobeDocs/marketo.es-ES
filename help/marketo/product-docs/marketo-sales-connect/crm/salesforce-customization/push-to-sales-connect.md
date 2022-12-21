---
unique-page-id: 14352477
description: 'Conexión push a las ventas: Documentos de Marketo: Documentación del producto'
title: Insertar en conexión de ventas
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Insertar en conexión de ventas {#push-to-sales-connect}

Nuestro botón Push to Tout tomará una lista de tus posibles clientes/contactos en Salesforce y los insertará en un grupo en Sales Connect. A continuación, puede enviar rápidamente un correo electrónico de grupo personalizable con el seguimiento de Tout adjunto.

## Requisitos {#requirements}

* Paquete Sales Connect Salesforce instalado por el administrador de Salesforce

* Botón Insertar en venta Conexión instalado para ver la lista por el administrador de Salesforce

* Conexión de Salesforce realizada con Conexión de Ventas para el usuario que realiza la inserción

## Cómo {#how-to}

1. Haga clic en el **Posible cliente/contacto** en Salesforce.
1. Cambie a la Vista de lista que desee insertar en Conexión de ventas junto al botón Ir .
1. Haga clic en **Ir**.
1. Seleccione todos los posibles clientes o contactos a los que desee enviar el mensaje.
1. Select **Insertar en MSE**.
1. Aparecerá una nueva ventana que comprobará el número de posibles clientes o contactos que desea impulsar. Select **Continuar al grupo**. Sales Connect no transferirá ningún contacto marcado como Exclusión de correo electrónico en Salesforce o Cancelación de suscripción en Sales Connect.

   >[!NOTE]
   >
   >Sales Connect agregará este grupo llamado &quot;SFDC-...&quot; a la página Relaciones de la página [aplicación web](https://toutapp.com/login).

1. Select **Enviar correo electrónico a todo el grupo** para enviar este correo electrónico de grupo.
