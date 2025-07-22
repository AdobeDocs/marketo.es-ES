---
unique-page-id: 30082174
description: Momentos interesantes en Sales Connect - Documentos de Marketo - Documentación del producto
title: Momentos interesantes en Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Momentos interesantes en [!DNL Sales Connect] {#interesting-moments-in-sales-connect}

Momentos interesantes son la clave para comunicarse con su equipo de ventas a través de [!DNL Marketo Sales Connect].

>[!AVAILABILITY]
>
>Están disponibles solo para [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) y [!DNL Marketo Sales Connect] clientes.

>[!PREREQUISITES]
>
>* Debe tener una [conexión con Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Debe ser el propietario del contacto o posible cliente de Salesforce
>* Debe tener acceso a [conceder acceso a la conexión de Marketo Engage](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## ¿Qué es un momento interesante? {#what-is-an-interesting-moment}

¡Eso depende de ti! Usted decide qué información es relevante para su equipo de ventas. Es posible que el equipo de ventas desee saber cuándo un posible cliente:

* Visita la página de precios del sitio web
* Hace clic en un vínculo de un correo electrónico para anunciar un nuevo producto
* Solicita una demostración del producto

## ¿Cómo puedo crear un momento interesante? {#how-do-i-create-an-interesting-moment}

1. Elija una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferiblemente una que el equipo de ventas encuentre interesante si se activa.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Arrastre sobre el paso de flujo **[!UICONTROL Momentos interesantes]**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Seleccione un **tipo** ([!UICONTROL Correo electrónico], [!UICONTROL Hito] o [!UICONTROL Web]).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Escriba un mensaje a su equipo de ventas en el campo **[!UICONTROL Descripción]** que explique por qué es importante esta acción.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo también añadirá la fecha en la que se produjo y cómo se añadió el momento interesante (es decir, acción de posible cliente > paso de flujo, API de SOAP).

## ¿Qué aspecto tiene un momento interesante en Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Se mostrarán momentos interesantes en el [registro de actividades del posible cliente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## ¿Qué aspecto tiene un momento interesante en [!DNL Sales Connect]? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Los momentos interesantes se mostrarán en tiempo real en el Live Feed de un usuario. Utilizamos el identificador de propietario del posible cliente de [!DNL Salesforce] para mostrar los momentos interesantes de los usuarios de posibles clientes relevantes de los que son propietarios. Los usuarios pueden realizar un seguimiento rápido con los posibles clientes a través del correo electrónico, el teléfono o la campaña de ventas haciendo clic en la lista desplegable situada junto al nombre del posible cliente.

![](assets/engagement.jpg)
