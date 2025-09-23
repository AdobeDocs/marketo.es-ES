---
unique-page-id: 2359646
description: Configuración del perfil progresivo de formularios - Documentos de Marketo - Documentación del producto
title: Configurar una creación de perfiles progresiva del formulario
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Configurar una creación de perfiles progresiva del formulario {#configure-form-progressive-profiling}

¡Las formas cortas son buenas! Cuando alguien vuelve a un formulario, puede presentar nuevos campos y rellenar progresivamente el perfil del visitante. Así es cómo se hace.

>[!NOTE]
>
>Para que esta función funcione correctamente, asegúrese de que Rellenar previamente formulario esté habilitado para los campos visibles y [deshabilitado](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para los campos ocultos.

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/ma-1.png)

1. Seleccione el formulario y haga clic en **[!UICONTROL Editar formulario]**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. En **[!UICONTROL Configuración de formulario]**, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Establezca **[!UICONTROL Perfil progresivo]** en **[!UICONTROL Habilitado]**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Bien, ahora vamos a configurarlo. Vaya a **[!UICONTROL Detalles del campo]**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arrastre y suelte todos los campos que forman parte del conjunto de perfiles progresivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Cuando termine de mover todos los campos, debería tener un aspecto similar al siguiente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Los campos que están fuera del cuadro **[!UICONTROL Perfiles progresivos]** siempre se mostrarán en el formulario, aunque estén rellenados.

1. Seleccione la casilla **[!UICONTROL Perfiles progresivos]**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenga cuidado al usar los campos obligatorios en [!UICONTROL Perfiles progresivos]. Estos campos podrían permanecer en blanco si el visitante introduce una nueva dirección de correo electrónico (que crearía una nueva persona) después de enviar anteriormente los datos de los demás campos, ya que se suprimirían en el formulario más reciente.

1. Ahora elija cuántos campos en blanco desea que vean los usuarios en el cuadro **Perfiles progresivos** en un momento dado.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Si elige **[!UICONTROL Cantidad de campos en blanco]** como 1, el visitante verá lo siguiente la primera vez que vea este formulario:
   >
   >* Nombre (vacío)
   >* Apellidos (vacío)
   >* Dirección de correo electrónico (vacía)
   >* Número de teléfono (vacío)
   >
   >Si rellenan todos los campos, la segunda vez que visiten, verán lo siguiente:
   >
   >* Nombre (rellenado previamente)
   >* Apellido (rellenado previamente)
   >* Dirección de correo electrónico (rellenada previamente)
   >* Número de teléfono móvil (vacío)
   >
   >Si rellenan el número de teléfono móvil, la tercera vez que lo visiten verán lo siguiente:
   >
   >* Nombre (rellenado previamente)
   >* Apellido (rellenado previamente)
   >* Dirección de correo electrónico (rellenada previamente)
   >* País (vacío)

1. Haga clic en **[!UICONTROL Finalizar]**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Haga clic en **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

¡Buen trabajo! El trabajo que acabas de hacer dará sus frutos.

Experimente con esta función y asegúrese de realizar pruebas. Es avanzado, pero puede hacer que sus formularios sean muy dinámicos de esta manera.
