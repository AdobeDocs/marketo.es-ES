---
unique-page-id: 2950682
description: Creación de un canal de programa - Documentos de Marketo - Documentación del producto
title: Crear un canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Crear un canal de programa {#create-a-program-channel}

Un programa es una iniciativa de marketing específica. El canal está diseñado para ser el mecanismo de entrega, como seminario web, patrocinio o anuncio en línea.

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!NOTE]
>
>Más información sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), el elemento más importante de Marketo.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/create-a-program-channel-1.png)

1. Clic **[!UICONTROL Etiquetas]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >¿Por qué etiquetas? Un canal es una forma de describir un programa, al igual que otras etiquetas. El canal solo tiene características adicionales especiales.

1. Haga clic en **+** firmar junto a [!UICONTROL Canal] para expandir y ver los canales existentes.

   ![](assets/create-a-program-channel-3.png)

1. En **[!UICONTROL Nuevo]**, haga clic en **[!UICONTROL Nuevo canal]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Canal: vallas publicitarias
   >
   >* Aplicar a: Predeterminado
   >* Progresión: Miembro, Comprometido (si tiene dudas, funcionan bien)
   >* Éxito: participación
   >
   >Canal: Party
   >
   >* Aplicar a: evento
   >* Progresión: Invitado, Registrado, Sin show y Asistido
   >* Éxito: asistencia
   >
   >Consulte las Progresiones de canales existentes para hacerse una idea de cómo utilizarlos.

1. Vamos con el ejemplo del canal Party. Asigne un nombre al nuevo **Canal** y seleccione el tipo de programa al que se aplicará.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >¿Aplicar a qué? Existen varios tipos de programas. Haga coincidir el canal con el tipo derecho. En caso de duda, elija **[!UICONTROL Predeterminado]**.

   >[!NOTE]
   >
   >Al usar &quot;[!UICONTROL Evento con seminario web],&quot; las asignaciones del sistema se bloquearán (según lo requieran las integraciones del seminario web) y no se podrán editar.

1. Introduzca los dos primeros nombres de estado del programa y haga clic en **[!UICONTROL Añadir etapa]**.

   ![](assets/create-a-program-channel-6.png)

1. Introduzca otro programa **[!UICONTROL Estado]** y **[!UICONTROL Etapa]** número y haga clic en **[!UICONTROL Añadir etapa]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >El **[!UICONTROL Etapa]** El número se utiliza para ordenar los estados del programa. Tenga en cuenta que las personas no pueden retroceder en estos pasos de progresión. Solo pueden cambiar el estado a un estado de valor mayor o igual. Utilice los valores iguales cuando los estados estén pensados para cambiar de un lado a otro en lugar de una progresión.

1. Introduzca el último programa **[!UICONTROL Estado]** y **[!UICONTROL Etapa]** número.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Al usar el tipo &quot;[!UICONTROL Evento],&quot; se requiere la asignación del sistema para los estados Registrado, En lista de espera y Asistido. Como tal, esos estados no se pueden ocultar.

1. Elija el **[!UICONTROL Estado de facturación móvil]** para **[!UICONTROL Registrados]**.

   ![](assets/create-a-program-channel-9.png)

1. Elija el **[!UICONTROL Estado de facturación móvil]** para **[!UICONTROL Asistió]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Estado de facturación móvil]** Las opciones de solo estarán disponibles si el canal es para programas de eventos.

   >[!NOTE]
   >
   >Solo las personas con **[!UICONTROL Estado de facturación móvil]** de **[!UICONTROL Registrados]** y **[!UICONTROL Asistió]** será visible en el [Aplicaciones de registro móviles](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Si se crea una nueva persona en la aplicación de registro móvil, se establece en Registrada en el programa de evento. Si una persona se registra en el evento de la aplicación, se establecerá en Asistió en el programa de evento.

1. Seleccione el **[!UICONTROL Correcto]** estado del programa y haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-a-program-channel-11.png)

   ¡Bien hecho! Cuando realice un nuevo programa de ese tipo, este nuevo canal será una de las opciones.
