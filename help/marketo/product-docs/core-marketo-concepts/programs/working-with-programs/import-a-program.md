---
unique-page-id: 1147108
description: 'Importación de un programa: documentos de Marketo, documentación del producto'
title: Importar un programa
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Importar un programa {#import-a-program}

Un programa se puede importar de una suscripción de Marketo Engage a otra. Por ejemplo, puede crear un programa en una zona protegida y luego importarlo en su suscripción activa. Además, puede importar un programa generado previamente desde el [Biblioteca del programa Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>Los programas que tengan listas inteligentes que contengan el déclencheur &quot;El objeto personalizado se ha actualizado&quot; provocarán un error en la importación. Elimine este déclencheur de todas las listas inteligentes antes de seguir los pasos descritos a continuación.

## Importación de programas {#importing-a-program}

1. Ir a **[!UICONTROL Actividades de marketing]**.

   ![](assets/import-a-program-1.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione. **[!UICONTROL Importar programa]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* La importación de programas solo está disponible para los usuarios que tienen roles con el permiso Importar programa habilitado. Más información sobre [administrar roles y permisos de usuario](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Para conectar una cuenta de zona protegida a su suscripción activa, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Seleccione una Marketo **[!UICONTROL Suscripción]** y un programa para importar. Clic **[!UICONTROL Siguiente]**.

   ![](assets/import-a-program-3.png)

1. Especifique un **[!UICONTROL Carpeta de campaña]** para el programa importado. Clic **[!UICONTROL Siguiente]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Asegúrese de **[!UICONTROL Utilizar conflicto predeterminado]** reglas está seleccionado. Se necesitan reglas de conflicto al importar programas en una instancia que tiene recursos del mismo nombre.

1. Seleccione los detalles del conflicto que desee y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Al importar un programa que utiliza pasos de flujo personalizados o reglas de listas inteligentes derivadas de un servicio de pasos de flujo a una instancia de destino en la que haya más de un proveedor de servicios compatible, se solicitará al usuario importador que asigne pasos o reglas al proveedor de servicios correcto en la instancia de destino.

1. Previsualizar detalles y **[!UICONTROL Importar]** el programa.

   ![](assets/import-a-program-6.png)

Recibirá una confirmación por correo electrónico una vez que la importación haya finalizado.

>[!NOTE]
>
>Debe volver a programar las campañas por lotes importadas y activar las campañas de déclencheur. El sistema desactiva automáticamente las programaciones de campaña y las campañas de déclencheur en el programa importado.

## Impacto en los activos externos durante las importaciones del programa {#impact-on-external-assets-during-program-imports}

Los programas utilizan recursos externos como plantillas de correo electrónico, plantillas de página de aterrizaje, imágenes, formularios, tokens y etiquetas de programas. Tiene la capacidad de configurar cómo se gestionan las plantillas de página de aterrizaje y las etiquetas de programa, y Marketo administra automáticamente el resto.

**Plantillas de correo electrónico/página de aterrizaje:** Las plantillas de correo electrónico/página de aterrizaje se importan en Design Studio. Puede utilizar reglas de conflicto para configurar el comportamiento cuando existe una plantilla con el mismo nombre. Con la regla predeterminada, se anexará un número a una plantilla si existe una con el mismo nombre. Por ejemplo, si ya tiene una plantilla denominada &quot;Plantilla estándar&quot;, la nueva se llamará &quot;Plantilla estándar - 1&quot;.

**Páginas de destino/Forms:** Si existe un formulario o una página de aterrizaje con el mismo nombre en Design Studio, se importarán, pero con un número anexado a su nombre (por ejemplo: Página de aterrizaje - 1).

**Imágenes:** Las imágenes utilizadas por las páginas de destino se importan en el estudio de diseño a menos que exista una con el mismo nombre.

**Tokens:** Los tokens que residen fuera de un programa se convertirán en tokens locales durante el proceso de importación.

>[!CAUTION]
>
>Tipo de imagen: mis tokens no son compatibles con las importaciones de programas. Si se importa un programa que tiene el tipo de imagen mis tokens, _no_ los tokens se transferirán.

**Etiquetas de programas:** Puede utilizar reglas de conflicto para controlar cómo se tratarán las etiquetas de programa que no existen en la cuenta de destino. El uso de la regla predeterminada creará las etiquetas de programa o puede optar por ignorar las etiquetas.

>[!CAUTION]
>
>Al importar un programa, correos electrónicos/páginas de aterrizaje que contengan lo siguiente [contenido dinámico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} se omitirá.
