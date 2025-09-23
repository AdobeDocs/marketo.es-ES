---
unique-page-id: 11380774
description: Puntuación de la cuenta - Documentos de Marketo - Documentación del producto
title: Calificación de la cuenta
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 1%

---

# [!UICONTROL Puntuación de la cuenta] {#account-score}

La puntuación de cuentas es una parte vital de [!UICONTROL Administración de cuentas de Target]. Le ayuda a determinar el nivel de participación de sus cuentas.

## ¿Qué es la puntuación de cuenta? {#what-is-account-scoring}

Se trata de un enfoque sistemático diseñado para ayudar a los equipos de ventas y marketing a identificar y priorizar las empresas (incluidos los posibles clientes) que tienen más probabilidades de realizar una compra.

En el complejo mundo de los procesos de compra B2B, es raro que un solo individuo tome una decisión de compra. A menudo hay varios roles involucrados, cada uno con sus propias necesidades. La puntuación basada en cuentas tiene esto en cuenta al agregar las puntuaciones de posibles clientes de varios posibles clientes y proporcionar una puntuación a nivel de cuenta.

## Ejemplos comunes {#common-examples}

<table>
 <tbody>
  <tr>
   <td><strong>Puntuación de participación de cuenta</strong></td>
   <td>Profundidad de participación basada en actividades de comportamiento rastreadas en varios canales (por ejemplo, correo electrónico, web y publicidad) de personas en cuentas de destinatario específicas.</td>
  </tr>
  <tr>
   <td><strong>Puntuación de interés del producto de cuenta</strong></td>
   <td>Personas de cuentas de Target que muestran interés en el contenido de un producto específico (por ejemplo, descargar un documento técnico).</td>
  </tr>
  <tr>
   <td><strong>Puntuación de participación web de cuenta</strong></td>
   <td>Usuarios de cuentas de Target que visitan el canal Web. Se puede crear la misma puntuación para medir la participación del canal desde el correo electrónico, la publicidad u otros canales.</td>
  </tr>
 </tbody>
</table>

## Cómo configurar la puntuación de la cuenta {#how-to-configure-account-score}

>[!NOTE]
>
>Para calcular las puntuaciones de la cuenta, primero debe crear puntuaciones de posibles clientes. Marketo TAM agrega automáticamente puntuaciones de posibles clientes a puntuaciones de cuenta. A modo de ejemplo, tomaremos dos de los ejemplos anteriores (_Puntuación de interés de producto de cuenta_ y _Puntuación de participación en la web de cuenta_).
>
>En primer lugar, cree campos de puntuación de posibles clientes que recopilen detalles relevantes de cada posible cliente de una cuenta de destino.
>>A continuación, asigne esas puntuaciones de posibles clientes a sus respectivas puntuaciones de cuenta:
>>Puntuación de interés de producto de cuenta = SUM (puntuación de interés de producto de cliente potencial)
>>Puntuación de participación en la web de la cuenta = SUM (Puntuación de participación en la web del posible cliente)

>[!NOTE]
>
>Los usuarios pueden crear varias puntuaciones de participación de la cuenta y asignar distintas puntuaciones de persona a distintas puntuaciones de cuenta.

Una vez que haya configurado la puntuación del posible cliente, siga los pasos a continuación.

1. Haga clic en **[!UICONTROL Administrador]**.

   ![](assets/account-score-1.png)

1. Haga clic en **[!UICONTROL Administración de cuenta de Target]**.

   ![](assets/account-score-2.png)

1. En [!UICONTROL Campos de puntuación], haga clic en **[!UICONTROL Editar]**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Puede elegir hasta **cinco** campos para calcular la [!UICONTROL puntuación de la cuenta].

1. Escriba el nombre [!UICONTROL Puntuación de cuenta], haga clic en el menú desplegable **[!UICONTROL Seleccionar puntuación de persona]** y seleccione la puntuación correspondiente.

   ![](assets/account-score-4.png)

1. Haga clic en **[!UICONTROL +Agregar]** para agregar más puntuaciones.

   ![](assets/account-score-5.png)

1. Añada todas las puntuaciones deseadas. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/account-score-6.png)
