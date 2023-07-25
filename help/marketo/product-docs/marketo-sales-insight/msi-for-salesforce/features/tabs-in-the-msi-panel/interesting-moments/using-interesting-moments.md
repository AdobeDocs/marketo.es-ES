---
unique-page-id: 2951640
description: 'Uso de momentos interesantes: documentos de Marketo, documentación del producto'
title: Uso de momentos interesantes
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Uso de momentos interesantes {#using-interesting-moments}

Los momentos interesantes son la clave para comunicarse con su equipo de ventas a través de la aplicación Marketo Sales Insight.

>[!AVAILABILITY]
>
>Están disponibles para Marketo Sales Insight y [Marketo Sales Connect](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) solo para clientes de.

## ¿Qué es un momento interesante? {#what-is-an-interesting-moment}

¡Eso depende de ti! Usted decide qué información es relevante para su equipo de ventas. Es posible que el equipo de ventas desee saber cuándo un posible cliente:

* Visita la página de precios del sitio web
* Hace clic en un vínculo de un correo electrónico para anunciar un nuevo producto
* Solicita una demostración del producto

## ¿Cómo puedo crear un momento interesante?  {#how-do-i-create-an-interesting-moment}

1. Elija una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferiblemente uno que el equipo de ventas encontraría interesante si se activa.

   ![](assets/using-interesting-moments-1.png)

1. Arrastre el cursor sobre **Momentos interesantes** paso de flujo.

   ![](assets/using-interesting-moments-2.png)

1. Seleccione una **type** (Correo electrónico, Hito o Web).

   ![](assets/using-interesting-moments-3.png)

1. Escriba un mensaje a su equipo de ventas en la **Descripción** que explica por qué importa esta acción.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo también añadirá la fecha en la que se produjo y cómo se añadió el momento interesante (es decir, acción de posible cliente > paso de flujo, API de SOAP).

## ¿Cómo puede esto ponerse aún más interesante?  {#how-can-this-get-even-more-interesting}

Tokens! Añádalos en el campo de descripción para proporcionar a su equipo de ventas información más específica, como la línea de asunto del correo electrónico que abrió el posible cliente o a quién envió. Consulte qué tokens están disponibles para su uso en [Tokens para momentos interesantes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) glosario.

>[!TIP]
>
>Comience con cinco momentos interesantes y luego trabaje con su equipo de ventas para determinar qué información le interesa ver.

## ¿Qué aspecto tiene un momento interesante en Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Los momentos de interés se mostrarán en una [registro de actividades del posible cliente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## ¿Qué aspecto tiene un momento interesante en Salesforce?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Una vez que haya [ha instalado la aplicación de Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md), se mostrarán momentos interesantes en las páginas de posible cliente, contacto, cuenta u oportunidad. También aparecen en el panel de información de ventas en la fuente de posibles clientes, las opciones más probables y la lista de observación.

![](assets/using-interesting-moments-6.png)

## ¿Qué aspecto tiene un momento interesante en Salesforce1? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Después de instalar o actualizar Marketo Sales Insight para Salesforce1, se mostrarán momentos interesantes en los vínculos relacionados con el posible cliente.

![](assets/using-interesting-moments-7.png)

## Suscribirse a momentos interesantes {#subscribe-to-interesting-moments}

Para suscribirse a un momento interesante, haga clic en el botón Suscribirse en la pestaña Momento interesante o en la fuente de posibles clientes. Los pasos siguientes son los mismos para ambos.

1. Haga clic en el icono Subscribe. A continuación, se le dirigirá a la pestaña Suscribirse por correo electrónico.

1. Puede elegir el tipo de alerta por correo electrónico que desea recibir en función del nombre, la cuenta, el tipo o la descripción.

1. Elija a qué dirección de correo electrónico desea enviar las alertas (usted/los integrantes del equipo)

1. Clic **Suscribirse**.

>[!NOTE]
>
>Al suscribirse a tipos de momentos o descripciones interesantes, el usuario recibe notificaciones por correo electrónico para las personas (posibles clientes o contactos) que sean propietarias cuando almacenen en déclencheur un momento interesante que coincida con ese tipo o descripción.

![](assets/using-interesting-moments-8.png)
