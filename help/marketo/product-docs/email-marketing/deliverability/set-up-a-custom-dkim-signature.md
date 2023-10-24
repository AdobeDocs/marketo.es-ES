---
unique-page-id: 2360219
description: 'Configuración de una firma DKIM personalizada: documentos de Marketo, documentación del producto'
title: Configurar una firma DKIM personalizada
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Configurar una firma DKIM personalizada {#set-up-a-custom-dkim-signature}

Para garantizar la máxima capacidad de entrega, firmamos automáticamente todo el correo saliente con una firma DKIM compartida de Marketo.

>[!NOTE]
>
>Es posible que necesite la ayuda de su equipo de TI para completar algunos de los pasos de este artículo.

Puede personalizar la firma DKIM para reflejar los dominios que elija. Así es como.

1. Vaya a la **Administrador** sección.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Si configura una firma DKIM personalizada de la forma antigua, seguirá funcionando y debería aparecer aquí.

1. Clic **Correo electrónico**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Haga clic en **SPF/DKIM** pestaña, luego **Añadir dominio**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Introduzca el dominio que utilizará en los correos electrónicos de Marketo como dirección de origen. Elija un Selector y un Tamaño de clave. Clic **Añadir** cuando termine.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* Recomendamos un tamaño de clave de 2048.
   >* Si utiliza un dominio diferente en la dirección remitente, se utilizará la firma DKIM compartida de Marketo.

   <table> 
   <tr>
   <td width="20%"><b>Selector</b></td>
   <td>Cadena o identificador único que se utiliza para localizar la parte de clave pública del registro DKIM. Puede ser una cadena arbitraria o un identificador único para separar e identificar el propósito de esa clave/registro DKIM.</td>
   </tr>
   <tr> 
   <td width="20%"><b>Tamaño de clave</b></td>
   <td>El nivel de seguridad con el que desea que se cifre su firma DKIM.</td>
   </tr>
   </tbody>
   </table>

   <p>

1. Envíe el **Registro de host** y **Valor TXT** a su equipo de TI. Pídale que cree el registro y asegúrese de que se propaga a todos los servidores de nombres asociados con el dominio de origen. La verificación DKIM de Marketo requiere que la clave DKIM se propague a todos los servidores de nombres asociados con el dominio que se está firmando con DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Una vez que confirmen que han creado el registro, vuelva a Marketo, seleccione el dominio y haga clic en **Comprobar DNS**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Si la confirmación falla y el equipo de TI ha creado el registro correctamente, puede ser una cuestión de propagación del DNS. Inténtelo de nuevo más tarde.

   >[!CAUTION]
   >
   >Modificar o eliminar el registro DNS correspondiente resultará en una capacidad de envío dañada. Asegúrese de eliminar la entrada en Marketo antes de realizar cambios en DNS.

   Esto le ayudará en absoluto con su capacidad de envío de correo electrónico. Debe obtener la validación de que el registro está allí y corregirlo.
