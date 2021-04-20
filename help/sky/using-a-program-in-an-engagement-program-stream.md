---
title: using-a-program-in-an-engagement-program-stream
description: Uso de un programa en una emisión de programa de participación
exl-id: b75c926d-d545-4557-970f-c893818d9566
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Uso de un programa en una emisión de programa de participación

## ¿Por qué utilizar un programa anidado en una secuencia de programa de participación?

Es fácil añadir un correo electrónico a un flujo en un programa de participación, y funciona bien. Sin embargo, si sus necesidades comerciales son más complejas, puede que sea recomendable colocar el correo electrónico dentro de un programa. Por ejemplo, puede que desee:

* Enviar un correo electrónico a un subgrupo de personas del flujo
* Enviar correos electrónicos _diferentes_ a subgrupos dentro del flujo
* Incluir páginas de aterrizaje, formularios u otros recursos en el programa de participación
* Habilitar atribución multitáctil
* Añadir pasos de flujo adicionales, como correos electrónicos de alerta

## ¿Qué sucede cuando se utiliza un programa en un flujo?

Al utilizar un programa anidado, la decisión de enviar un correo electrónico a una persona se basa en la pertenencia al programa y el ID del programa.

* Si no es miembro del programa, recibirá cualquier correo electrónico que forme parte del programa una vez
* Si es miembro del programa, no recibirá el correo electrónico
* Si ya no es miembro pero ya ha recibido el correo electrónico anteriormente a través de ese programa, no recibirá el correo electrónico

Cuando utiliza un programa en un flujo, no importa si ha recibido antes ese correo electrónico específico. Siempre y cuando el correo electrónico no se haya enviado antes de _en ese programa específico_, puede volver a recibirlo.

Puede resultar difícil mezclar correos electrónicos y programas en un programa de participación. Es posible que desee usar una u otra.

>[!TIP]
>
>Asegúrese de utilizar un filtro Miembro del programa de participación en su lista inteligente.

## ¿Qué les sucede a las personas que no cumplen los criterios de la lista inteligente?

En el caso de que alguien quede fuera de la lista inteligente de la campaña inteligente de un programa anidado, no pasará al siguiente fragmento de contenido durante la emisión actual. Pasarán al siguiente fragmento de contenido del flujo para el _siguiente_ reparto.

## ¿Qué contiene un programa anidado?

Un programa anidado bien diseñado contiene correos electrónicos, informes y campañas inteligentes. Tiene sentido mantenerlos juntos.

El correo electrónico que utilice puede residir en el programa, en un programa diferente o incluso en Design Studio. El lugar en el que vive depende de cómo lo quiera usar.

Los informes cambian con la ubicación del correo electrónico. Por lo tanto, si el correo electrónico está en Design Studio, en el informe Rendimiento del correo electrónico, todas las métricas se muestran en una línea: se combinan las diferentes emisiones. Sin embargo, en el informe Rendimiento del flujo de participación, los diferentes envíos se muestran por separado.

>[!CAUTION]
>
>Si desea reenviar algo, es más seguro crear un nuevo programa y una campaña inteligente.
