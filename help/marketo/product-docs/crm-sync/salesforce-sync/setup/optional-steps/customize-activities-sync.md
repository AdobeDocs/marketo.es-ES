---
unique-page-id: 4719294
description: Personalizar sincronización de actividades - Documentos de Marketo - Documentación del producto
title: Personalizar sincronización de actividades
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 4%

---

# Personalizar sincronización de actividades {#customize-activities-sync}

Si no utiliza Marketo Sales Insight, Marketo Engage puede crear Registros de historial de actividades de Salesforce para determinados eventos. A continuación se indica cómo habilitarlos.

1. Ir a **[!UICONTROL Administrador]**.

   ![](assets/admin.png)

1. Clic **[!DNL Salesforce]**, luego haga clic en **[!UICONTROL Editar opciones de sincronización]**.

   ![](assets/two-1.png)

1. Marque las casillas junto a las actividades que Marketo debe insertar en Salesforce y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una vez habilitado, Marketo insertará un historial de actividades de tres meses. Según la cantidad de datos, _esta operación podría tardar varios días en completarse_. Las actualizaciones que se producen durante la inserción inicial de Actividades se pueden retrasar hasta que se completa la sincronización inicial de Actividades.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Tipo de actividad</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Completó el formulario</td> 
   <td>Rellenó cualquier formulario de Marketo</td> 
  </tr> 
  <tr> 
   <td>Añadido a la lista</td> 
   <td><p>Paso de flujo: Se ha añadido a una lista estática</p></td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Paso de flujo: se envió un correo electrónico</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Se ha recibido un correo electrónico (no devuelto)</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico abierto</td> 
   <td>Apertura de un correo electrónico (sin bloquear imágenes)</td> 
  </tr> 
  <tr> 
   <td>Hizo clic en el vínculo del email</td> 
   <td>Se ha hecho clic en un vínculo de un correo electrónico enviado por Marketo</td> 
  </tr> 
  <tr> 
   <td>Eliminado de la lista</td> 
   <td>Paso de flujo: se ha eliminado de una lista estática</td> 
  </tr> 
  <tr> 
   <td>Quitar de flujo</td> 
   <td>Paso de flujo: Eliminar del flujo</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas enviado</td> 
   <td>Se ha enviado un correo electrónico a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas abierto</td> 
   <td>Se ha abierto un correo electrónico enviado a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Haga clic en el vínculo del correo electrónico de ventas</td> 
   <td>Se ha hecho clic en un vínculo de un correo electrónico enviado a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td>El representante de ventas recibió y registró un correo electrónico en el complemento MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Correo electrónico de ventas recibido&quot; sí _no_ media entregada. El estado de entrega no se captura para los correos electrónicos enviados mediante Sales Insight.

>[!TIP]
>
>Si está interesado en obtener más información de Marketo en Salesforce, consulte nuestra [Perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} producto.
