---
unique-page-id: 11381156
description: Concordancia de posibles clientes con cuentas - Marketo Docs - Documentación del producto
title: Coincidencia de posibles clientes con cuentas
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Coincidencia de posibles clientes con cuentas {#lead-to-account-matching}

La coincidencia a la derecha lleva a cuentas con el nombre correcto que utilizan la coincidencia de cliente potencial a cuenta de Marketo.

>[!NOTE]
>
>**La** coincidencia entre posibles clientes es una función integrada de Administración de cuentas de Marketo Target. Utiliza lógica borrosa para hacer coincidir automáticamente los posibles clientes con las cuentas con nombre correcto en tiempo casi real. Estas cuentas con nombre podrían ser cuentas CRM o empresas de Marketo.

Marketo Lead-to-Account Matching sigue un proceso de 4 pasos:

**Paso 1:** Nuestro proceso de coincidencia comienza utilizando información clave en los registros de posibles clientes, como:

* Dominio de correo electrónico (por ejemplo, acme.com)
* Nombre de empresa vinculado de la dirección IP
* Nombre de la empresa : Podría ser un nombre de cuenta de CRM o un atributo de nombre de la empresa principal (por ejemplo, vino de rellenar el formulario)

**Paso 2:** normalizamos los nombres de empresas que encontramos en función de varios atributos de posibles clientes (por ejemplo, Acme Inc. y Acme Corp se normalizan automáticamente a Acme). Este paso garantiza que tengamos una sola representación de la cuenta nombrada en Marketo y que podamos ver todos los posibles clientes dentro de una única cuenta con nombre.

**Paso 3:** La partición coincidente de los posibles clientes en 2 bloques: Coincidencia fuerte y coincidencia débil.

* Los posibles clientes con poca coincidencia aparecen en las cuentas con nombre, lo que se puede resolver manualmente.

**Paso 4:** Presentamos una lista de las empresas propuestas con correspondencias fuertes y débiles. Cuando se crea una cuenta con nombre basada en una de las empresas propuestas, se crean reglas de coincidencia para asociar automáticamente nuevos posibles clientes (por ejemplo, los posibles clientes rellenaron un formulario) a las cuentas con nombre correctas. De esta manera puede preocuparse menos por los posibles clientes y más por obtener ingresos.

Dado que la coincidencia de posibles clientes de Marketo con cuentas es una característica integrada de Administración de cuentas de Marketo Target, la coincidencia de posibles clientes se produce casi en tiempo real (por ejemplo, en el momento en que un posible cliente rellena un formulario de Marketo, asociamos dicho posible cliente con la cuenta con nombre correcto). Este evento se puede utilizar para almacenar en déclencheur las alertas y notificar a los propietarios de cuentas los nuevos posibles clientes que llegan desde sus cuentas con nombre.

>[!NOTE]
>
>Si utiliza LeanData en Salesforce para hacer la coincidencia entre posibles clientes y cuentas, Marketo tiene una integración que sincronizará esas coincidencias con su instancia de Marketo. Para habilitar esa función, póngase en contacto con el [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Discover de cuentas](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
