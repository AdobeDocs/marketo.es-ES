---
unique-page-id: 11381156
description: Coincidencia de clientes potenciales con cuentas - Documentos de Marketo - Documentación del producto
title: Coincidencia de cliente potencial con cuenta
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Coincidencia de cliente potencial con cuenta {#lead-to-account-matching}

El derecho de coincidencia lleva a las cuentas con nombre correcto mediante la coincidencia de cliente potencial con cuenta de Marketo.

>[!NOTE]
>
>**Coincidencia de cliente potencial con cuenta** es una función integrada de Marketo Target Account Management. Utiliza lógica difusa para hacer coincidir automáticamente los posibles clientes con las cuentas con nombre correcto en tiempo casi real. Estas cuentas con nombre pueden ser cuentas de CRM o empresas de Marketo.

## Información general {#overview}

La coincidencia de cliente potencial con cuenta de Marketo sigue un proceso de 4 pasos:

**Paso 1:** Nuestro proceso de coincidencia comienza con el uso de información clave en los registros de posibles clientes, como:

* Dominio de correo electrónico (por ejemplo, acme.com)
* Nombre de empresa deducido de la dirección IP
* Nombre de la empresa: podría ser un nombre de cuenta de CRM o un atributo de nombre de empresa del posible cliente (por ejemplo, procede de la cumplimentación del formulario)

**Paso 2:** Normalizamos los nombres de las empresas que encontramos en función de varios atributos de posibles clientes (por ejemplo, Acme Inc. y Acme Corp se normalizan automáticamente a Acme). Este paso garantiza que tengamos una sola representación de la cuenta con nombre en Marketo y que podamos ver todos los posibles clientes dentro de una sola cuenta con nombre.

**Paso 3:** Dividimos los posibles clientes coincidentes en 2 bloques: Coincidencia fuerte y Coincidencia débil.

* Los posibles clientes no coincidentes aparecen en las cuentas con nombre, que se pueden resolver manualmente.

**Paso 4:** Presentamos una lista de empresas propuestas con coincidencias fuertes y débiles. Cuando se crea una cuenta con nombre basada en una de las empresas propuestas, creamos reglas de coincidencia para asociar automáticamente nuevos posibles clientes (por ejemplo, los posibles clientes rellenados en un formulario) a las cuentas con nombre correctas. De este modo, puede preocuparse menos por la coincidencia de posibles clientes y más por obtener ingresos.

Dado que la coincidencia de cliente potencial con cuenta de Marketo es una función integrada de Marketo Target Account Management, la coincidencia de clientes potenciales con cuentas se produce en tiempo casi real (por ejemplo, en el momento en que un posible cliente rellena un formulario de Marketo, asociamos dicho posible cliente con la cuenta con el nombre correcto). Este evento se puede utilizar para almacenar en déclencheur las alertas y notificar a los propietarios de cuentas los nuevos posibles clientes que llegan desde sus cuentas con nombre.

>[!NOTE]
>
>Si utiliza LeanData en Salesforce para hacer correspondencias de cliente potencial con cuenta, Marketo tiene una integración que sincronizará esas coincidencias con su instancia de Marketo. Para activar esta función, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) Aprenda a configurar LeanData a continuación.

## Uso de LeanData para la coincidencia de cliente potencial con cuenta {#using-leandata-for-lead-to-account-matching}

Después [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) ha habilitado LeanData para su cuenta, siga los pasos a continuación para configurarlo.

1. En Salesforce, haga clic **Configurar inicio** en la barra de navegación izquierda.

1. En la barra de navegación izquierda, debajo de Administración, haga clic en **Usuarios** entonces **Perfiles**.

1. Busque y seleccione el **Sincronización de Marketo** perfil.

1. Desplácese hacia abajo hasta la sección Seguridad de nivel de campo y busque el objeto Posible cliente. Seleccionar **Ver**.

1. Para el nombre de campo &quot;Cuenta coincidente de creación de informes&quot;, asegúrese de que la casilla de verificación del **Acceso de lectura** está seleccionada.

1. En Marketo, vaya a **Administrador** sección.

   ![](assets/lead-to-account-matching-1.png)

1. Seleccionar **Administración de campos**.

   ![](assets/lead-to-account-matching-2.png)

1. Confirme que el campo está allí buscando &quot;Cuenta coincidente de creación de informes&quot;.

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Detectar cuentas](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
