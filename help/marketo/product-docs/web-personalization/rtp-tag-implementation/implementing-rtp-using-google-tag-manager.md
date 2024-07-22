---
unique-page-id: 4720145
description: 'Implementación de RTP con Google Tag Manager: Documentos de Marketo: documentación del producto'
title: Implementación de RTP con Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Implementación de RTP con Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de Google Tag Manager.

1. Añada una nueva etiqueta > Configuraciones de etiqueta > Etiqueta de HTML personalizada**.** Llámelo **RTP**.

1. Inicie sesión en su cuenta de RTP**.**

1. Vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, continúe con el paso 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie la etiqueta RTP JavaScript y péguela en la nueva **etiqueta de HTML personalizada** que creó (paso 1).

1. Haga clic en **+Agregar regla para activar la etiqueta**. Seleccione **Todas las páginas**.

1. Haga clic en **Guardar** y [publicar la nueva versión](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   a. Puede hacerlo haciendo clic con el botón derecho en la página del sitio web. Vaya a **Inspect Element**, busque **RTP** para encontrar la etiqueta.
