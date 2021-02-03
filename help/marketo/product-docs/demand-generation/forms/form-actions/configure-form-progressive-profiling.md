---
unique-page-id: 2359646
description: Configurar la creación progresiva de perfiles de formulario - Documentos de marketing - Documentación del producto
title: Configurar la creación progresiva de perfiles de formulario
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Configurar la generación progresiva de perfiles de formulario {#configure-form-progressive-profiling}

¡Los formularios cortos son buenos! Cuando alguien regresa a un formulario, puede presentar nuevos campos y rellenar progresivamente el perfil del visitante. Así es como.

>[!NOTE]
>
>Para que esta función funcione correctamente, asegúrese de que Prerellenar el formulario está habilitado para los campos visibles y [deshabilitado](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para los campos ocultos.

1. Vaya a **Actividades de marketing**.

   ![](assets/ma-1.png)

1. Seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. En **Configuración del formulario**, haga clic en **Configuración**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Establezca **Perfiles progresivos** en **Habilitado**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Bien, ahora configúrelo. Vaya a **Detalles del campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arrastre y suelte todos los campos que forman parte del conjunto de perfiles progresivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Cuando termine de mover todos los campos, debería tener este aspecto:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Los campos fuera del cuadro **Perfiles progresivos** siempre se mostrarán en el formulario, incluso si se han rellenado.

1. Seleccione el cuadro **Perfiles progresivos**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenga cuidado al usar los campos obligatorios en Perfiles progresivos. Estos campos podrían quedar en blanco si el visitante introduce una nueva dirección de correo electrónico (que crearía una nueva persona) después de haber enviado previamente datos para los demás campos, ya que se suprimirían en el formulario más reciente.

1. Ahora elija cuántos campos en blanco desea que vean las personas en el cuadro **Perfiles progresivos** en un momento dado.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Si elige **Número** **de** **Campo en blanco** **Campos** como 1, el visitante verá lo siguiente la primera vez que vea este formulario:
   >
   >* Nombre (vacío)
   >* Apellido (vacío)
   >* Dirección de correo electrónico (vacía)
   >* Número de teléfono (vacío)

   >
   >Suponiendo que rellenen todos los campos, la segunda vez que los visiten, verán:
   >
   >* Nombre (prerelleno)
   >* Apellidos (prerellenado)
   >* Dirección de correo electrónico (rellenado previamente)
   >* Número de teléfono móvil (vacío)

   >
   >Suponiendo que rellenen el número de teléfono móvil, la tercera vez que visiten verá:
   >
   >* Nombre (prerelleno)
   >* Apellidos (prerellenado)
   >* Dirección de correo electrónico (rellenado previamente)
   >* País (vacío)


1. Haga clic en **Finalizar**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Haga clic en **Aprobar y cerrar**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

¡Buen trabajo! El trabajo que acabas de hacer dará sus frutos.

Experimente con esta función y asegúrese de probarla. Está avanzado, pero puede hacer que los formularios sean muy dinámicos de esta manera.
