---
unique-page-id: 4719294
description: Sincronización de Actividades personalizadas - Documentos de marketing - Documentación del producto
title: Sincronización de Actividades personalizadas
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Sincronización de Actividades personalizadas {#customize-activities-sync}

Si no utiliza [Sales Insight](http://docs.marketo.com/display/DOCS/Marketo+Sales+Insight), Marketing puede crear registros del historial de Actividades de Salesforce para determinados eventos. Así es como habilitarlos.

1. Vaya a **Administración. **

   ![](assets/admin.png)

1. Haga clic en **Salesforce** y, a continuación, en **Editar opciones** de sincronización.

   ![](assets/two-1.png)

1. Marque las casillas situadas junto a actividades que desee que Marketing envíe a Salesforce y haga clic en **Guardar**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una vez habilitado, Marketing impulsará tres meses de historia de actividad. En función de la cantidad de datos, *esto podría tardar varios días en completarse*. Las actualizaciones que se producen durante la inserción de Actividades iniciales pueden retrasarse hasta que se complete la sincronización de Actividades iniciales.

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
   <td>Formulario rellenado</td> 
   <td>Se completó cualquier formulario de marketing</td> 
  </tr> 
  <tr> 
   <td>Añadido a la lista</td> 
   <td><p>Paso de flujo: Se agregó a una lista estática</p></td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Paso de flujo: Se ha enviado un correo electrónico</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Recibió un correo electrónico (no devuelto)</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico abierto</td> 
   <td>Se abrió un correo electrónico (sin bloquear imágenes)</td> 
  </tr> 
  <tr> 
   <td>Se ha hecho clic en el vínculo en el correo electrónico</td> 
   <td>Se ha hecho clic en un vínculo de un mensaje de correo electrónico enviado por Marketo</td> 
  </tr> 
  <tr> 
   <td>Eliminado de la lista</td> 
   <td>Paso de flujo: Se eliminó de una lista estática</td> 
  </tr> 
  <tr> 
   <td>Quitar del flujo</td> 
   <td>Paso de flujo: Quitar del flujo</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas enviado</td> 
   <td>Se envió un mensaje de correo electrónico a través de Marketingto Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas abierto</td> 
   <td>Se abrió un correo electrónico enviado a través de MarketingTo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Haga clic en el vínculo del correo electrónico de ventas</td> 
   <td>Se ha hecho clic en un vínculo de un mensaje de correo electrónico enviado a través de Marketing to Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td>El representante de ventas recibió y registró un correo electrónico en el complemento MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Recordatorio**
>
>
>&quot;Correo electrónico de ventas recibido&quot; **no significa que** se haya enviado. El estado de entrega no se captura para los correos electrónicos enviados mediante Sales Insight.

>[!TIP]
>
>Si le interesa obtener más información sobre el marketing en Salesforce, consulte nuestro producto [de Marketing Sales Insight](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) .

