---
description: Sincronización de campos personalizados de miembros del programa - Documentos de Marketo - Documentación del producto
title: Sincronización de campo personalizado para miembros del programa
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 11%

---

# Sincronización de campo personalizado para miembros del programa {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Creación de [campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Sincronizar una [!DNL Salesforce] campaña con un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>El objeto Miembro de programa puede tener hasta 20 campos personalizados. Estos campos están disponibles para cualquier programa.

## Asignar campos de Salesforce a campos personalizados de miembros del programa {#map-salesforce-fields-to-program-member-custom-fields}

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Haga clic en **[!DNL Salesforce]** y luego en **[!UICONTROL Editar]** junto a Sincronización de campos personalizados de miembros del programa.

   ![](assets/program-member-custom-field-sync-2.png)

1. Utilice el cuadro de búsqueda para localizar los [!DNL Salesforce] campos que desea asignar. En este ejemplo, se utiliza No llamar.

   ![](assets/program-member-custom-field-sync-3.png)

1. Haga clic en la lista desplegable.

   ![](assets/program-member-custom-field-sync-4.png)

1. Elija el campo personalizado [!UICONTROL Miembro del programa] de Marketo que desee asignar.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >La lista desplegable solo mostrará [!UICONTROL Campos personalizados de miembro del programa] que coincidan con el tipo de datos del campo [!DNL Salesforce].

1. Para asignaciones de campos adicionales, borre el cuadro de búsqueda y repita los pasos del 3 al 5.

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >Los cambios en los datos de miembros del programa en los campos asignados se sincronizarán entre Marketo y [!DNL Salesforce] a partir de ahora.

   >[!NOTE]
   >
   >Si cambia el nombre o el tipo de datos de un campo de [!DNL Salesforce], se quitará cualquier asignación de ese campo con el [!UICONTROL Campo personalizado de miembro del programa]. Pero puede reasignarlo con el nuevo campo después de la revisión.

## Desasignar campos Salesforce de campos personalizados de miembros del programa {#unmap-salesforce-fields-from-program-member-custom-fields}

Si alguna vez desea liberar un campo para reemplazarlo o simplemente realizar un cambio general, primero debe realizar una desasignación. Así es como.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Haga clic en **[!DNL Salesforce]** y luego en **[!UICONTROL Editar]** junto a Sincronización de campos personalizados de miembros del programa.

   ![](assets/program-member-custom-field-sync-8.png)

1. Utilice el cuadro de búsqueda para localizar los campos que desea desasignar. En este ejemplo, se utiliza No llamar.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >Puede seleccionar la casilla de verificación **[!UICONTROL Asignado]** para ver solo los campos asignados.

1. Desasigne haciendo clic en **X** junto al campo.

   ![](assets/program-member-custom-field-sync-10.png)

1. La asignación se ha eliminado. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Asignación de tipos de datos {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Tipo de datos de SFDC</th>
      <th>Tipo de datos del campo personalizado del miembro del programa</th>
    </tr>
    <tr>
      <td>Texto</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Lista de selección</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Lista de selección múltiple</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Teléfono</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Correo electrónico</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Número(m)</td>
      <td>Entero</td>
    </tr>
    <tr>
      <td>Número(m,n)</td>
      <td>Flotante</td>
    </tr>
    <tr>
      <td>Casilla de verificación</td>
      <td>Booleano</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Fecha</td>
      <td>Fecha</td>
    </tr>
    <tr>
      <td>Fecha y hora</td>
      <td>Fecha y hora</td>
    </tr>
    <tr>
      <td>Búsqueda (referencia)</td>
      <td>Cadena</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>Cadena</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Cambiar datos de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Ver datos en la cuadrícula de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [Sincronización de SFDC: sincronización de Campaign](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
