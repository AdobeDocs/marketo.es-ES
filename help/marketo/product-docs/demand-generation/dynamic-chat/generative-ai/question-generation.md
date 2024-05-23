---
description: Generación de preguntas - Documentos de Marketo - Documentación del producto
title: Generación de preguntas
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: b2ceefb068005d916027fb71be0dc4e25849ae23
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Generación de preguntas {#question-generation}

Vea todas las tareas y sus detalles pertinentes, como cuándo se generaron, la cantidad total de preguntas, el estado de aprobación y más.

## Generar preguntas {#generate-questions}

1. En IA generativa, haga clic en **[!UICONTROL Respuestas asistidas]**.

   ![](assets/question-generation-1.png)

1. Clic **[!UICONTROL Generación de preguntas]**.

   ![](assets/question-generation-2.png)

1. Asigne un nombre a la tarea e introduzca una dirección URL de origen (hasta 10) desde la que se extraerá todo el contenido. Introduzca los temas/palabras clave deseados y pulse Enter en el teclado. Cuando termine, haga clic en **[!UICONTROL Generar]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Para garantizar que el Marketo Engage pueda crear secuencias de comandos de contenido desde las direcciones URL proporcionadas, primero debe realizar la lista de permitidos de varias direcciones IP. [Consulte a continuación para obtener más información](#ip-addresses-to-allowlist).

1. En función de su contenido, la generación de preguntas y respuestas puede tardar hasta 30 minutos. Clic **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Pulse Actualizar para ver el último estado de la generación de preguntas.

   ![](assets/question-generation-5.png)

## Descargar preguntas y respuestas {#download-questions-and-responses}

>[!NOTE]
>
>Las preguntas y respuestas generadas también se pueden ver en [Biblioteca de respuestas](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Busque la tarea deseada y haga clic en el icono de descarga junto a su nombre.

   ![](assets/question-generation-6.png)

1. Busque la carpeta de descargas en el explorador y seleccione el archivo. Este aspecto puede variar según el explorador que utilice.

   ![](assets/question-generation-7.png)

1. En el archivo de Excel, **[!DNL Task details]** muestra solo eso, varios detalles sobre la tarea, incluidas instrucciones sobre cómo agregar o editar preguntas o respuestas.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Si decide añadir/editar preguntas y/o respuestas de forma masiva, [obtenga información sobre cómo volver a cargarlos aquí](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. El **[!DNL Q&Rs]** proporciona detalles adicionales, incluidas las preguntas y respuestas generadas.

   ![](assets/question-generation-9.png)

## Direcciones IP para Lista de permitidos {#ip-addresses-to-allowlist}

Para permitir la extracción de contenido de las URL de su web durante la generación de preguntas y respuestas, busque su región a continuación y asegúrese de que su equipo web haya incluido en la lista de permitidos todas las direcciones IP asociadas con ella.

<table width="450">
<thead>
  <tr>
    <th>América del Norte</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>20.10.235.188</td>
    <td>20.76.246.248</td>
    <td>20.167.0.195</td>
  </tr>
  <tr>
    <td>20.10.235.189</td>
    <td>20.76.247.92</td>
    <td>20 248 128 31</td>
  </tr>
  <tr>
    <td>20.10.235.246</td>
    <td>20.76.247.134</td>
    <td>20 167 1 48</td>
  </tr>
  <tr>
    <td>20.10.235.248</td>
    <td>20.76.247.244</td>
    <td>20 167 1 63</td>
  </tr>
  <tr>
    <td>20.10.235.255</td>
    <td>20.93.168.10</td>
    <td>20 167 1 92</td>
  </tr>
  <tr>
    <td>20.10.236.96</td>
    <td>20.93.168.44</td>
    <td>20.167.1.155</td>
  </tr>
  <tr>
    <td>20.119.144.14</td>
    <td>20.105.224.16</td>
    <td>20.211.64.11</td>
  </tr>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20 213 91 77</td>
  </tr>
</tbody>
</table>
