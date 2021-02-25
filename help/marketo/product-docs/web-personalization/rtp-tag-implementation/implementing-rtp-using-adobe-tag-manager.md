---
unique-page-id: 4720218
description: 'Implementación de RTP mediante Adobe Tag Manager: documentos de marketing: documentación del producto'
title: Implementación de RTP mediante Adobe Tag Manager
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Implementación de RTP mediante Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar la etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Inicie sesión en su cuenta RTP.

1. Vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript de la asistencia técnica, continúe con el paso 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. En Dominio, localice el dominio relevante y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Inicie sesión en su cuenta del Administrador dinámico de etiquetas ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Vaya a **Panel.** Haga clic en la propiedad web correspondiente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vaya a **Reglas**, haga clic en **Crear nueva regla**.

1. Complete lo siguiente

   1. Nombre: **RTP de marketing**
   1. Condiciones (contraer): Regla de déclencheur en - **Principio de la página**
   1. Javascript (contraer): haga clic en **Añadir nueva secuencia de comandos**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Llame a la nueva etiqueta: **Etiqueta RTP de marketing**

1. Elimine el siguiente código de la etiqueta RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Pegue la etiqueta RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Asegúrese de eliminar todas las etiquetas y dejar solo la propia secuencia de comandos (no `<script type='text/javascript'>` , `</script>` )

1. Haga clic en **Guardar código** en el editor de secuencias de comandos y **Guardar regla** en el editor de reglas.

1. En el panel Reglas, ubique la regla de carga de página RTP de marketing y, en la lista desplegable **Acciones**, seleccione **Activar reglas**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **** Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Puede hacerlo haciendo clic con el botón derecho en las páginas del sitio web. Vaya a **Elemento de Inspect**, haga clic en **Red**, Buscar: **RTP**.
