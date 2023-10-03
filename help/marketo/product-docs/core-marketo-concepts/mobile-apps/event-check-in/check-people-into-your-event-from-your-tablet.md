---
unique-page-id: 2949839
description: 'Registrar a las personas en su evento desde su tableta: documentos de Marketo, documentación del producto'
title: Incorporar personas a su evento desde su tableta
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 61b5500c6acbe6448a70e28f4b0cafe3c005a02a
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Incorporar personas a su evento desde su tableta {#check-people-into-your-event-from-your-tablet}

Cuando las personas se presenten en su evento, puede encontrar su información en la aplicación. Después de registrarse, se promocionan al estado Asistido cuando se sincroniza con Marketo.

>[!IMPORTANT]
>
>El 2 de octubre de 2023, Adobe eliminó la aplicación Eventos de Marketo de todas las tiendas de aplicaciones. Si ya tiene la aplicación instalada en su tableta o dispositivo móvil, puede seguir utilizándola por el momento. Una vez que la instancia de Marketo Engage se haya migrado a Identidad de Adobe para la autenticación de Marketo, ya no podrá acceder a la aplicación. [Más información](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}.

La aplicación funciona igual tanto en iPad como en Android, excepto por pequeñas diferencias de diseño.

>[!PREREQUISITES]
>
>* Cree un evento en Marketo y rellénelo con personas invitadas y registradas.

## Registrar invitados registrados {#check-in-registered-guests}

1. Toque el icono de la aplicación en su tableta iPad o Android.

1. Tocar **Iniciar sesión** para iniciar la aplicación Marketo Event.

   ![](assets/1.jpg)

1. Introduzca su nombre de usuario y contraseña de Marketo y haga clic en **Iniciar sesión**.

   >[!NOTE]
   >
   >Debe tener una función con acceso a la base de datos para ver a las personas en la aplicación.

1. Seleccione un **Evento**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Solo se muestran los programas de eventos (con la excepción de los seminarios web) programados una semana antes y una semana después de la fecha de hoy.

1. En la pantalla Inicio, busque Registrados invitados. Para encontrar una persona en la lista, puede:

   * Desplazarse para buscar un nombre
   * Introduzca un nombre en el campo de búsqueda
   * Para ir a una letra inicial específica del apellido, púlsela en el lado derecho de la lista

   >[!NOTE]
   >
   >El proceso es el mismo en iPad y Android, pero las pantallas difieren y los elementos pueden estar en ubicaciones diferentes. Este artículo incluye la interfaz de iPad. Compare la pantalla de Android en esta sección como referencia.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Pulse el nombre seleccionado y, en el registro de persona, pulse **Check-in**.

   ![](assets/img-0068-35-hands.png)

El invitado ahora tiene el estado Asistido y recibe una marca de verificación. El registro de persona se actualiza cuando se sincroniza con Marketo. El contador rojo del botón Sincronizar aumenta para mostrar el número de registros desde la última sincronización con Marketo. El botón Sincronizar tiene un aspecto diferente y se encuentra en una ubicación diferente para iPad y Android:

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Si una persona está invitada pero no se ha registrado, puede buscar el nombre haciendo clic en **Buscar en el servidor**, justo debajo del cuadro de búsqueda. El estado Invitado cambia a **Asistió** para el evento.

## Crear una nueva persona en la tableta {#create-a-new-person-on-the-tablet}

Puede agregar manualmente invitados que no sean personas existentes en la base de datos de Marketo. Se registrarán automáticamente y se agregarán a la base de datos al sincronizar con Marketo.

1. Clic **Añadir**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Complete tantos campos de información básica como pueda y pulse **Listo**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Solo puede utilizar los campos existentes. No se pueden crear los personalizados.

   >[!CAUTION]
   >
   >Compruebe la dirección de correo electrónico. Otros campos se pueden corregir más adelante, pero la dirección de correo electrónico es el método principal para ponerse en contacto con el invitado.

La nueva persona se registrará como registrada en el evento y se agregará a la base de datos de Marketo con el estado Asistido cuando se sincronice con Marketo.

## Invertir un registro de entrada {#reverse-a-check-in}

Si registraste a una persona por error, _antes de sincronizar con Marketo_, puede invertir el estado Asistencia.

1. Pulse el nombre en la lista y, en el registro de persona, pulse **Deshacer**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   ¡Todo arreglado!

## Editar un registro de persona al registrarse {#edit-a-person-record-at-check-in}

Puede añadir y modificar la información de los invitados, justo en el evento.

1. Pulse el nombre en la lista Personas y pulse **Editar**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Edite y agregue información a los campos y, a continuación, pulse **Listo**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >En Android, la variable **Listo** El botón puede estar oculto. Desplácese hacia abajo para encontrarlo.

La información se actualizará cuando sincronice la aplicación con Marketo.

## Sincronizar la aplicación con Marketo {#sync-the-app-with-marketo}

La aplicación Eventos de Marketo funciona de forma independiente hasta que sincronice la actividad con la base de datos de Marketo. Es mejor sincronizar lo antes posible después de la última llegada. Su tableta debe estar conectada a Internet.

>[!CAUTION]
>
>Después de la sincronización, no se puede revertir un registro desde la aplicación.

1. En la tableta, abra la aplicación y vaya al evento.

1. Tocar **Sincronización**.

   El evento se actualiza con nuevos registros en la base de datos de Marketo. El contador rojo del botón Sincronizar se borra hasta que se registra a otra persona.

   Por motivos de seguridad, debe salir de la aplicación Eventos de Marketo después de terminar de sincronizar.

## Uso de acceso limitado a Internet {#working-with-limited-internet-access}

Algunos lugares tienen un acceso a Internet escaso. Necesita una buena conexión para:

* Descargue e instale la aplicación
* Iniciar sesión
* Seleccione un evento
* Sincronizar la aplicación con Marketo

Si te preocupa el acceso a Internet en el lugar de celebración, es posible que quieras iniciar sesión en la aplicación Marketo Events y seleccionar tu evento con antelación, en un lugar con un fuerte acceso a Internet. De este modo, podrá seguir utilizando la aplicación sin conexión. A continuación, cuando recupere una conexión a Internet, sincronícese inmediatamente con la base de datos de Marketo.

>[!TIP]
>
>Si no tiene conexión a Internet, puede crear una nueva persona para una persona que esté registrándose. Se reconciliará con la persona existente cuando sincronices la aplicación.

>[!NOTE]
>
>La aplicación cierra sesión automáticamente tras ocho horas de inactividad.
