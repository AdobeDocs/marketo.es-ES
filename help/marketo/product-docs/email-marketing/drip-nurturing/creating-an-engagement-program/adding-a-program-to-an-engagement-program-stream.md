---
unique-page-id: 10098134
description: Obtenga información sobre los programas anidados en flujos de participación y cuándo utilizarlos. Agregue programas para subgrupos, pasos de varios contactos y de flujo adicional.
title: Adición de un programa a un flujo de programa de participación
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/kI2v6drF78DnJhhEbgeVSi4TYbF5rExY2wgR0aAK-bI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 477
ht-degree: 4%

---

# Adición de un programa a un flujo de programa de participación {#adding-a-program-to-an-engagement-program-stream}

## ¿Por qué utilizar un programa anidado en un flujo de programa de participación? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es fácil añadir un correo electrónico a un flujo en un programa de participación y funciona bien. Sin embargo, si las necesidades de su empresa son más complejas, puede tener sentido colocar el correo electrónico dentro de un programa. Por ejemplo, es posible que desee:

* Enviar un correo electrónico a un subgrupo de personas en el flujo
* Enviar *correos electrónicos diferentes* a subgrupos dentro del flujo
* Incluir páginas de aterrizaje, formularios u otros recursos en el entorno de
* Habilitar la atribución multitáctil
* Añadir pasos de flujo adicionales, como correos electrónicos de alerta

## ¿Qué sucede cuando se utiliza un programa en una secuencia? {#what-happens-when-you-use-a-program-in-a-stream}

Cuando se utiliza un programa anidado, la decisión de enviar un correo electrónico a una persona se basa en la pertenencia al programa y el ID de programa.

* Si no es miembro de un programa, recibirá cualquier correo electrónico que forme parte del programa una vez
* Si es miembro del programa, no recibirá el correo electrónico
* Si ya no es miembro pero recibió el correo electrónico anteriormente a través de ese programa, no recibirá el correo electrónico

Cuando utiliza un programa en un flujo, no importa si ya ha recibido ese correo electrónico específico anteriormente. Siempre que el correo electrónico no se haya enviado antes de *en ese programa específico*, puede recibirlo de nuevo.

Puede resultar difícil mezclar correos electrónicos y programas en un programa de participación. Es posible que desee utilizar una o la otra.

>[!TIP]
>
>Asegúrese de usar un filtro de **[!UICONTROL Miembro del programa de participación]** en la lista inteligente.

## ¿Qué les sucede a las personas que no cumplen los criterios de las listas inteligentes? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

En caso de que alguien se filtre de la lista inteligente de la campaña inteligente de un programa anidado, no pasa al siguiente fragmento de contenido durante el reparto actual. Pasarán al siguiente fragmento de contenido del flujo para el *siguiente* reparto.

## ¿Qué contiene un programa anidado? {#what-does-a-nested-program-contain}

Un programa anidado bien diseñado contiene correos electrónicos, informes y campañas inteligentes. Tiene sentido mantener estas cosas juntas.

El correo electrónico que uses puede estar en el programa, en un programa diferente o incluso en [!UICONTROL Design Studio]. El lugar donde se encuentre dependerá de cómo desee usarlo.

Informes de cambios con la ubicación del correo electrónico. Por ejemplo, si el correo electrónico se encuentra en [!UICONTROL Design Studio], en el informe de rendimiento del correo electrónico, todas las métricas se mostrarán en una línea: se combinarán las diferentes conversiones. Sin embargo, en el informe Rendimiento del flujo de participación, los diferentes envíos se muestran por separado.

>[!CAUTION]
>
>Si desea reenviar algo, lo más seguro es crear un nuevo programa y una campaña inteligente.

>[!MORELIKETHIS]
>
>* [Añadir contenido a un flujo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Explicación de programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
