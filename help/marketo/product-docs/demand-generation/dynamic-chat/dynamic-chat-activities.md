---
description: Actividades del Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Actividades del Dynamic Chat
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: b1101617ec670d42aed8c35044b656ba5fa0f9f5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Actividades del Dynamic Chat {#dynamic-chat-activities}

Dynamic Chat ofrece varios filtros y déclencheur para utilizarlos en sus listas inteligentes.

![](assets/dynamic-chat-activities-1.png)

## Definiciones {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td><b>Activado</b></td>
    <td>Un evento de déclencheur se produce cuando un visitante cumple los criterios de segmentación de un flujo de diálogo o conversación y se muestra en el cuadro de diálogo.
    <br>Un evento de déclencheur por visitante y sesión.</td>
  </tr>
  <tr>
    <td><b>Participación con un flujo/diálogo de conversación</b></td>
    <td>La primera vez que un visitante web hace clic en un mensaje en un flujo de diálogo o conversación (haciendo clic en una opción de opción múltiple, enviando información, reservando una reunión, abriendo un documento, etc.) se produce una participación. Si un visitante abre un diálogo o un flujo de conversación, pero no hace clic en un mensaje, se genera una participación <b>no</b> registrado. 
    <br>Un evento de participación por visitante y sesión.</td>
  </tr>
   <tr>
    <td><b>Interacción con un agente</b></td>
    <td>Sucede cuando un visitante se conecta correctamente a un agente de chat en directo.
    <br>Uno relacionado con el evento del agente por visitante y por sesión.</td>
  </tr>
  <tr>
    <td><b>Interactuó con el documento</b></td>
    <td>Sucede cuando un visitante hace clic en un documento de una tarjeta de documento.
    <br>Puede haber varias interacciones de documentos por visitante y por sesión.</td>
  </tr>
  <tr>
    <td><b>Meta(s) alcanzada(s)</b></td>
    <td>Sucede cuando un visitante alcanza una meta. <br>Puede haber varios eventos objetivo por visitante y por sesión.</td>
  </tr>
  <tr>
    <td><b>Reunión programada</b></td>
    <td>Sucede cuando un visitante reserva una reunión con un agente de Dynamic Chat.
    <br>Puede haber varios eventos reservados para reuniones por visitante y por sesión.</td>
  </tr>
</tbody>
</table>

## Cosas que hay que tener en cuenta {#things-to-note}

* Las condiciones son compatibles con los pasos de flujo del Dynamic Chat
* Las actividades del Dynamic Chat se pueden sincronizar con [Perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Puede ver actividades de Dynamic Chat individuales en el registro de actividad de una persona
