---
unique-page-id: 14746188
description: Sincronización de la cancelación de suscripciones con Salesforce - Marketo Docs - Documentación del producto
title: Sincronización de la cancelación de suscripciones con Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 1%

---

# Sincronización de la cancelación de suscripciones con Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelar la suscripción para sincronizar con Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronización de cancelación de suscripción debe estar habilitada (para sincronización por la noche)
* El campo de exclusión debe estar instalado en Salesforce
* Los registros de persona de Sales Connect deben tener un ID de Salesforce

**Cancelación de suscripciones push**

Cuando se recopila una cancelación de suscripción en Sales Connect, se envía a Salesforce en tiempo real y se actualiza cualquiera de los campos de exclusión que ha seleccionado para sincronizar. Si ha desactivado la sincronización de Salesforce, se continúa transfiriendo la cancelación de suscripción a la exclusión de correo electrónico.

**Cancelar suscripción**

Cuando habilite la sincronización de cancelación de suscripción (paso 3 a continuación), activará la sincronización por la noche. La sincronización se produce una vez al día, alrededor de las 20:00 PST. Sincronizará bidireccionalmente todas las cancelaciones de suscripción en MSE/ToutApp con el campo Exclusión de Salesforce.

## Configurar la cancelación de la suscripción a Salesforce {#configure-unsubscribe-sync-to-salesforce}

Los usuarios pueden decidir si desean sincronizar sus cancelaciones de suscripción con el campo de exclusión de correo electrónico estándar con el que Marketo también puede sincronizar, o si pueden sincronizarse con el campo de exclusión de ventas de Marketo para que se puedan diferenciar las cancelaciones de suscripción de ventas y las cancelaciones de suscripción de marketing.

1. Vaya a la [aplicación web](https://toutapp.com/login), haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/one-1.png)

1. En Configuración de administración , seleccione **Cancelación de suscripción**.

   ![](assets/two-2.png)

1. Haga clic en **Sincronización con Salesforce** y, a continuación, habilite la sincronización por la noche.

   ![](assets/three-2.png)

1. Seleccione el campo al que desee sincronizar.

   ![](assets/4.png)

   | Campo | Descripción |
   |---|---|
   | **Campo Sincronizar con exclusión de Salesforce** | Seleccionado de forma predeterminada, solo actualiza el campo Exclusión de Salesforce . |
   | **Campo Sincronizar con exclusión de ventas de Marketo** | Si desea separar las cancelaciones de suscripción de Ventas y Marketing, elija esta opción para actualizar las suscripciones adicionales [Campo Exclusión de ventas de Marketo .](#msoo) |

## Instalación del campo Exclusión en el diseño de página {#installing-the-opt-out-field-in-the-page-layout}

**No participar en el correo electrónico**

La exclusión de correo electrónico es un campo estándar de Salesforce que está disponible para instalar desde Salesforce. Debe ser administrador de Salesforce para instalarlo.

1. Vaya a [Salesforce.com](https://salesforce.com) e inicie sesión.

   ![](assets/five-1.png)

1. Haga clic en el nombre de usuario y seleccione **Configuración**.

   ![](assets/six-1.png)

1. En el cuadro de búsqueda rápida, busque Contacto o Posible cliente. En esta situación, se está instalando el campo en el diseño de página de contacto, pero se desea instalar para ambos registros de persona.

   ![](assets/seven-1.png)

1. Select **Diseños de página**.

   ![](assets/eight-1.png)

1. Select **Editar** junto al diseño de página al que desea añadir el campo .

   ![](assets/nine.png)

1. Select **Campos**.

   ![](assets/ten.png)

1. Arrastre y suelte la opción Desactivar correo electrónico en el diseño de página.

   ![](assets/11.png)

1. Haga clic en **Guardar**.

   ![](assets/twelve.png)

## Exclusión de ventas de Marketo {#marketo-sales-opt-out}

El campo Exclusión de ventas de Marketo es un campo personalizado que está disponible para los usuarios que han instalado las personalizaciones de conexión de ventas de Marketo.

Una vez que haya instalado correctamente las personalizaciones de Marketo Sales Connect en Salesforce, verá el campo Exclusión de ventas de Marketo disponible para usted.
