---
unique-page-id: 10098134
description: 'Añadir un Programa a un flujo de Programa de participación: Documentos de marketing: Documentación del producto'
title: Añadir un Programa en un flujo de Programa de participación
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Añadir un Programa en un flujo de Programa de participación {#adding-a-program-to-an-engagement-program-stream}

## ¿Por qué utilizar un programa anidado en un flujo de programas de participación? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es fácil agregar un correo electrónico a un flujo en un programa de participación, y funciona bien. Sin embargo, si sus necesidades comerciales son más complejas, puede que tenga sentido colocar el correo electrónico dentro de un programa. Por ejemplo, puede que desee:

* Envío de un correo electrónico a un subgrupo de personas del flujo
* Envío de *distintos* correos electrónicos a subgrupos dentro del flujo
* Incluir páginas de aterrizaje, formularios u otros recursos en la alimentación
* Habilitar atribución multitáctil
* Añadir pasos de flujo adicionales, como correos electrónicos de alerta

## ¿Qué ocurre cuando se utiliza un programa en un flujo? {#what-happens-when-you-use-a-program-in-a-stream}

Cuando se utiliza un programa anidado, la decisión de enviar un correo electrónico a una persona se basa en la pertenencia al programa y en el ID de programa.

* Si no es miembro de un programa, recibirá cualquier correo electrónico que forme parte del programa una vez
* Si eres miembro del programa, no recibirás el correo electrónico
* Si ya no eres miembro pero has recibido el correo electrónico anteriormente a través de ese programa, no recibirás el correo electrónico

Cuando se utiliza un programa en un flujo, no importa si ya ha recibido ese correo electrónico específico anteriormente. Siempre y cuando el correo electrónico no se haya enviado antes *en ese programa* específico, puede volver a recibirlo.

Puede resultar complicado mezclar correos electrónicos y programas en un programa de participación. Es posible que desee usar uno u otro.

>[!TIP]
>
>Asegúrese de utilizar un filtro de Programa **** Miembro de compromiso en su lista inteligente.

## ¿Qué pasa con las personas que no cumplen los criterios de lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

En el evento de que alguien se filtra fuera de la lista inteligente de la campaña inteligente de un programa anidado, no pasa al siguiente contenido durante la conversión actual. Pasarán al siguiente contenido del flujo para el *siguiente* lanzamiento.

## ¿Qué contiene un programa anidado? {#what-does-a-nested-program-contain}

Un programa anidado bien diseñado contiene correos electrónicos, informes y campañas inteligentes. Tiene sentido mantenerlos juntos.

El correo electrónico que utilice puede residir en el programa, en un programa diferente o incluso en Design Studio. El lugar donde vive dependerá de cómo lo queramos usar.

El sistema de informes cambia con la ubicación del correo electrónico. Así, por ejemplo, si el correo electrónico está en Design Studio, en el informe Rendimiento del correo electrónico, todas las métricas se muestran en una línea: se combinan las diferentes emisiones. Sin embargo, en el informe Rendimiento del flujo de participación, los diferentes envíos se muestran por separado.

>[!CAUTION]
>
>Si quieres reenviar algo, es más seguro crear un nuevo programa y una campaña inteligente.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Añadir contenido en un flujo](add-content-to-a-stream.md)
>* [Explicación de los Programas](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

>



