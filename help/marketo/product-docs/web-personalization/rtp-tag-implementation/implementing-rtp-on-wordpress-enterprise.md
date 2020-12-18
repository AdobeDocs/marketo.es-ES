---
unique-page-id: 4720215
description: Implementación de RTP en Wordpress Enterprise - Documentos de marketing - Documentación del producto
title: Implementación de RTP en Wordpress Enterprise
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Implementación de RTP en Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar la etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Vaya a Configuración de cuenta**.**

   1. Si ya ha recibido la etiqueta JavaScript de la asistencia técnica, continúe con el paso 3.\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. En Dominio, localice el dominio relevante y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie la etiqueta RTP JavaScript.
1. Inicie sesión en su cuenta de WordPress como usuario administrador

   1. En **Aspecto**, vaya a **JavaScript personalizado**.
   1. Pegue la etiqueta RTP Javascript justo después del código existente.

      ![](assets/image2014-12-3-17-3a51-3a46.png)
   >[!CAUTION]
   >
   >Al pegar el código EXCLUIR las etiquetas siguientes:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >    
   >Inserte la propia secuencia de comandos SOLAMENTE.

1. Haga clic en **Actualizar**.
