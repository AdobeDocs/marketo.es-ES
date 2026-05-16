---
description: Comprenda los déclencheur, filtros y pasos de flujo de SMS en campañas inteligentes. Segmente y déclencheur campañas usando la actividad y las listas de SMS de Vibes.
title: Usar opciones de SMS en una campaña inteligente
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
TQID: https://experienceleague.adobe.com/wpXQpXx-Og5t9TJtlZnuXS2sgGkdDPYv7n5ehPSPHC4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 420
ht-degree: 7%

---

# Usar opciones de SMS en una campaña inteligente {#using-sms-options-in-a-smart-campaign}

Después de [crear un mensaje SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, querrás usar déclencheur de listas inteligentes y filtros dentro de una campaña inteligente para obtener los beneficios.

>[!NOTE]
>
>Si deseas enviar un mensaje SMS, tenemos un [artículo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} específico para ese caso.

>[!PREREQUISITES]
>
>Los déclencheur/filtros SMS solo aparecen si el servicio [Vibes se ha habilitado](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## DÉCLENCHEUR de SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

A continuación se muestran algunos ejemplos:

El déclencheur **Devoluciones de mensajes SMS** inicia un flujo, como enviar un correo electrónico, cuando se devuelve un mensaje SMS.

El déclencheur **Suscribirse a la lista de vibraciones** inicia un flujo cuando una persona se suscribe.

El déclencheur **Clicks Link in SMS Message** inicia un flujo cuando una persona hace clic en un vínculo del mensaje SMS.

## Filtros SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

El filtro **Suscrito a la lista de vibraciones** encuentra a cualquiera que se haya suscrito a vibraciones *alguna vez*. Esto incluye tanto a las personas sin suscribir como a las eliminadas, aunque estas se omitan del flujo. Este filtro es el más adecuado para los informes.

Por el contrario, el filtro **Lista de miembros de vibraciones** encuentra a *cualquiera* suscrito actualmente a vibraciones y es el más adecuado para usarlo en campañas o listas inteligentes.

>[!NOTE]
>
>Todos los filtros de SMS incluyen la restricción **Fecha de actividad** de forma predeterminada.

## Pasos de flujo de SMS {#sms-flow-steps}

Hay tres pasos de flujo de SMS para elegir.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Enviar mensaje SMS</b></td>
    <td>Esta acción de flujo envía mensajes a las personas de la lista inteligente de Marketo suscritas a una lista de suscripción de Vibes seleccionada por el usuario. No inicia el proceso de suscripción. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">Más información</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>Suscribirse a la lista de Vibes</b></td>
    <td>Esta acción de flujo inicia el proceso de suscripción de SMS mediante una campaña de adquisición de vibraciones seleccionada por el usuario. A continuación, Vibes envía un mensaje de confirmación y el destinatario debe responder con "Y" en un plazo de 24 horas para confirmar la inclusión. Una vez que el usuario se haya suscrito, pasará a ser miembro de su lista de suscripción de Vibes asociada.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Cancelar suscripción a la lista de Vibes</b></td>
    <td>Esta acción de flujo cancela la suscripción de cada persona a una lista de suscripción de Vibes seleccionada por el usuario. Cuando un usuario envía un mensaje de texto "STOP" a su código, el registro de persona se actualiza para reflejar que ya no es miembro de la lista de suscripción a Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Los flujos **Suscribirse a la lista de vibraciones** y **Cancelar la suscripción a la lista de vibraciones** tienen requisitos diferentes. Para **Suscribirse**, debe seleccionar la lista Vibes y la campaña de adquisición Vibes. Para **Cancelar la suscripción**, solo se requiere la lista de vibraciones.

>[!MORELIKETHIS]
>
>* [Enviar un mensaje SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definir lista inteligente para campaña inteligente | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definir lista inteligente para campaña inteligente | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
