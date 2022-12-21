---
unique-page-id: 2950682
description: 'Creación de un canal de programa: Marketo Docs: documentación del producto'
title: Creación de un canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Creación de un canal de programa {#create-a-program-channel}

Un programa es una iniciativa de marketing específica. El canal está diseñado para ser el mecanismo de entrega, como seminario web o patrocinio o publicidad en línea.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>Más información sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), el elemento más importante de Marketo.

1. En el **Administrador** , haga clic en **Etiquetas**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >¿Por qué las etiquetas? Un canal es una forma de describir un programa, al igual que otras etiquetas. El canal solo tiene características adicionales especiales.

1. Haga clic en el **+** iniciar sesión junto a **Canal** para expandir y ver los canales existentes.

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. En **Nuevo**, haga clic en **Nuevo canal**.

   ![](assets/image2014-9-24-12-3a58-3a53.png)

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Canal: Valla
   >
   >* Aplicar a: Predeterminado
   >* Progresión: Miembro, comprometido (si hay dudas, funcionan bien)
   >* Correcto: Comprometido

   >
   >Canal: Parte
   >
   >* Aplicar a: Evento
   >* Progresión: Invitado, registrado, sin programa y asistido
   >* Correcto: Asistida

   >
   >Consulte Progressions of existing channels para obtener una idea de cómo utilizarlos.

1. Vamos con el ejemplo de canal de Party. Asigne un nombre a la nueva **Canal** y seleccione el tipo de programa al que se aplicará.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >¿Aplicar a qué? Existen varios tipos de programas. Haga coincidir el canal con el tipo correcto. Si tiene dudas, elija **Predeterminado**.

   >[!NOTE]
   >
   >Al usar &quot;Evento con seminario web&quot;, las asignaciones del sistema se bloquearán (como lo requieren las integraciones de seminarios web) y no se podrán editar.

   Introduzca los dos primeros nombres de estado del programa y, a continuación, haga clic en Agregar paso.
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Introducir otro programa **Estado** y **Paso** número y, a continuación, haga clic en **Agregar paso**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >La variable **Paso** se utiliza para ordenar los estados del programa. Tenga en cuenta que la gente no puede retroceder en estos pasos de progresión. Solo pueden cambiar el estado a un estado de valor mayor o igual. Utilice los valores iguales cuando los estados pretendan cambiar de un estado a otro en lugar de una progresión.

1. Introducir el último programa **Estado** y **Paso** número.

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >Al utilizar el tipo &quot;Evento&quot;, se requiere la asignación del sistema para los estados Registrados, En lista de espera y Asistidos. Como tal, esos estados no pueden ocultarse.

1. Elija el **Estado de registro móvil** para **Registrados**.

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Elija el **Estado de registro móvil** para **Asistida**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**Estado de registro móvil**** **las opciones solo estarán disponibles si el canal está disponible para los programas de eventos.

   >[!NOTE]
   >
   >Solo las personas con un **Estado de registro móvil** de **Registrados** y **Asistida** será visible en la variable [Aplicaciones de registro móvil](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Si se crea una nueva persona en la aplicación de registro móvil, se establecerá en Registrada en el programa de evento. Si una persona está protegida en el evento de la aplicación, se establecerá en Asistido en el programa de eventos.

1. Seleccione el **Correcto** estado del programa y, a continuación, haga clic en **Crear**.

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   ¡Bien hecho! Cuando realice un nuevo programa de ese tipo, este nuevo canal será una de las opciones.
