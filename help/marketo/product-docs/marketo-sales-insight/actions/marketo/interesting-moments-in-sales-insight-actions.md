---
description: Momentos interesantes en las acciones de información de ventas - Documentos de Marketo - Documentación del producto
title: Momentos interesantes en acciones de información de ventas
exl-id: b2423fbb-9ce0-4ce9-bc26-93aa69aa9e12
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Momentos interesantes en acciones de información de ventas {#interesting-moments-in-sales-insight-actions}

Los momentos interesantes son la clave para comunicarse con su equipo de ventas a través de las acciones de información de ventas de Marketo.

## ¿Qué es un momento interesante? {#what-is-an-interesting-moment}

¡Eso depende de ti! Usted decide qué información es relevante para su equipo de ventas. Es posible que el equipo de ventas desee saber cuándo un posible cliente:

* Visita la página de precios del sitio web
* Hace clic en un vínculo de un correo electrónico para anunciar un nuevo producto
* Solicita una demostración del producto

## ¿Cómo puedo crear un momento interesante? {#how-do-i-create-an-interesting-moment}

1. Elija una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}, preferiblemente una que el equipo de ventas encuentre interesante si se activa.

   ![](assets/interesting-moments-in-sales-insight-actions-1.png)

1. Arrastre sobre el paso de flujo **Momentos interesantes**.

   ![](assets/interesting-moments-in-sales-insight-actions-2.png)

1. Seleccione un **tipo** (correo electrónico, hito o web).

   ![](assets/interesting-moments-in-sales-insight-actions-3.png)

1. Escriba un mensaje a su equipo de ventas en el campo **Descripción** que explique por qué es importante esta acción.

   ![](assets/interesting-moments-in-sales-insight-actions-4.png)

   >[!NOTE]
   >
   >Marketo SOAP también añadirá la fecha en la que se produjo y cómo se añadió el momento interesante (es decir, acción de posible cliente > paso de flujo, API de).

## ¿Qué aspecto tiene un momento interesante en Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Se mostrarán momentos interesantes en el [registro de actividades del posible cliente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

![](assets/interesting-moments-in-sales-insight-actions-5.png)

## ¿Qué aspecto tiene un momento interesante en las acciones de información de ventas? {#what-does-an-interesting-moment-look-like-in-sales-insight-actions}

Los momentos interesantes se mostrarán en tiempo real en el Live Feed de un usuario. Utilizamos el ID del propietario del posible cliente en Salesforce para mostrar los momentos interesantes de los usuarios de posibles clientes relevantes de los que son propietarios. Los usuarios pueden realizar un seguimiento rápido con los posibles clientes a través del correo electrónico, el teléfono o la campaña de ventas haciendo clic en la lista desplegable situada junto al nombre del posible cliente.

![](assets/interesting-moments-in-sales-insight-actions-6.png)
