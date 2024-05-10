---
description: Generación de preguntas - Documentos de Marketo - Documentación del producto
title: Generación de preguntas
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: a6745e4a5321000bc1c91ef99c5f265b4c6c5760
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Generación de preguntas {#question-generation}

Vea todas las tareas y sus detalles relevantes, como cuándo se generaron, la cantidad total de preguntas, el estado de aprobación y más.

## Generar preguntas {#generate-questions}

1. En IA generativa, haga clic en **Respuestas asistidas**.

   ![](assets/question-generation-1.png)

1. Clic **Generación de preguntas**.

   ![](assets/question-generation-2.png)

1. Asigne un nombre a la tarea e introduzca una dirección URL de origen (hasta 50) desde la que se extraerá todo el contenido. Introduzca los temas/palabras clave deseados y pulse Enter en el teclado. Cuando termine, haga clic en **Generar**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Para garantizar que el Marketo Engage pueda crear secuencias de comandos de contenido desde las direcciones URL proporcionadas, primero debe realizar la lista de permitidos de varias direcciones IP. [Consulte a continuación para obtener más información](#ip-addresses-to-allowlist).

1. En función de su contenido, la generación de preguntas y respuestas puede tardar hasta 30 minutos. Clic **OK**.

   ![](assets/question-generation-4.png)

>[!TIP]
>
>El estado de la página no se actualiza en tiempo real. Pulse Actualizar para ver cuándo pasa de &quot;Procesando&quot; a &quot;Completado&quot;.

![](assets/question-generation-5.png)

## Descargar preguntas y respuestas {#download-questions-and-responses}

>[!NOTE]
>
>Las preguntas y respuestas generadas también se pueden ver en [Biblioteca de respuestas](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Busque la tarea deseada y haga clic en el icono de descarga junto a su nombre.

   ![](assets/question-generation-6.png)

1. Busque la carpeta de descargas en el explorador y seleccione el archivo. Este aspecto puede variar según el explorador.

   ![](assets/question-generation-7.png)

1. En el archivo de Excel, **Detalles de tarea** muestra solo eso, varios detalles sobre la tarea, incluidas instrucciones sobre cómo agregar o editar preguntas o respuestas.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Si decide editar de forma masiva las preguntas o respuestas, [obtenga información sobre cómo volver a cargarlos aquí](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. El **Preguntas y respuestas** proporciona detalles adicionales, incluidas las preguntas y respuestas generadas.

   ![](assets/question-generation-9.png)

## Direcciones IP para Lista de permitidos {#ip-addresses-to-allowlist}

Para permitir la extracción de contenido de las URL de su web durante la generación de preguntas y respuestas, asegúrese de que su equipo web haya incluido en la lista de permitidos todas las direcciones IP siguientes.

<table width="150">
  <tr>
    <td>20.167.0.149</td>
  </tr>
  <tr>
    <td>20 248 129 111</td>
  </tr>
  <tr>
    <td>20.167.0.146</td>
  </tr>
  <tr>
    <td>20.167.0.205</td>
  </tr>
  <tr>
    <td>20 248 135,80</td>
  </tr>
  <tr>
    <td>20.92.173.115</td>
  </tr>
  <tr>
    <td>20.167.0.195</td>
  </tr>
  <tr>
    <td>20 248 128 31</td>
  </tr>
  <tr>
    <td>20 167 1 48</td>
  </tr>
  <tr>
    <td>20 167 1 63</td>
  </tr>
  <tr>
    <td>20 167 1 92</td>
  </tr>
  <tr>
    <td>20.167.1.155</td>
  </tr>
  <tr>
    <td>20 248 135 132</td>
  </tr>
  <tr>
    <td>20 248 135 108</td>
  </tr>
  <tr>
    <td>20 248 134 140</td>
  </tr>
  <tr>
    <td>20 167 1 242</td>
  </tr>
  <tr>
    <td>20.167.0.198</td>
  </tr>
  <tr>
    <td>20 248 133 185</td>
  </tr>
  <tr>
    <td>20 248 134 190</td>
  </tr>
  <tr>
    <td>20 167 1 254</td>
  </tr>
  <tr>
    <td>20 248 128 118</td>
  </tr>
  <tr>
    <td>20 248 131 252</td>
  </tr>
  <tr>
    <td>20.167.0.188</td>
  </tr>
  <tr>
    <td>20.167.0.201</td>
  </tr>
  <tr>
    <td>20.211.64.11</td>
  </tr>
  <tr>
    <td>20.76.243.87</td>
  </tr>
  <tr>
    <td>20.76.244.212</td>
  </tr>
  <tr>
    <td>20.76.245.48</td>
  </tr>
  <tr>
    <td>20.76.245.76</td>
  </tr>
  <tr>
    <td>20.76.246.63</td>
  </tr>
  <tr>
    <td>20.76.246.146</td>
  </tr>
  <tr>
    <td>20.76.246.248</td>
  </tr>
  <tr>
    <td>20.76.247.92</td>
  </tr>
  <tr>
    <td>20.76.247.134</td>
  </tr>
  <tr>
    <td>20.76.247.244</td>
  </tr>
  <tr>
    <td>20.93.168.10</td>
  </tr>
  <tr>
    <td>20.93.168.44</td>
  </tr>
  <tr>
    <td>20.93.168.137</td>
  </tr>
  <tr>
    <td>20.93.169.20</td>
  </tr>
  <tr>
    <td>20.93.169.115</td>
  </tr>
  <tr>
    <td>20.93.169.214</td>
  </tr>
  <tr>
    <td>20.93.170.130</td>
  </tr>
  <tr>
    <td>20.93.170.138</td>
  </tr>
  <tr>
    <td>20.93.170.149</td>
  </tr>
  <tr>
    <td>20.93.172.63</td>
  </tr>
  <tr>
    <td>20.93.173.217</td>
  </tr>
  <tr>
    <td>20.93.173.243</td>
  </tr>
  <tr>
    <td>20.93.174.120</td>
  </tr>
  <tr>
    <td>20.93.174.159</td>
  </tr>
  <tr>
    <td>20.105.224.16</td>
  </tr>
  <tr>
    <td>20.10.235.102</td>
  </tr>
  <tr>
    <td>20.10.235.103</td>
  </tr>
  <tr>
    <td>20.10.235.143</td>
  </tr>
  <tr>
    <td>20.10.235.146</td>
  </tr>
  <tr>
    <td>20.10.235.147</td>
  </tr>
  <tr>
    <td>20.10.235.148</td>
  </tr>
  <tr>
    <td>20.10.235.188</td>
  </tr>
  <tr>
    <td>20.10.235.189</td>
  </tr>
  <tr>
    <td>20.10.235.246</td>
  </tr>
  <tr>
    <td>20.10.235.248</td>
  </tr>
  <tr>
    <td>20.10.235.255</td>
  </tr>
  <tr>
    <td>20.10.236.96</td>
  </tr>
  <tr>
    <td>20.10.236.97</td>
  </tr>
  <tr>
    <td>20.10.236.110</td>
  </tr>
  <tr>
    <td>20.10.236.11</td>
  </tr>
  <tr>
    <td>20.10.235.254</td>
  </tr>
  <tr>
    <td>20.10.236.138</td>
  </tr>
  <tr>
    <td>20.10.236.139</td>
  </tr>
  <tr>
    <td>20.10.236.140</td>
  </tr>
  <tr>
    <td>20.10.236.141</td>
  </tr>
  <tr>
    <td>20.10.236.84</td>
  </tr>
  <tr>
    <td>20.10.236.85</td>
  </tr>
  <tr>
    <td>20.10.236.86</td>
  </tr>
  <tr>
    <td>20.10.236.87</td>
  </tr>
  <tr>
    <td>20.119.144.14</td>
  </tr>
  <tr>
    <td>20.75.41.107</td>
  </tr>
  <tr>
    <td>20.75.43.104</td>
  </tr>
  <tr>
    <td>20.75.43.107</td>
  </tr>
  <tr>
    <td>20.75.43.113</td>
  </tr>
  <tr>
    <td>20.75.43.124</td>
  </tr>
  <tr>
    <td>20.75.43.204</td>
  </tr>
  <tr>
    <td>20.75.43.207</td>
  </tr>
  <tr>
    <td>20.75.43.214</td>
  </tr>
  <tr>
    <td>20.75.43.220</td>
  </tr>
  <tr>
    <td>20.75.44.0</td>
  </tr>
  <tr>
    <td>20.75.44.9</td>
  </tr>
  <tr>
    <td>20.75.44.52</td>
  </tr>
  <tr>
    <td>20.75.44.66</td>
  </tr>
  <tr>
    <td>20.75.44.82</td>
  </tr>
  <tr>
    <td>20.75.44.105</td>
  </tr>
  <tr>
    <td>20.75.44.108</td>
  </tr>
  <tr>
    <td>20.75.44.133</td>
  </tr>
  <tr>
    <td>20.75.44.135</td>
  </tr>
  <tr>
    <td>20.75.44.137</td>
  </tr>
  <tr>
    <td>20.75.44.147</td>
  </tr>
  <tr>
    <td>20.75.44.154</td>
  </tr>
  <tr>
    <td>20.75.44.195</td>
  </tr>
  <tr>
    <td>20.75.44.198</td>
  </tr>
  <tr>
    <td>20.75.45.32</td>
  </tr>
  <tr>
    <td>20 119 136 14</td>
  </tr>
  <tr>
    <td>172 177 93 157</td>
  </tr>
  <tr>
    <td>52 252 22 155</td>
  </tr>
  <tr>
    <td>20.62.18.64</td>
  </tr>
  <tr>
    <td>52 179 234 0</td>
  </tr>
  <tr>
    <td>52 179 234,1</td>
  </tr>
  <tr>
    <td>52 179 237 99</td>
  </tr>
  <tr>
    <td>52 179 237 148</td>
  </tr>
  <tr>
    <td>52 252 23 246</td>
  </tr>
  <tr>
    <td>52 253 64 47</td>
  </tr>
  <tr>
    <td>52 253 64 124</td>
  </tr>
  <tr>
    <td>52 253 64 125</td>
  </tr>
  <tr>
    <td>52 253 65 84</td>
  </tr>
  <tr>
    <td>52 253 65 85</td>
  </tr>
  <tr>
    <td>52 254 103 240</td>
  </tr>
  <tr>
    <td>52 253 65 92</td>
  </tr>
  <tr>
    <td>52 253 65 93</td>
  </tr>
  <tr>
    <td>52 177 89 135</td>
  </tr>
  <tr>
    <td>52 253 69 207</td>
  </tr>
  <tr>
    <td>52 253 69 240</td>
  </tr>
  <tr>
    <td>52 167 19 211</td>
  </tr>
  <tr>
    <td>52 177 147 229</td>
  </tr>
  <tr>
    <td>40.65.238.53</td>
  </tr>
  <tr>
    <td>52 177 147 249</td>
  </tr>
  <tr>
    <td>20.44.83.102</td>
  </tr>
  <tr>
    <td>52 177 148 19</td>
  </tr>
  <tr>
    <td>20.49.97.17</td>
  </tr>
  <tr>
    <td>20.14.171.7</td>
  </tr>
  <tr>
    <td>172 177 93 157</td>
  </tr>
  <tr>
    <td>20 213 91 77</td>
  </tr>
  <tr>
    <td>20.105.150.224</td>
  </tr>
  <tr>
    <td>13.68.17.252</td>
  </tr>
</table>