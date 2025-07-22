---
description: 'Paso 1 de 3: Agregar campos de Marketo a  [!DNL Veeva] CRM - Documentos de Marketo - Documentación del producto'
title: 'Paso 1 de 3: Agregar campos de Marketo a  [!DNL Veeva] CRM'
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# Paso 1 de 3: Agregar campos de Marketo a [!DNL Veeva] CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>La instancia de CRM [!DNL Veeva] debe tener acceso a las API de Salesforce para sincronizar datos entre Marketo Engage y CRM [!DNL Veeva].

Marketo Engage utiliza un conjunto de campos para capturar determinados tipos de información relacionada con el marketing. Si desea estos datos en [!DNL Veeva] CRM, siga las instrucciones a continuación.

`1.` Crear un campo personalizado en [!DNL Veeva] CRM en los objetos de contacto: Puntuación

`2.` Si lo desea, puede crear campos adicionales (consulte la tabla siguiente).

Todos estos campos personalizados son opcionales y no son necesarios para sincronizar Marketo Engage y [!DNL Veeva] CRM.

## Agregar campos de Marketo a [!DNL Veeva] CRM {#add-marketo-fields-to-veeva-crm}

Agregue un campo personalizado a los objetos de contacto y posible cliente de [!DNL Veeva] CRM enumerados anteriormente. Si desea agregar más, consulte la tabla de campos disponibles al final de esta sección.

Siga estos pasos para agregar el campo Score.

1. Inicie sesión en [!DNL Veeva] CRM y haga clic en **[!UICONTROL Configurar]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Haga clic en **[!UICONTROL Objetos y campos]** y seleccione **[!UICONTROL Administrador de objetos]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. En la barra de búsqueda, busque &quot;Contacto&quot;.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Haga clic en el objeto **[!UICONTROL Contact]**.

1. Seleccione **[!UICONTROL Campos y relaciones]**.

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Elija el tipo de campo adecuado (para Puntuación - número).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Escriba **[!UICONTROL Etiqueta de campo]**, **[!UICONTROL Longitud]** y **[!UICONTROL Nombre de campo]** para el campo, como se muestra en la tabla siguiente.

<table>
 <tbody>
  <tr>
   <th>Etiqueta del campo
   <th>Nombre del campo
   <th>Tipo de datos
   <th>Atributos de campo
  </tr>
  <tr>
   <td>Puntuación</td>
   <td>mkto71_Lead_Score</td>
   <td>Número</td>
   <td>Longitud 10<br/>
Cifras decimales 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Veeva] CRM anexa __c a los nombres de campo cuando los utiliza para crear nombres de API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Los campos de texto y número requieren una longitud, pero los campos de fecha y hora no. Una descripción es opcional.

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Especifique la configuración de acceso y haga clic en **[!UICONTROL Siguiente]**.

1. Definir todos los roles en **[!UICONTROL Visible]** y **[!UICONTROL Solo lectura]**.

1. Desactive la casilla de verificación **[!UICONTROL Solo lectura]** para el perfil del usuario de sincronización:

* Si tiene un usuario con el perfil de un administrador del sistema como usuario de sincronización, desactive la casilla de verificación [!UICONTROL Solo lectura] para el perfil del administrador del sistema (como se muestra a continuación).
* Si creó un perfil personalizado para el usuario de sincronización, desactive la casilla de verificación [!UICONTROL Solo lectura] para ese perfil personalizado.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Elija los diseños de página que deben mostrar el campo.

1. Haga clic en **[!UICONTROL Guardar y nuevo]** para volver y crear los otros dos campos personalizados.

1. Haz clic en **[!UICONTROL Guardar]** cuando hayas terminado con los tres.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Al agregar el campo al objeto Contact, también se agregan al objeto Person Account.

OPCIONAL: utilice el procedimiento anterior para cualquier campo personalizado adicional de la tabla siguiente.

<table>
 <tbody>
  <tr>
   <th>Etiqueta del campo
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
>Los valores de los campos asignados automáticamente por Marketo no estarán disponibles inmediatamente en [!DNL Veeva] CRM cuando se haya creado el nuevo campo. Marketo sincronizará los datos con [!DNL Veeva] CRM la próxima vez que se actualice el registro en cualquiera de los sistemas (es decir, una actualización de cualquiera de los campos sincronizados entre Marketo y [!DNL Veeva] CRM).
