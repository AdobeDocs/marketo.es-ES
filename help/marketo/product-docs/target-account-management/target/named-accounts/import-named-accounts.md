---
unique-page-id: 12615800
description: Importar [!UICONTROL Cuentas Con Nombre] - Documentos De Marketo - Documentación Del Producto
title: Importar [!UICONTROL Cuentas con nombre]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Importar [!UICONTROL Cuentas con nombre] {#import-named-accounts}

¿Ya tiene un CSV lleno de posibles cuentas de destinatario? ¡Importarlos directamente en TAM!

1. Haga clic en el menú desplegable **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Importar cuentas con nombre]**.

   ![](assets/inaone.png)

1. Se abrirá una nueva ventana. Haga clic en **[!UICONTROL Examinar]** y, a continuación, seleccione el archivo de cuentas con nombre que desee importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >En su archivo, proporcione [tanta información](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) como sea posible. Solo puede agregar información firmográfica; no hay nada que Marketo calcule (es decir, Canalización). Para crear cuentas con nombre basadas en cuentas de CRM, simplemente exporte el nombre de la cuenta y el ID de CRM desde su CRM a un archivo CSV, utilice la opción Nombre de cuenta y asigne el ID de CRM durante el proceso de importación. Para vincular correctamente una cuenta CRM a una cuenta con nombre, debe proporcionar el nombre exacto de la cuenta CRM.

1. Elija entre dos modos desduplicados: Nombre de cuenta o Nombre de dominio. En este ejemplo, elegimos Cuenta. Haga clic en el menú desplegable **[!UICONTROL Modos]** y seleccione **[!UICONTROL Por nombre de cuenta]**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Si elige **[!UICONTROL Por nombre de dominio]**, se deben incluir los campos de cuenta con nombre y dominio.

1. Para elegir a qué lista de cuentas se agrega su cuenta con nombre, haga clic en la lista desplegable **[!UICONTROL Lista de cuentas]** y realice la selección.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >También puede crear una [!UICONTROL lista de cuentas] completamente nueva simplemente escribiendo su nombre en el cuadro desplegable.

1. Para enviar una notificación sobre la importación, haz clic en el menú desplegable **[!UICONTROL Enviar alerta a]** y selecciona un usuario de Marketo. Usted _no puede_ escribir manualmente una dirección de correo electrónico.

   ![](assets/inafive-2.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/inasix-2.png)

1. Asigne cada campo haciendo doble clic en la lista desplegable **[!UICONTROL Campo de Marketo]** y seleccionando el campo correspondiente. Haga clic en **[!UICONTROL Siguiente]** cuando haya terminado.

   ![](assets/inaseven.png)

   ¡Éxito!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Comprobar estado de importación&quot; solo muestra los últimos tres días de actividad.

Situaciones en las que se desduplica [!UICONTROL por nombre de cuenta]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importando registro con nombre de <span class="uicontrol">Cuenta con nombre</span> existente</strong></td> 
   <td><p>Actualizaremos el registro existente</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro con el nuevo nombre de <span class="uicontrol">Cuenta con nombre</span></strong></td> 
   <td>Crearemos un nuevo registro</td> 
  </tr> 
 </tbody> 
</table>

Situaciones en las que se desduplica [!UICONTROL por nombre de dominio]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importación de un registro con un nuevo nombre de cuenta y un nuevo nombre de dominio</strong></td> 
   <td>Crearemos una nueva <span class="uicontrol">cuenta con nombre</span> con la información proporcionada</td> 
  </tr> 
  <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta existente y un nombre de dominio existente</strong></td> 
   <td>Actualizaremos la <span class="uicontrol">cuenta con nombre</span> existente</td> 
  </tr> 
   <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta nuevo y un nombre de dominio existente</strong></td> 
   <td>Anexaremos el nuevo nombre de cuenta a la <span class="uicontrol">cuenta con nombre</span> existente que coincida con el nombre de dominio y actualizaremos otra información (por ejemplo: sector, estado, etc.)</td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro con nombre de <span class="uicontrol">Cuenta con nombre</span> existente y nombre de dominio nuevo</strong></td> 
   <td>Anexaremos el nuevo nombre de dominio a la <span class="uicontrol">cuenta con nombre</span> existente que coincida con el nombre de la cuenta y actualizaremos otra información (por ejemplo: sector, estado, etc.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Cuando Marketo anexa una cuenta con nombre, estamos actualizando una regla (en segundo plano) que nos permite identificar a las personas que deberían ser parte de la [!UICONTROL cuenta con nombre]. Ejemplo: si actualiza &quot;IBM&quot; a &quot;IBM, USA&quot;, las personas con cualquiera de los nombres de compañía se asociarán a [!UICONTROL Cuenta con nombre].

Si Marketo encuentra registros que vemos como duplicados, solo procesaremos el primero.
