---
unique-page-id: 4720218
description: Implementación de RTP mediante Adobe Tag Manager - Marketo Docs - Documentación del producto
title: Implementación de RTP mediante Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementación de RTP mediante Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Inicie sesión en su cuenta RTP.

1. Vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript de Asistencia : siga con el paso 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Inicie sesión en su cuenta de Administrador dinámico de etiquetas ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Vaya a **Tablero.** Haga clic en la propiedad web correspondiente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vaya a **Reglas**, haga clic en **Crear nueva regla**.

1. Complete lo siguiente

   1. Nombre: **Marketo RTP**
   1. Condiciones (contraer) : regla de déclencheur en - **Principio de la página**
   1. Javascript (contraer): click **Agregar nuevo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Llame a la nueva etiqueta : **Etiqueta RTP de Marketo**

1. Elimine el siguiente código de la etiqueta RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Pegue la etiqueta RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Asegúrese de eliminar todas las etiquetas y dejar solo el propio script (no `<script type='text/javascript'>` , `</script>` )

1. Haga clic en **Guardar código** en el editor de secuencias de comandos y **Guardar regla** en el editor de reglas.

1. En el panel Reglas , ubique la regla de carga de página RTP de Marketo y dentro del **Acciones** selección desplegable **Activar reglas**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificar** que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Puede hacerlo haciendo clic con el botón derecho en las páginas de su sitio web. Vaya a **Elemento Inspect**, haga clic en **Red**, Buscar: **RTP**.
