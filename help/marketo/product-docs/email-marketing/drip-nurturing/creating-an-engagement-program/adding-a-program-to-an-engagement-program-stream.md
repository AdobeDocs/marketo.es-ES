---
unique-page-id: 10098134
description: 'Adición de un programa a un flujo de programa de participación: Marketo Docs: documentación del producto'
title: Adición de un programa a un flujo de programa de participación
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Adición de un programa a un flujo de programa de participación {#adding-a-program-to-an-engagement-program-stream}

## ¿Por qué utilizar un programa anidado en una secuencia de programa de participación? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es fácil añadir un correo electrónico a un flujo en un programa de participación, y funciona bien. Sin embargo, si sus necesidades comerciales son más complejas, puede que sea recomendable colocar el correo electrónico dentro de un programa. Por ejemplo, puede que desee:

* Enviar un correo electrónico a un subgrupo de personas del flujo
* Enviar *different* correos electrónicos para subgrupos dentro de la emisión
* Incluir páginas de aterrizaje, formularios u otros recursos en el futuro
* Habilitar atribución multitáctil
* Añadir pasos de flujo adicionales, como correos electrónicos de alerta

## ¿Qué sucede cuando se utiliza un programa en un flujo? {#what-happens-when-you-use-a-program-in-a-stream}

Al utilizar un programa anidado, la decisión de enviar un correo electrónico a una persona se basa en la pertenencia al programa y el ID del programa.

* Si no es miembro de un programa, recibirá cualquier correo electrónico que forme parte del programa una vez
* Si eres miembro del programa, no recibirás el correo electrónico
* Si ya no es miembro pero ha recibido el correo electrónico anteriormente a través de ese programa, no recibirá el correo electrónico

Cuando utiliza un programa en un flujo, no importa si ha recibido antes ese correo electrónico específico. Siempre y cuando el correo electrónico no se haya enviado antes de *en ese programa específico*, puede recibirlo de nuevo.

Puede resultar difícil mezclar correos electrónicos y programas en un programa de participación. Es posible que desee usar una u otra.

>[!TIP]
>
>Asegúrese de utilizar un **Miembro del programa de participación** en la lista inteligente.

## ¿Qué les sucede a las personas que no cumplen los criterios de la lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

En el caso de que alguien quede fuera de la lista inteligente de la campaña inteligente de un programa anidado, no pasará al siguiente fragmento de contenido durante la emisión actual. Pasarán al siguiente fragmento de contenido del flujo para el *following* elástica.

## ¿Qué contiene un programa anidado? {#what-does-a-nested-program-contain}

Un programa anidado bien diseñado contiene correos electrónicos, informes y campañas inteligentes. Tiene sentido mantenerlos juntos.

El correo electrónico que utilice puede residir en el programa, en un programa diferente o incluso en Design Studio. El lugar en el que se encuentre dependerá de cómo lo quiera usar.

Los informes cambian con la ubicación del correo electrónico. Por lo tanto, si el correo electrónico está en Design Studio, en el informe Rendimiento del correo electrónico, todas las métricas se muestran en una línea; se combinan las diferentes emisiones. Sin embargo, en el informe Rendimiento del flujo de participación, los diferentes envíos se muestran por separado.

>[!CAUTION]
>
>Si desea reenviar algo, es más seguro crear un nuevo programa y una campaña inteligente.

>[!MORELIKETHIS]
>
>* [Añadir contenido a un flujo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Explicación de los programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

