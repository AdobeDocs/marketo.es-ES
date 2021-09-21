---
unique-page-id: 11372975
description: 'Paso 1 de 3: Añadir campos de Marketo a Salesforce (Professional) - Marketo Docs: Documentación del producto'
title: 'Paso 1 de 3: Añadir campos de Marketo a Salesforce (Professional)'
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
source-git-commit: 7de9b708626172aa6fa0a2fcb87c8aa534d5e9f7
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 5%

---

# Paso 1 de 3: Agregar campos de Marketo a Salesforce (Professional) {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>La instancia de Salesforce debe tener acceso a las API de Salesforce para sincronizar datos entre Marketo y Salesforce.

Marketo utiliza un conjunto de campos para capturar ciertos tipos de información relacionada con el marketing. Si desea estos datos en Salesforce, siga las instrucciones que se indican a continuación.

1. Cree tres campos personalizados en Salesforce en los objetos de contacto y posible cliente: Puntuación, programa de adquisición y fecha de adquisición.
1. Asigne estos campos personalizados entre posibles clientes y contactos para que, al realizar la conversión en Salesforce, los valores se mantengan.
1. Si es necesario, puede crear otros campos adicionales (consulte la tabla siguiente).

Todos estos campos personalizados son opcionales y no son necesarios para sincronizar Marketo y Salesforce. Como práctica recomendada, se recomienda crear campos para Puntuación, Programa de adquisición y Fecha de adquisición.

## Agregar campos de Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Agregue tres campos personalizados en el posible cliente y los objetos de contacto de Salesforce enumerados arriba. Si desea agregar más, consulte la tabla de campos disponibles al final de esta sección.

Realice los siguientes pasos para cada uno de los tres campos personalizados para agregarlos. Comience con **Score**.

1. Inicie sesión en Salesforce y haga clic en **Configuración.**

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. En el menú Generar de la izquierda, haga clic en **Personalizar** y seleccione **Posibles clientes**. Haga clic en **Fields**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Haga clic en **Nuevo** en la sección Campos y relaciones personalizados en la parte inferior de la página.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Elija el tipo de campo apropiado (para Puntuación — **número**; Programa de adquisición — **text**; Fecha de adquisición — **Fecha/Hora**).

   ![](assets/choose-field-type-2-hand.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Introduzca la Etiqueta de campo, Longitud y Nombre de campo para el campo, como se muestra en la tabla siguiente.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Etiqueta de campo 
    </div></th> 
   <th> 
    <div>
      Nombre del campo 
    </div></th> 
   <th> 
    <div>
      Tipo de datos 
    </div></th> 
   <th> 
    <div>
      Atributos de campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Puntuación</td> 
   <td>mkto71_Lead_Score</td> 
   <td>Número</td> 
   <td>Longitud 10<br>Cifras decimales 0 </td> 
  </tr> 
  <tr> 
   <td>Fecha de adquisición</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>Fecha/hora</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programa de adquisición</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce anexa __c a Field Names cuando los utiliza para crear API Names.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>Los campos de texto y número requieren una longitud, pero los campos de fecha y hora no la necesitan. Una descripción es opcional.

1. Haga clic en **Siguiente**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Especifique la configuración de acceso y haga clic en **Siguiente**:

   * Establezca todas las funciones como **Visible** y **Solo lectura**

   * Desactive la casilla **Read-Only** para el perfil del usuario de sincronización:

      * Si tiene un usuario con el perfil de _System Administrator_ como usuario de sincronización, desactive la casilla **Read-Only** del perfil del administrador del sistema (como se muestra a continuación)

      * Si ha creado un _perfil personalizado_ para el usuario de sincronización, desactive la casilla **Solo lectura** para ese perfil personalizado

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Elija los diseños de página que deben mostrar el campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Haga clic en **Guardar y nuevo** para volver y crear cada uno de los otros dos campos personalizados. Haga clic en **Guardar** con los tres.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. En el menú Generar de la izquierda, haga clic en **Personalizar** y seleccione **Contactos**. Haga clic en **Fields**.
1. Siga los pasos del 3 al 10 para los campos Puntuación, Fecha de adquisición y Programa de adquisición en el objeto de contacto, tal como hizo para el objeto de posible cliente.
1. Opcionalmente, utilice el procedimiento anterior para cualquier campo personalizado adicional de esta tabla.

<table> 
 <tbody> 
  <tr> 
   <th>Etiqueta de campo</th> 
   <th>Nombre del campo</th> 
   <th>Tipo de datos</th> 
   <th>Atributos de campo</th> 
  </tr> 
  <tr> 
   <td>Id Del Programa De Adquisición</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Número</td> 
   <td>Longitud 18<br>Cifras decimales 0 </td> 
  </tr> 
  <tr> 
   <td>Remitente original</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
  </tr> 
  <tr> 
   <td>Motor de búsqueda original</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
  </tr> 
  <tr> 
   <td>Frase de búsqueda original</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
  </tr> 
  <tr> 
   <td>Información de origen original</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
  </tr> 
  <tr> 
   <td>Tipo de origen original</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Texto</td> 
   <td>Longitud 255</td> 
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
>Los valores de los campos asignados automáticamente por Marketo no estarán disponibles inmediatamente en Salesforce cuando se haya creado el nuevo campo. Marketo sincronizará los datos con Salesforce la próxima actualización del registro en cualquier sistema (es decir, una actualización de cualquiera de los campos sincronizados entre Marketo y Salesforce).

## Asignar campos personalizados para conversiones  {#map-custom-fields-for-conversions}

Un campo personalizado del objeto de posible cliente de Salesforce debe asignarse a un campo de contacto del objeto de contacto para que los datos se transfieran cuando se produce una conversión.

1. En la esquina superior derecha, haga clic en Configuración.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Escriba &quot;campos&quot; en la búsqueda de navegación sin pulsar Intro. Los campos aparecen bajo diferentes objetos; Haga clic en Campos en Posibles clientes.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Vaya a la sección Campos y relaciones personalizados de posibles clientes y haga clic en Asignar campos de posibles clientes .

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Haga clic en la lista desplegable situada junto al campo que desee asignar.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Seleccione el campo personalizado de contacto correspondiente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Repita los pasos anteriores para cualquier otro campo que haya creado.
1. Haga clic en Guardar cuando termine.

Fácil, ¿verdad?

>[!NOTE]
>
>Aquí hay un [video de todo el proceso](https://nation.marketo.com/videos/1475) que debería dejar el proceso muy claro!

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)
