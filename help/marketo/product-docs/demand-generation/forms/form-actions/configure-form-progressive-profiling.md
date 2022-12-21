---
unique-page-id: 2359646
description: 'Configuración de perfiles progresivos de formulario: documentos de Marketo: documentación del producto'
title: Configurar la creación progresiva de formularios
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Configurar la creación progresiva de formularios {#configure-form-progressive-profiling}

Las formas cortas son buenas. Cuando alguien vuelve a un formulario, puede presentar nuevos campos y rellenar progresivamente el perfil del visitante. Así es como.

>[!NOTE]
>
>Para que esta función funcione correctamente, asegúrese de que el relleno previo del formulario esté habilitado para los campos visibles y [disabled](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para campos ocultos.

1. Vaya a **Actividades de marketing**.

   ![](assets/ma-1.png)

1. Seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. En **Configuración de formulario**, haga clic en **Configuración**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Establezca **Perfiles progresivos** a **Habilitado**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Bien, ahora vamos a configurarlo. Vaya a **Detalles del campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arrastre y suelte todos los campos que formen parte del conjunto de perfiles progresivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Cuando termine de mover todos los campos, debería tener un aspecto similar al siguiente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Los campos fuera de la variable **Perfiles progresivos** siempre se mostrará en el formulario, aunque estén rellenados.

1. Seleccione el **Perfiles progresivos** en la ventana

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenga cuidado al usar los campos obligatorios en Perfiles progresivos. Estos campos podrían seguir en blanco si el visitante introduce una nueva dirección de correo electrónico (que creará una persona nueva) después de enviar previamente datos para los demás campos, ya que se suprimirán en el formulario más reciente.

1. Ahora elija cuántos campos en blanco desea que vean las personas de la variable **Perfiles progresivos** en cualquier momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Si elige **Número** **de** **En blanco** **Campos** como 1, el visitante verá lo siguiente la primera vez que vea este formulario:
   >
   >* Nombre (vacío)
   >* Apellidos (vacío)
   >* Dirección de correo electrónico (vacía)
   >* Número de teléfono (vacío)

   >
   >Suponiendo que rellenen todos los campos, la segunda vez que visiten verá:
   >
   >* Nombre (prerellenado)
   >* Apellidos (rellenado previamente)
   >* Dirección de correo electrónico (precargada)
   >* Número de teléfono móvil (vacío)

   >
   >Suponiendo que rellenen el número de teléfono móvil, la tercera vez que visiten verán:
   >
   >* Nombre (prerellenado)
   >* Apellidos (rellenado previamente)
   >* Dirección de correo electrónico (precargada)
   >* País (vacío)


1. Haga clic en **Finalizar**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Haga clic en **Aprobar y cerrar**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

¡Buen trabajo! El trabajo que acabas de hacer saldrá adelante.

Experimente con esta función y asegúrese de probarla. Es avanzado, pero puede hacer que los formularios sean muy dinámicos de esta manera.
