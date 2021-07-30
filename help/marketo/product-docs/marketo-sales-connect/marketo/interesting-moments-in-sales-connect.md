---
unique-page-id: 30082174
description: Momentos interesantes en Sales Connect - Documentos de Marketo - Documentación del producto
title: Momentos interesantes en la conexión de ventas
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
source-git-commit: b18b2172e2c20cdb740854924a48fc996caf59f9
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Momentos interesantes en la conexión de ventas {#interesting-moments-in-sales-connect}

Los momentos interesantes son la clave para comunicarse con su equipo de ventas a través de Marketo Sales Connect.

>[!AVAILABILITY]
>
>Están disponibles solo para los clientes de [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) y Marketo Sales Connect .

## ¿Qué es un momento interesante? {#what-is-an-interesting-moment}

¡Eso depende de ti! Usted decide qué información es relevante para su equipo de ventas. Es posible que el equipo de ventas desee saber cuándo un posible cliente:

* Visita la página de precios de su sitio web
* Hace clic en un vínculo de un nuevo correo electrónico de anuncio de producto
* Solicita una demostración de producto

## ¿Cómo creo un momento interesante? {#how-do-i-create-an-interesting-moment}

1. Elija una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferiblemente una que su equipo de ventas encontrará interesante si se activa.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Arrastre el paso de flujo **Momentos interesantes**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Seleccione un **tipo** (Correo electrónico, Milestone o Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Escriba un mensaje al equipo de ventas en el campo **Description** que explique por qué esta acción importa.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo también agregará la fecha en la que se produjo y cómo se añadió el momento interesante (es decir, acción del posible cliente > paso del flujo, API SOAP).

## ¿Cómo se ve un momento interesante en Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Los momentos interesantes se mostrarán en un [registro de actividades del posible cliente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## ¿Qué aspecto tiene un momento interesante en Sales Connect? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Los momentos interesantes se mostrarán en tiempo real en la fuente en directo de un usuario. Utilizamos el ID de propietario principal de Salesforce para mostrar a los usuarios momentos interesantes de posibles clientes relevantes de los que son propietarios. Los usuarios pueden realizar un seguimiento rápido de los posibles clientes a través de la campaña de correo electrónico/teléfono/ventas haciendo clic en la lista desplegable situada junto al nombre del posible cliente.

![](assets/engagement.jpg)
