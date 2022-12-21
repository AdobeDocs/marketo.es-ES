---
unique-page-id: 11380774
description: Puntuación de cuenta - Documentos de Marketo - Documentación del producto
title: Puntuación de la cuenta
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Puntuación de la cuenta {#account-score}

La Puntuación de cuentas es una parte vital de la Administración de cuentas de Target. Le ayuda a determinar el nivel de participación de sus cuentas.

## ¿Qué es la puntuación de la cuenta? {#what-is-account-scoring}

Es un enfoque sistemático diseñado para ayudar a los equipos de ventas y marketing a identificar y priorizar las empresas (incluidos los posibles clientes) que tienen más probabilidades de realizar una compra.

En el complejo mundo de los procesos de compra B2B, es raro que una sola persona tome una decisión de compra. A menudo hay varias funciones involucradas, cada una con sus propias necesidades. La puntuación basada en cuentas lo tiene en cuenta agregando las puntuaciones de posible cliente de varios posibles clientes y proporcionando una puntuación a nivel de cuenta.

## Ejemplos comunes {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Puntuación de participación de la cuenta</strong></td> 
   <td>Profundidad de participación basada en actividades de comportamiento rastreadas en varios canales (por ejemplo, correo electrónico, web, publicidad) de personas en cuentas de destino específicas.</td>
  </tr>
  <tr>
   <td><strong>Puntuación de interés del producto de la cuenta</strong></td>
   <td>Personas de cuentas de destino que muestren interés en el contenido de un producto específico (por ejemplo, descargar un libro blanco).</td> 
  </tr>
  <tr>
   <td><strong>Puntuación de participación en la web de la cuenta</strong></td>
   <td>Personas de cuentas de destino que visitan el canal web. Se puede crear la misma puntuación para medir la participación del canal a partir de correo electrónico, publicidad u otros canales.</td> 
  </tr>
 </tbody>
</table>

## Cómo configurar la puntuación de cuenta {#how-to-configure-account-score}

>[!NOTE]
>
>Para calcular las puntuaciones de la cuenta, primero debe crear puntuaciones de posible cliente. Marketo TAM agrega automáticamente las puntuaciones de posible cliente a las puntuaciones de cuenta. Por ejemplo, tomaremos dos de los ejemplos anteriores (_Puntuación de interés del producto de la cuenta_ y _Puntuación de participación en la web de la cuenta_).
>
>En primer lugar, cree campos de puntuación de posible cliente que capten detalles relevantes de cada posible cliente de una cuenta de destino.\
>A continuación, asigne esas puntuaciones de posible cliente a sus puntuaciones de cuenta respectivas:\
>Puntuación de interés del producto de la cuenta = SUM (Puntuación de interés del producto potencial)\
>Puntuación de participación en la web de la cuenta = SUMA (Puntuación de participación en la web de los posibles clientes)

>[!NOTE]
>
>Los usuarios pueden crear varias puntuaciones de participación de cuenta y asignar distintas puntuaciones de persona a distintas puntuaciones de cuenta.

Una vez que haya configurado la puntuación de posibles clientes, siga los pasos a continuación.

1. Haga clic en **Administrador**.

   ![](assets/one-1.png)

1. Haga clic en **Administración de cuentas de Target**.

   ![](assets/account-score-2.png)

1. En Campos de puntuación, haga clic en **Editar**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Puede elegir hasta **Five** para calcular la puntuación de cuenta.

1. Introduzca el nombre de la puntuación de cuenta y haga clic en el botón **Seleccionar puntuación de persona** y seleccione la puntuación correspondiente.

   ![](assets/four.png)

1. Haga clic en **+Añadir** para agregar más puntuaciones.

   ![](assets/five.png)

1. Añada todas las puntuaciones deseadas. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/six.png)
