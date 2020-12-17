---
unique-page-id: 11381156
description: Coincidencia de posibles clientes con cuentas - Documentos de marketing - Documentación del producto
title: Coincidencia de posibles clientes con cuentas
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Coincidencia de posibles clientes con cuentas {#lead-to-account-matching}

La coincidencia a la derecha lleva a las cuentas con nombre a la derecha mediante la coincidencia de posibles clientes de marketing a cuenta.

>[!NOTE]
>
>**La** coincidencia de posibles clientes con cuentas es una característica integrada de la mercadotecnia basada en cuentas de marketing. Utiliza una lógica borrosa para hacer coincidir automáticamente los leads con las cuentas con nombre correctas en tiempo casi real. Estas cuentas con nombre pueden ser cuentas CRM o compañías de marketing.

La coincidencia de posibles clientes con respecto a la cuenta de Marketing sigue un proceso de cuatro pasos:

**Paso 1:** Nuestro proceso de coincidencia comienza con la información clave de los registros de posibles clientes, como:

* Dominio de correo electrónico (por ejemplo, acme.com)
* Nombre de compañía preferido de la dirección IP
* Nombre de la compañía: puede ser el nombre de la cuenta de CRM o el atributo del nombre de la compañía de posible cliente, por ejemplo, proviene del formulario de cumplimentación

**Paso 2:** normalizamos los nombres de compañías que encontramos en función de varios atributos de posibles clientes (por ejemplo, Acme Inc. y Acme Corp se normalizan automáticamente en Acme). Este paso garantiza que contamos con una sola representación de la cuenta con nombre en Marketing y que podemos ver todos los leads dentro de una única cuenta con nombre.

**Paso 3:** Los leads coincidentes de partición se dividen en dos bloques: Coincidencia fuerte y coincidencia débil.

* Los posibles clientes que no coinciden aparecen en las cuentas con nombre, lo que puede resolverse manualmente.

**Paso 4 -** Presentamos una lista de compañías propuestas con coincidencias fuertes y débiles. Cuando se crea una cuenta con nombre basada en una de las compañías propuestas, creamos reglas de coincidencia para asociar automáticamente nuevos leads (por ejemplo, posibles clientes rellenados en un formulario) a las cuentas con nombre correctas. De este modo, puede preocuparse menos por los posibles clientes coincidentes y más por obtener ingresos.

Dado que la coincidencia de posibles clientes de marketing con cuentas es una característica integrada de Marketing basado en cuentas de marketing, la coincidencia de leads con cuentas se produce en tiempo casi real (por ejemplo, en el momento en que un posible cliente rellena un formulario de marketing, asociamos dicho posible cliente con la cuenta con el nombre correcto). Este evento se puede utilizar para activar alertas y notificar a los propietarios de cuentas los nuevos posibles clientes que ingresan desde sus cuentas con nombre.

>[!NOTE]
>
>Si usa LeanData en Salesforce para hacer la coincidencia de posibles clientes con cuentas, Marketing tiene una integración que sincronizará esas coincidencias con su instancia de Marketing. Para habilitar esa función, póngase en contacto con [Soporte técnico de Marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>* [Cuentas de Discover](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)

