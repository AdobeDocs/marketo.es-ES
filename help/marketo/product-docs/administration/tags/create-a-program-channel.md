---
unique-page-id: 2950682
description: Creación de un canal de programa - Documentos de Marketo - Documentación del producto
title: Creación de un canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---

# Creación de un canal de programa {#create-a-program-channel}

Un programa es una iniciativa de marketing específica. El canal está diseñado para ser el mecanismo de entrega, como seminario web, patrocinio o anuncio en línea.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>Más información sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), el elemento más importante de Marketo.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-program-channel-1.png)

1. Haga clic en **[!UICONTROL Etiquetas]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >¿Por qué etiquetas? Un canal es una forma de describir un programa, al igual que otras etiquetas. El canal solo tiene características adicionales especiales.

1. Haga clic en el signo **+** que está junto al [!UICONTROL Canal] para expandir y ver los canales existentes.

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

1. Vamos con el ejemplo del canal Party. Asigne un nombre a su nuevo **[!UICONTROL canal]** y seleccione el tipo de programa al que se aplicará.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >¿Aplicar a qué? Existen varios tipos de programas. Haga coincidir el canal con el tipo derecho. Si tiene dudas, elija **[!UICONTROL Predeterminado]**.

   >[!NOTE]
   >
   >Al usar &quot;[!UICONTROL Evento con seminario web]&quot;, las asignaciones del sistema se bloquearán (según lo requieran las integraciones del seminario web) y no se podrán editar.

1. Escriba los dos primeros nombres de estado del programa y haga clic en **[!UICONTROL Agregar paso]**.

   ![](assets/create-a-program-channel-6.png)

1. Escriba otro número de programa **[!UICONTROL Status]** y **[!UICONTROL Step]**, y luego haga clic en **[!UICONTROL Agregar paso]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >El número **[!UICONTROL Step]** se usa para ordenar los estados del programa. Tenga en cuenta que las personas no pueden retroceder en estos pasos de progresión. Solo pueden cambiar el estado a un estado de valor mayor o igual. Utilice los valores iguales cuando los estados estén pensados para cambiar de un lado a otro en lugar de una progresión.

1. Introduzca el último número de programa **[!UICONTROL Status]** y **[!UICONTROL Step]**.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Al usar el tipo &quot;[!UICONTROL Event]&quot;, se requiere la asignación del sistema para los estados Registrado, En lista de espera y Asistido. Como tal, esos estados no se pueden ocultar.

1. Elija el **[!UICONTROL estado de registro móvil]** para **[!UICONTROL Registrado]**.

   ![](assets/create-a-program-channel-9.png)

1. Elija el **[!UICONTROL estado de registro móvil]** para **[!UICONTROL Asistió]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >Las opciones de **[!UICONTROL Estado de protección móvil]** solo estarán disponibles si el canal se utilizará para programas de eventos.

   >[!NOTE]
   >
   >Solo las personas con **[!UICONTROL estado de registro móvil]** de **[!UICONTROL Registradas]** y **[!UICONTROL Asistidas]** serán visibles en las [Aplicaciones de registro móvil](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Si se crea una nueva persona en la aplicación de registro móvil, se establecerá en [!UICONTROL Registrada] en el programa de eventos. Si una persona está registrada en el evento de la aplicación, se establecerá en [!UICONTROL Asistió] en el programa de eventos.

1. Seleccione el estado del programa **[!UICONTROL Success]** y luego haga clic en **[!UICONTROL Create]**.

   ![](assets/create-a-program-channel-11.png)

   ¡Bien hecho! Cuando realice un nuevo programa de ese tipo, este nuevo canal será una de las opciones.
