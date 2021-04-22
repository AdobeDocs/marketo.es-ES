---
unique-page-id: 4719294
description: 'Sincronización de actividades de personalización: Documentos de Marketo: documentación del producto'
title: Personalizar sincronización de actividades
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Sincronización de actividades de personalización {#customize-activities-sync}

Si no utiliza Marketo Sales Insight, Marketo puede crear Registros del historial de actividades de Salesforce para determinados eventos. Así es como habilitarlos.

1. Vaya a **Admin**.

   ![](assets/admin.png)

1. Haga clic en **Salesforce** y, a continuación, haga clic en **Editar opciones de sincronización**.

   ![](assets/two-1.png)

1. Marque las casillas situadas junto a las actividades que desea que Marketo inserte en Salesforce y haga clic en **Guardar**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una vez habilitado, Marketo inserta el historial de actividades de tres meses. Dependiendo de la cantidad de datos, _esto podría tardar varios días en completarse_. Las actualizaciones que se producen durante la notificación push inicial de Actividades pueden retrasarse hasta que se complete la sincronización inicial de Actividades.

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
   <td>Se ha rellenado cualquier formulario de Marketo</td> 
  </tr> 
  <tr> 
   <td>Se ha añadido a la lista</td> 
   <td><p>Paso de flujo: Se agregó a una lista estática</p></td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Paso de flujo: Se ha enviado un correo electrónico</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico enviado</td> 
   <td>Se ha recibido un correo electrónico (no devuelto)</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico abierto</td> 
   <td>Se ha abierto un correo electrónico (sin bloquear imágenes)</td> 
  </tr> 
  <tr> 
   <td>Se hizo clic en el vínculo en el correo electrónico</td> 
   <td>Se hizo clic en un vínculo de un correo electrónico enviado por Marketo</td> 
  </tr> 
  <tr> 
   <td>Eliminado de la lista</td> 
   <td>Paso de flujo: Se ha eliminado de una lista estática</td> 
  </tr> 
  <tr> 
   <td>Eliminar del flujo</td> 
   <td>Paso de flujo: Eliminar del flujo</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas enviado</td> 
   <td>Se ha enviado un correo electrónico a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas abierto</td> 
   <td>Apertura de un correo electrónico enviado a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Haga clic en el vínculo en el correo electrónico de ventas</td> 
   <td>Se hizo clic en un vínculo de un correo electrónico enviado a través de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico de ventas recibido</td> 
   <td>El representante de ventas recibió y registró un correo electrónico en el complemento de MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Correo electrónico de ventas recibido&quot; significa **no** entregado. El estado de entrega no se captura para los correos electrónicos enviados mediante la perspectiva de ventas.

>[!TIP]
>
>Si está interesado en obtener más información de Marketo en Salesforce, consulte nuestro [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) producto.
