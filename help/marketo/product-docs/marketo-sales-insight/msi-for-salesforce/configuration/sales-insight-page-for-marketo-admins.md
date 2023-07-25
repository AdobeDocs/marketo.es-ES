---
unique-page-id: 42762409
description: Página de perspectiva de ventas para administradores de Marketo - Documentos de Marketo - Documentación del producto
title: Página de perspectiva de ventas para administradores de Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---

# Página de perspectiva de ventas para administradores de Marketo {#sales-insight-page-for-marketo-admins}

Los administradores de Marketo tienen ciertos privilegios en Sales Insight. Descubra cuáles son a continuación.

## Configuración de API de SOAP {#soap-api-configuration}

Estas credenciales se utilizan para conectar su cuenta de Salesforce a la instancia de Marketo para utilizar MSI en Salesforce.

![](assets/one-1.png)

## Configuración de API de REST {#rest-api-configuration}

Estas credenciales se utilizan para conectar su cuenta de Salesforce a la instancia de Marketo, para utilizar el panel de información de MSI en Salesforce.

![](assets/two-1.png)

## Configuración de puntuación de persona {#person-score-settings}

* **Estrellas**: Las estrellas representan la puntuación total de posibles clientes en comparación con otros posibles clientes.
* **Llamas**: las llamas representan urgencia, cuánto ha cambiado recientemente la puntuación de un posible cliente.

De forma predeterminada, Marketo Sales Insight utiliza el campo Puntuación de posibles clientes para calcular las estrellas y las llamas. Pero si desea elegir un campo diferente, así es como:

1. En el **Administrador** de Marketo, haga clic en **Perspectiva de ventas**.

   ![](assets/four.png)

1. En Configuración de puntuación de posibles clientes, haga clic en **Editar**.

   ![](assets/five.png)

1. Seleccione el campo que desee utilizar para las estrellas.

   ![](assets/six.png)

1. Seleccione el campo que desee utilizar para las llamas.

   ![](assets/seven.png)

1. Clic **Guardar**. La perspectiva de ventas tardará un tiempo en volver a calcularse. Puede comprobar su CRM más tarde para ver las estrellas y las llamas.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Si aún no tiene los campos de puntuación personalizados, así es como hacerlo [crearlos](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Estrellas y llamas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Configuración {#settings}

![](assets/nine.png)

**Configuración de la cancelación de suscripción:**

Puede elegir entre las siguientes configuraciones para cancelar la suscripción a Sin plantilla, Correos electrónicos estándar y Correos electrónicos operativos

* Respetar configuración de cancelación de suscripción
* Respetar la configuración de cancelación de suscripción cuando más de un destinatario
* Respetar la configuración de cancelación de suscripción cuando más de 5 destinatarios
* Ignorar configuración de cancelación de suscripción

**Habilitar la capacidad de bloquear plantillas:**

Cuando se habilita, los usuarios de MSI no podrán editar las plantillas al enviar correos electrónicos desde Salesforce

**Habilitar fuente RSS:**

Cuando se habilita, los usuarios de MSI pueden ver su fuente de posibles clientes en una fuente RSS (además de la fuente de posibles clientes de Salesforce). La fuente RSS solo puede funcionar si la función &quot;Caducidad del token&quot; está desactivada.

**Vencimiento del token:**

La caducidad del token se controla en el Administrador de funciones. Para habilitarlo o deshabilitarlo, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Cuando se habilita, todos los tokens de Marketo caducan en un plazo de 10 minutos. Cuando está desactivado, los tokens de Marketo no caducan.

Los tokens generados antes de habilitar la caducidad del token no tendrán una hora de caducidad con la que validarse, por lo que no caducarán aunque la función esté habilitada actualmente.

Los tokens generados después de habilitar la caducidad del token tendrán un tiempo de caducidad de 10 minutos, por lo que caducarán en 10 minutos incluso después de que la función esté deshabilitada.

El comportamiento del token se basará en el momento en que se generó (cuando la función de caducidad del token estaba habilitada/deshabilitada, en lugar de su estado actual).
