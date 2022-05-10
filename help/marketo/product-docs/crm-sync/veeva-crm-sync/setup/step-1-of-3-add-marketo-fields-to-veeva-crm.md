---
description: 'Paso 1 de 3: Añadir campos de Marketo a Veva CRM - Marketo Docs - Documentación del producto'
title: 'Paso 1 de 3: Añadir campos de Marketo a Veva CRM'
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 4%

---

# Paso 1 de 3: Añadir campos de Marketo a Veva CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>La instancia de Veva CRM debe tener acceso a las API de Salesforce para sincronizar datos entre Marketo Engage y Veva CRM.

El Marketo Engage utiliza un conjunto de campos para capturar ciertos tipos de información relacionada con el marketing. Si desea estos datos en Veva CRM, siga las instrucciones que se indican a continuación.

`1.` Cree un campo personalizado en Veva CRM en los objetos de contacto: Puntuación

`2.` Si lo desea, puede crear campos adicionales (consulte la tabla siguiente).

Todos estos campos personalizados son opcionales y no son necesarios para sincronizar Marketo Engage y Veva CRM.

## Añadir campos de Marketo a Veva CRM {#add-marketo-fields-to-veeva-crm}

Agregue un campo personalizado en el posible cliente y los objetos de contacto en Veva CRM enumerados arriba. Si desea agregar más, consulte la tabla de campos disponibles al final de esta sección.

Realice los siguientes pasos para que el campo Score lo añada.

1. Inicie sesión en Veeva CRM y haga clic en **Configuración**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Haga clic en Objetos y campos y seleccione Administrador de objetos.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. En la barra de búsqueda, busque Contacto.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Haga clic en el objeto Contact .

1. Seleccione Campos y relaciones.

1. Haga clic en **Nuevo**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Elija el tipo de campo apropiado (para Puntuación — número).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Haga clic en **Siguiente**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Introduzca la Etiqueta de campo, Longitud y Nombre de campo para el campo, como se muestra en la tabla siguiente.

<table>
 <tbody>
  <tr>
   <th>Etiqueta de campo
   <th>Nombre del campo
   <th>Tipo de datos
   <th>Atributos de campo
  </tr>
  <tr>
   <td>Puntuación</td>
   <td>mkto71_Lead_Score</td>
   <td>Número</td>
   <td>Longitud 10<br/>
Lugares decimales 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Veeva CRM anexa __c a Nombres de campo cuando los utiliza para crear nombres de API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Los campos de texto y número requieren una longitud, pero los campos de fecha y hora no la necesitan. Una descripción es opcional.

1. Haga clic en **Siguiente**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Especifique la configuración de acceso y haga clic en **Siguiente**.

1. Establezca todas las funciones como Visible y de Solo lectura.

1. Desactive la casilla de verificación de solo lectura para el perfil del usuario de sincronización:

* Si tiene un usuario con el perfil de un administrador del sistema como usuario de sincronización, desactive la casilla de verificación Solo lectura del perfil del administrador del sistema (como se muestra a continuación).
* Si ha creado un perfil personalizado para el usuario de sincronización, desactive la casilla de verificación de solo lectura para ese perfil personalizado.

   ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Elija los diseños de página que deben mostrar el campo.

1. Haga clic en **Guardar y nuevo** para volver atrás y crear cada uno de los otros dos campos personalizados.

1. Haga clic en **Guardar** cuando haya terminado con los tres.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Al agregar el campo al objeto Contact , también se agregan al objeto Person Account .

OPCIONAL: Utilice el procedimiento anterior para cualquier campo personalizado adicional de la siguiente tabla.

<table>
 <tbody>
  <tr>
   <th>Etiqueta de campo
   <th>Nombre del campo
   <th>Tipo de datos
   <th>Atributos de campo
  </tr>
  <tr>
   <td>Ciudad inferida</td>
   <td>mkto71_Inferred_City</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>Compañía inferida</td>
   <td>mkto71_Inferred_Company</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>País inferido</td>
   <td>mkto71_Inferred_Country</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>Área metropolitana inferida</td>
   <td>mkto71_Inferred_Metropolitan_Area</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>Código de área telefónico inferido</td>
   <td>mkto71_Inferred_Phone_Area_Code</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>Código postal inferido</td>
   <td>mkto71_Inferred_Postal_Code</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
  <tr>
   <td>Región del estado inferida</td>
   <td>mkto71_Inferred_State_Region</td>
   <td>Texto</td>
   <td>Longitud 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Los valores de los campos asignados automáticamente por Marketo no estarán disponibles inmediatamente en Veva CRM cuando se haya creado el nuevo campo. Marketo sincronizará los datos con Veva CRM en la próxima actualización del registro en cualquiera de los sistemas (es decir, una actualización de cualquiera de los campos sincronizados entre Marketo y Veva CRM).
