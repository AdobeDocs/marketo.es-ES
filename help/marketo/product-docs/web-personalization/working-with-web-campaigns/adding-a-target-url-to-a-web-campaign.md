---
unique-page-id: 6094879
description: 'Adición de una URL de destino a una campaña web: documentos de Marketo, documentación del producto'
title: Adición de una URL de destino a una campaña web
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Adición de una URL de destino a una campaña web {#adding-a-target-url-to-a-web-campaign}

Se encuentra una dirección URL de destino en la página Definir campaña y define la dirección URL o direcciones URL específicas en las que aparecerá una campaña web.

## Adición de una URL de destino para campañas web de cuadros de diálogo o widgets {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Vaya a **[!UICONTROL Campañas web]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Seleccione **[!UICONTROL Crear nueva campaña web]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Agregar **[!UICONTROL nombre de campaña]**. Seleccione un **[!UICONTROL Segmento de destino]**. Agregar **[!UICONTROL URL de destino]**.

   ![](assets/set-web-campaign-hands.jpg)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">Nombre</th>
   <th colspan="1" rowspan="1">Descripción</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Cualquier página]</strong></td>
   <td colspan="1" rowspan="1"><p>Permitir que la campaña aparezca en cualquier página.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL Incluir parámetro de URL al hacer coincidir]</strong></p></td>
   <td colspan="1" rowspan="1">Añada el parámetro de URL para que coincida y mostrar la campaña en las direcciones URL que incluyen este parámetro. P. ej. campaign=cpc</td>
  </tr>
 </tbody>
</table>

## Adición de varias direcciones URL en la dirección URL de destino {#adding-multiple-urls-to-target-url}

Al hacer clic en el icono de signo más (![—](assets/image2015-2-18-8-3a40-3a59.png)), se abrirá el cuadro de diálogo [!UICONTROL Entrada de varios valores] para agregar varias direcciones URL. Añada una dirección URL por línea.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Las campañas web de cuadros de diálogo y widgets pueden utilizar las opciones Cualquier página y Comodín (&#42;).
>* En casos de uso avanzados, las campañas web de la zona In pueden utilizar comodines al final de la ruta de la URL. Ejemplo: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* La URL distingue entre mayúsculas y minúsculas

## Adición de una URL de destino para campañas web en la zona {#adding-a-target-url-for-in-zone-web-campaigns}

1. Vaya a **[!UICONTROL Campañas web]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Seleccione **[!UICONTROL Crear nueva campaña web]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Agregar **[!UICONTROL nombre de campaña]**. Seleccione un **[!UICONTROL Segmento de destino]**. Agregar **[!UICONTROL URL de destino]**.

   >[!NOTE]
   >
   >La dirección URL de destino con zonas de entrada debe definir una dirección URL o direcciones URL específicas. En casos de uso avanzados, las campañas web de la zona In pueden utilizar comodines al final de la ruta de la URL. Ejemplo: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [Crear una campaña de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Crear una campaña de RTP en la zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Crear una campaña de widget de RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
