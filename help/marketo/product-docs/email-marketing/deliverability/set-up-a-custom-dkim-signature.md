---
unique-page-id: 2360219
description: Configurar una firma de DKIM personalizada - Documentos de Marketo - Documentación del producto
title: Configurar una firma personalizada de DKIM
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# Configurar una firma personalizada de DKIM {#set-up-a-custom-dkim-signature}

Para garantizar una entrega de primer nivel, firmamos automáticamente todo el correo saliente con una firma compartida de Marketo DKIM.

>[!NOTE]
>
>Es posible que necesite la ayuda de su equipo de TI para completar algunos de los pasos de este artículo.

Puede personalizar la firma de DKIM para que refleje los dominios que elija. Así es como.

1. Vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Si configura una firma de DKIM personalizada de la forma antigua, seguirá funcionando y debería aparecer aquí.

1. Haga clic en **Correo electrónico**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Haga clic en la ficha **SPF/DKIM** y luego en **Agregar dominio**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Introduzca el dominio que utilizará en los correos electrónicos de Marketo como dirección de origen. Elija un Selector y un Tamaño de clave. Haga clic en **Agregar** cuando haya terminado.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>Selector</b></td>
   <td>Cadena o identificador único que se utiliza para localizar la parte de clave pública del registro de DKIM. Puede ser una cadena arbitraria o un identificador único para separar e identificar el propósito de esa clave/registro de DKIM.</td>
   </tr>
   <tr>
   <td width="20%"><b>Tamaño de clave</b></td>
   <td>El nivel de seguridad con el que desea que se cifre la firma de DKIM.</td>
   </tr>
   </tbody>
   </table>

   <p>

   >[!TIP]
   >
   >* Recomendamos un tamaño de clave de 2048.
   >* Si utiliza un dominio diferente en la dirección remitente, se utilizará la firma de DKIM compartida de Marketo.

   >[!IMPORTANT]
   >
   >Si necesita actualizar el Selector de DKIM o el Tamaño de cifrado de DKIM para su dominio, debe eliminar el registro existente y volver a publicar el registro recién generado con los nuevos valores.
   >
   >Tenga en cuenta que, al hacerlo, DKIM no se firmará para su dominio hasta que nuestro sistema publique y valide su nuevo registro. Planifique el cambio en consecuencia, ya que pueden pasar de 24 a 48 horas antes de que el nuevo registro de DKIM se propague completamente por Internet.

1. Envíe el **[!UICONTROL registro de host]** y el **[!UICONTROL valor TXT]** a su equipo de TI. Pídale que cree el registro y asegúrese de que se propaga a todos los servidores de nombres asociados con el dominio de origen. La verificación DKIM de Marketo requiere que la clave de DKIM se propague a todos los servidores de nombres asociados con el dominio que se firma con DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Una vez que confirmen que han creado el registro, vuelva a Marketo, seleccione su dominio y haga clic en **[!UICONTROL Comprobar DNS]**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Si la confirmación falla y el equipo de TI ha creado el registro correctamente, puede ser una cuestión de propagación del DNS. Inténtelo de nuevo más tarde.

   >[!CAUTION]
   >
   >Modificar o eliminar el registro DNS correspondiente resultará en una capacidad de envío dañada. Asegúrese de eliminar la entrada en Marketo antes de realizar cambios en DNS.

   Esto le ayudará en absoluto con su capacidad de envío de correo electrónico. Debe obtener la validación de que el registro está allí y corregirlo.
