---
unique-page-id: 2360219
description: 'Configuración de una firma DKIM personalizada: documentos de Marketo, documentación del producto'
title: Configurar una firma DKIM personalizada
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Configurar una firma DKIM personalizada {#set-up-a-custom-dkim-signature}

Para garantizar la máxima capacidad de entrega, firmamos automáticamente todo el correo saliente con una firma DKIM compartida de Marketo.

>[!NOTE]
>
>Es posible que necesite la ayuda de su equipo de TI para completar algunos de los pasos de este artículo.

Puede personalizar la firma DKIM para reflejar los dominios que elija. Así es como.

1. Vaya a la **Administrador** sección.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >Si configura una firma DKIM personalizada de la forma antigua, seguirá funcionando y debería aparecer aquí.

1. Clic **Correo electrónico** y, a continuación, el **DKIM** y finalmente. **Añadir dominio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Introduzca el dominio que utilizará en los correos electrónicos de Marketo como dirección de origen y haga clic en **Añadir**.

   >[!TIP]
   >
   >Si utiliza un dominio diferente en la dirección remitente, utilizaremos la firma DKIM compartida de Marketo.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Envíe el **Registro de host** y **Valor TXT** a su equipo de TI. Pídale que cree el registro y asegúrese de que se propaga a todos los servidores de nombres asociados con el dominio de origen. La verificación DKIM de Marketo requiere que la clave DKIM se propague a todos los servidores de nombres asociados con el dominio que se está firmando con DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Una vez que confirmen que han creado el registro, vuelva a Marketo, seleccione el dominio y haga clic en **Comprobar DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >Si la confirmación falla y el equipo de TI ha creado el registro correctamente, puede ser una cuestión de propagación del DNS. Inténtelo de nuevo más tarde.

   >[!CAUTION]
   >
   >Modificar o eliminar el registro DNS correspondiente resultará en una capacidad de envío dañada. Asegúrese de eliminar la entrada en Marketo antes de realizar cambios en DNS.

   Esto le ayudará en absoluto con su capacidad de envío de correo electrónico. Debe obtener la validación de que el registro está allí y corregirlo.
