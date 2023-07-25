---
unique-page-id: 4720215
description: Implementación de RTP en Wordpress Enterprise - Documentos de Marketo - Documentación del producto
title: Implementación de RTP en Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementación de RTP en Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Ir a **Configuración de cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie la etiqueta JavaScript de RTP.

1. Inicie sesión en su cuenta de WordPress como usuario administrador

   a. En **Aspecto**, vaya a **JavaScript personalizado**.
b. Pegue la etiqueta Javascript RTP justo después del código existente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Cuando pegue el código, EXCLUYA las siguientes etiquetas:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Inserte la secuencia de comandos SOLAMENTE.

1. Clic **Actualizar**.
