---
unique-page-id: 4720215
description: Implementación de RTP en Wordpress Enterprise - Marketo Docs - Documentación del producto
title: Implementación de RTP en Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementación de RTP en Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript de Asistencia : siga con el paso 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie la etiqueta RTP JavaScript .

1. Inicie sesión en su cuenta de WordPress como usuario administrador

   a. En **Aspecto**, vaya a **JavaScript personalizado**.
b. Pegue la etiqueta Javascript de RTP justo después del código existente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Cuando pegue el código EXCLUIR las siguientes etiquetas:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >Inserte el script en sí SOLO.

1. Haga clic en **Actualizar**.
