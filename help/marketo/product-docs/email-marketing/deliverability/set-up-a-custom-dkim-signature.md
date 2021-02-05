---
unique-page-id: 2360219
description: Configuración de una firma DKIM personalizada - Documentos de marketing - Documentación del producto
title: Configuración de una firma DKIM personalizada
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Configure una firma DKIM personalizada {#set-up-a-custom-dkim-signature}

Con el fin de garantizar la entrega de primera calidad, firmamos automáticamente todos los correos salientes con una firma compartida de Marketing a DKIM.

>[!NOTE]
>
>Es posible que necesite la ayuda de su equipo de TI para completar algunos de los pasos de este artículo.

Puede personalizar la firma DKIM para que refleje los dominios de su elección. Así es como.

1. Vaya a la sección **Administración**.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >Si configuras una firma DKIM personalizada de la manera antigua, seguirá funcionando y debería aparecer aquí.

1. Haga clic en **Correo electrónico**, luego en la ficha **DKIM** y, finalmente, **Añadir dominio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Escriba el dominio que va a usar en los correos electrónicos de Marketing como Dirección de origen y haga clic en **Añadir**.

   >[!TIP]
   >
   >Si usa un dominio diferente en su dirección de origen, usaremos la firma DKIM compartida de Marketing Cloud.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Envíe el **Registro de host** y **Valor TXT** a su TI. Pídale que cree el registro por usted y asegúrese de que se propaga a todos los servidores de nombres asociados con el dominio de origen. La verificación DKIM de Marketing requiere que la clave DKIM se propague a todos los servidores de nombres asociados con el dominio que se firma DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Una vez que confirmen que han creado el registro, vuelva a Marketing, seleccione su dominio y haga clic en **Comprobar DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >Si la confirmación falla y el departamento de TI ha creado el registro correctamente, puede que se trate de una propagación de DNS. Inténtelo de nuevo más tarde.

   >[!CAUTION]
   >
   >Si se modifica o elimina el registro DNS correspondiente, se dañará la capacidad de entrega. Asegúrese de eliminar la entrada en Marketing antes de realizar cambios en DNS.

   Esto le ayudará en absoluto con la entrega de su correo electrónico. Debe obtener la validación de que el registro está ahí y es correcto.
