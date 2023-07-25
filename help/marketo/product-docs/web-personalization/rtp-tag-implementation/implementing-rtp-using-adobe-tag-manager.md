---
unique-page-id: 4720218
description: Implementación de RTP con Adobe Tag Manager - Documentos de Marketo - Documentación del producto
title: Implementación de RTP con Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementación de RTP con Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Inicie sesión en su cuenta de RTP.

1. Ir a **Configuración de cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Inicie sesión en su cuenta de Dynamic Tag Manager ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Ir a **Tablero.** Haga clic en la propiedad web correspondiente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Ir a **Reglas**, haga clic en **Crear nueva regla**.

1. Complete lo siguiente

   1. Nombre: **MARKETO RTP**
   1. Condiciones (contraer) : regla de Déclencheur en - **Parte superior de la página**
   1. Javascript (contraer): clic **Agregar nuevo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Llame a la nueva etiqueta: **Etiqueta RTP de Marketo**

1. Elimine el siguiente código de la etiqueta RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Pegue la etiqueta JavaScript de RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Asegúrese de eliminar todas las etiquetas y dejar solo la secuencia de comandos en sí (no `<script type='text/javascript'>` , `</script>` )

1. Clic **Guardar código** en el editor de scripts y **Guardar regla** en el editor de reglas.

1. En el panel Reglas, localice la regla de carga de página RTP de Marketo y dentro de la variable **Acciones** selección desplegable **Activar reglas**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificar** que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Puede hacerlo haciendo clic con el botón derecho en las páginas del sitio web. Ir a **Elemento Inspect**, haga clic en **Red**, Buscar: **RTP**.
