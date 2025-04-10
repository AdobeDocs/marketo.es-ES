---
unique-page-id: 4719294
description: Personalizar sincronización de actividades - Documentos de Marketo - Documentación del producto
title: Personalizar sincronización de actividades
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 11%

---

# Personalizar sincronización de actividades {#customize-activities-sync}

Si no utiliza Marketo Sales Insight, Marketo Engage puede crear registros del historial de actividades de Salesforce para determinados eventos. A continuación se indica cómo habilitarlos.

>[!NOTE]
>
>La sincronización de Salesforce/Marketo Engage no insertará ninguna actividad en Salesforce que se haya producido antes de que la persona se insertara en Salesforce.

1. Ir a **[!UICONTROL Administrador]**.

   ![](assets/customize-activities-sync-1.png)

1. Haga clic en **[!DNL Salesforce]** y luego en **[!UICONTROL Editar opciones de sincronización]**.

   ![](assets/two-1.png)

1. Marque las casillas junto a las actividades que Marketo debe insertar en Salesforce y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una vez habilitado, Marketo insertará un historial de actividades de tres meses. Según la cantidad de datos, _esto podría tardar varios días en completarse_. Las actualizaciones que se producen durante la inserción inicial de Actividades se pueden retrasar hasta que se completa la sincronización inicial de Actividades.

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
   <td>Formulario completo</td> 
   <td>Rellenó cualquier formulario de Marketo</td> 
  </tr> 
  <tr> 
   <td>Se agregó a la lista</td> 
   <td><p>Paso de flujo: Se ha añadido a una lista estática</p></td> 
  </tr> 
  <tr> 
   <td>Se envió el email</td> 
   <td>Paso de flujo: se envió un correo electrónico</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico entregado</td> 
   <td>Se ha recibido un correo electrónico (no devuelto)</td> 
  </tr> 
  <tr> 
   <td>Se abrió el email</td> 
   <td>Apertura de un correo electrónico (sin bloquear imágenes)</td> 
  </tr> 
  <tr> 
   <td>Hizo clic en el vínculo del email</td> 
   <td>Se ha hecho clic en un vínculo de un correo electrónico enviado por Marketo</td> 
  </tr> 
  <tr> 
   <td>Se quitó de Lista</td> 
   <td>Paso de flujo: se ha eliminado de una lista estática</td> 
  </tr> 
  <tr> 
   <td>Quitar de Flujo</td> 
   <td>Paso de flujo: Eliminar del flujo</td> 
  </tr> 
  <tr> 
   <td>Se envió el email de ventas</td> 
   <td>Se ha enviado un correo electrónico a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Se abrió el email de ventas</td> 
   <td>Se ha abierto un correo electrónico enviado mediante Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Haga clic en el vínculo del correo electrónico de ventas</td> 
   <td>Se ha hecho clic en un vínculo de un correo electrónico enviado a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Se recibió el email de ventas</td> 
   <td>El representante de ventas recibió y registró un correo electrónico en el complemento MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Correo electrónico de ventas recibido&quot; significa _no_ entregado. El estado de entrega no se captura para los correos electrónicos enviados mediante Sales Insight.

>[!TIP]
>
>Si estás interesado en obtener más información sobre Marketo en Salesforce, echa un vistazo a nuestro producto [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
