---
unique-page-id: 14746188
description: 'Sincronización de cancelaciones de suscripción con Salesforce: documentación de Marketo: documentación del producto'
title: Sincronización de cancelaciones de suscripción con Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 5%

---

# Sincronización de cancelaciones de suscripción con Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisitos para las cancelaciones de suscripción a la sincronización con Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronización de cancelación de suscripción debe estar habilitada (para sincronización nocturna)
* El campo de exclusión debe estar instalado en Salesforce
* Los registros de persona en Sales Connect deben tener un ID de Salesforce

**Cancelaciones de suscripción push**

Cuando se recopila una cancelación de suscripción en Sales Connect, se envía a Salesforce en tiempo real y se actualiza cualquiera de los campos de exclusión seleccionados para la sincronización. Si ha desactivado la sincronización de Salesforce, aún insertaremos la opción de cancelación de suscripción en la opción de exclusión de correo electrónico.

**Cancelar suscripción a sincronización**

Cuando haya habilitado la sincronización de cancelación de suscripción (Paso 3 a continuación), activará la sincronización nocturna. La sincronización se produce una vez al día alrededor de las 20:00 PST. Sincronizará bidireccionalmente todas las cancelaciones de suscripción en Marketo Sales con el campo de exclusión de Salesforce.

## Configurar la sincronización de cancelación de suscripción a Salesforce {#configure-unsubscribe-sync-to-salesforce}

Los usuarios pueden decidir si desean sincronizar sus cancelaciones de suscripción con el campo de exclusión de correo electrónico estándar con el que Marketo también puede sincronizarse, o pueden sincronizar con el campo de exclusión de ventas de Marketo para poder diferenciar las cancelaciones de suscripción de ventas y las de marketing.

1. Vaya a la [aplicación web](https://toutapp.com/login), haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one-1.png)

1. En Configuración de administración, seleccione **Cancela la suscripción**.

   ![](assets/two-2.png)

1. Clic **Sincronización con Salesforce**, luego habilite la sincronización nocturna.

   ![](assets/three-2.png)

1. Seleccione el campo con el que desea sincronizar.

   ![](assets/4.png)

   | Campo | Descripción |
   |---|---|
   | **Sincronizar con el campo No participar en Salesforce** | Seleccionado de forma predeterminada, solo actualiza el campo Exclusión de Salesforce. |
   | **Sincronizar con el campo No participar en Marketo Sales.** | Si desea cancelar la suscripción de ventas y marketing por separado, elija esta opción para actualizar las suscripciones adicionales [Campo de exclusión de ventas de Marketo.](#msoo) |

## Instalación del campo de exclusión en el diseño de página {#installing-the-opt-out-field-in-the-page-layout}

**No participar en el correo electrónico**

La exclusión de correo electrónico es un campo estándar en Salesforce que está disponible para su instalación desde Salesforce. Debe ser administrador de Salesforce para instalarlo.

1. Ir a [Salesforce.com](https://salesforce.com) e inicie sesión.

   ![](assets/five-1.png)

1. Haga clic en su nombre de usuario y seleccione **Configurar**.

   ![](assets/six-1.png)

1. En el cuadro de búsqueda rápida, busque Contacto o Posible cliente. En esta situación, se está instalando el campo en el diseño de página Contacto, pero es recomendable instalar para ambos registros de persona.

   ![](assets/seven-1.png)

1. Seleccionar **Diseños de página**.

   ![](assets/eight-1.png)

1. Seleccionar **Editar** situado junto al diseño de página al que desee añadir el campo.

   ![](assets/nine.png)

1. Seleccionar **Campos**.

   ![](assets/ten.png)

1. Arrastre y suelte Exclusión de correo electrónico en el diseño de página.

   ![](assets/11.png)

1. Clic **Guardar**.

   ![](assets/twelve.png)

## No participar de las Marketo Sales {#marketo-sales-opt-out}

El campo Exclusión de ventas de Marketo es un campo personalizado disponible para los usuarios que han instalado las personalizaciones de Marketo Sales Connect.

Una vez que haya instalado correctamente las personalizaciones de Marketo Sales Connect en Salesforce, verá el campo Exclusión de ventas de Marketo disponible para usted.
