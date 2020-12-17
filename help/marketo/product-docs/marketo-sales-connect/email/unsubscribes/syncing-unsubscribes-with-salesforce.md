---
unique-page-id: 14746188
description: Sincronización de cancelaciones de suscripción con Salesforce - Documentos de marketing - Documentación del producto
title: Sincronización de cancelaciones de suscripción con Salesforce
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Sincronización de cancelaciones de suscripción con Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelar la suscripción a la sincronización con Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronización de cancelación de suscripción debe estar activada (para sincronización nocturna)
* El campo exclusión debe estar instalado en Salesforce
* Los registros de personas de Sales Connect deben tener un ID de Salesforce

**Eliminaciones de suscripciones push**

Cuando se recopila una cancelación de suscripción en Sales Connect, se envía a Salesforce en tiempo real y se actualiza cualquiera de los campos Exclusión que ha seleccionado para sincronizar. Si deshabilitaste la sincronización de Salesforce, seguiremos impulsando la cancelación de suscripción al exclusión de correo electrónico.

**Cancelar suscripción de sincronización**

Cuando habilite la sincronización de cancelación de suscripción (paso 3 a continuación), activará la sincronización por la noche. La sincronización se produce una vez al día alrededor de las 20:00 PST. Sincronizará bidireccionalmente todas las cancelaciones de suscripción en MSE/ToutApp con el campo Exclusión de Salesforce.

## Configurar la anulación de suscripción de la sincronización con Salesforce {#configure-unsubscribe-sync-to-salesforce}

Los usuarios pueden decidir si desean sincronizar sus cancelaciones de suscripción con el campo Exclusión correo electrónico estándar con el que Marketing también puede sincronizar, o si pueden sincronizarse con el campo Exclusión ventas de marketing para que se puedan diferenciar las cancelaciones de ventas y las cancelaciones de suscripción de marketing.

1. Vaya a la [aplicación Web](http://toutapp.com/login), haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one-1.png)

1. En Configuración de administración, seleccione **Anula suscripciones**.

   ![](assets/two-2.png)

1. Haga clic en **Sincronización con Salesforce** y habilite la sincronización por la noche.

   ![](assets/three-2.png)

1. Seleccione el campo al que desee sincronizar.

   ![](assets/4.png)

   | **Sincronizar con el campo Exclusión de Salesforce** | Seleccionado de forma predeterminada, solo actualiza el campo Exclusión de Salesforce. |
   |---|---|
   | **Sincronizar con el campo Exclusión ventas de marketing** | Si desea separar las cancelaciones de ventas y de marketing, elija esta opción para actualizar el campo adicional [Exclusión ventas de marketing.](#msoo) |

## Instalación del campo Exclusión en el diseño de página {#installing-the-opt-out-field-in-the-page-layout}

**Exclusión correo electrónico**

Exclusión correo electrónico es un campo estándar de Salesforce que se puede instalar desde Salesforce. Debe ser administrador de Salesforce para instalarlo.

1. Vaya a [Salesforce.com](http://Salesforce.com) e inicie sesión.

   ![](assets/five-1.png)

1. Haga clic en el nombre de usuario y seleccione **Configuración**.

   ![](assets/six-1.png)

1. En el cuadro de búsqueda rápida, busque Contacto o Posible cliente. En este escenario, instalaremos el campo en el diseño de página Contacto, pero querrá instalarlo para ambos registros de persona.

   ![](assets/seven-1.png)

1. Seleccione **Diseños de página**.

   ![](assets/eight-1.png)

1. Seleccione **Editar** al lado del diseño de página al que desea agregar el campo.

   ![](assets/nine.png)

1. Seleccione **Campos**.

   ![](assets/ten.png)

1. Arrastre y suelte Exclusión correo electrónico en el diseño de página.

   ![](assets/11.png)

1. Haga clic en **Guardar**.

   ![](assets/twelve.png)

## Exclusión ventas de marketing {#marketo-sales-opt-out}

El campo Exclusión ventas de marketing es un campo personalizado que está disponible para los usuarios que han instalado las personalizaciones de conexión de marketing y ventas.

Una vez que haya instalado correctamente en Salesforce las personalizaciones de conexión de marketing para ventas, verá el campo Exclusión ventas de marketing disponible para usted.
