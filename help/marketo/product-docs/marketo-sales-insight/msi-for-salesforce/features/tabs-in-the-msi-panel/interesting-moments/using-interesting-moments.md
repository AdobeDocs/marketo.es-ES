---
unique-page-id: 2951640
description: 'Uso de momentos interesantes: documentos de Marketo, documentación del producto'
title: Uso de momentos interesantes
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Uso de momentos interesantes {#using-interesting-moments}

Momentos interesantes son la clave para comunicarse con su equipo de ventas a través de la aplicación [!DNL Marketo Sales Insight].

>[!AVAILABILITY]
>
>Solo están disponibles para [!DNL Marketo Sales Insight] y [[!DNL Marketo Sales Connect]](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) clientes.

## ¿Qué es un momento interesante? {#what-is-an-interesting-moment}

¡Eso depende de ti! Usted decide qué información es relevante para su equipo de ventas. Es posible que el equipo de ventas desee saber cuándo un posible cliente:

* Visita la página de precios del sitio web
* Hace clic en un vínculo de un correo electrónico para anunciar un nuevo producto
* Solicita una demostración del producto

## ¿Cómo puedo crear un momento interesante?  {#how-do-i-create-an-interesting-moment}

1. Elija una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferiblemente una que el equipo de ventas encuentre interesante si se activa.

   ![](assets/using-interesting-moments-1.png)

1. Arrastre sobre el paso de flujo **[!UICONTROL Momentos interesantes]**.

   ![](assets/using-interesting-moments-2.png)

1. Seleccione un **tipo** ([!UICONTROL Correo electrónico], [!UICONTROL Hito] o [!UICONTROL Web]).

   ![](assets/using-interesting-moments-3.png)

1. Escriba un mensaje a su equipo de ventas en el campo **[!UICONTROL Descripción]** que explique por qué es importante esta acción.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo también añadirá la fecha en la que se produjo y cómo se añadió el momento interesante (es decir, acción de posible cliente > paso de flujo, API de SOAP).

## ¿Cómo puede esto ponerse aún más interesante?  {#how-can-this-get-even-more-interesting}

¡Tokens! Añádalos en el campo de descripción para proporcionar a su equipo de ventas información más específica, como la línea de asunto del correo electrónico que abrió el posible cliente o a quién envió. Consulte los tokens que están disponibles para su uso en el glosario de [Tokens for Interested Moments](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md).

>[!TIP]
>
>Comience con cinco momentos interesantes y luego trabaje con su equipo de ventas para determinar qué información le interesa ver.

## ¿Qué aspecto tiene un momento interesante en Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Se mostrarán momentos interesantes en el [registro de actividades del posible cliente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## ¿Qué aspecto tiene un momento interesante en [!DNL Salesforce]?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Una vez que hayas [instalado la [!DNL Marketo Sales Insight] aplicación](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md), se mostrarán momentos interesantes en las páginas de posible cliente, contacto, cuenta u oportunidad. También aparecen en el panel [!DNL Sales Insight] en la fuente de posibles clientes, [!DNL Best Bets] y la lista de observación.

![](assets/using-interesting-moments-6.png)

## ¿Qué aspecto tiene un momento interesante en [!DNL Salesforce1]? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Una vez que haya instalado o actualizado [!DNL Marketo Sales Insight] para [!DNL Salesforce1], los momentos interesantes se mostrarán en los vínculos relacionados con el posible cliente.

![](assets/using-interesting-moments-7.png)

## Suscribirse a momentos interesantes {#subscribe-to-interesting-moments}

Para suscribirse a un momento interesante, haga clic en el botón [!UICONTROL Suscribirse] en la pestaña Momento interesante o en la fuente de posibles clientes. Los pasos siguientes son los mismos para ambos.

1. Haga clic en el icono Subscribe. A continuación, se le dirigirá a la pestaña Suscribirse por correo electrónico.

1. Puede elegir el tipo de alerta por correo electrónico que desea recibir en función de [!UICONTROL Nombre], [!UICONTROL Cuenta], [!UICONTROL Tipo] o [!UICONTROL Descripción].

1. Elija a qué dirección de correo electrónico desea enviar las alertas (usted/los integrantes del equipo)

1. Haga clic en **[!UICONTROL Suscribirse]**.

>[!NOTE]
>
>Al suscribirse a tipos de momentos o descripciones interesantes, el usuario recibe notificaciones por correo electrónico para las personas (posibles clientes o contactos) que sean propietarias cuando almacenen en déclencheur un momento interesante que coincida con ese tipo o descripción.

![](assets/using-interesting-moments-8.png)
