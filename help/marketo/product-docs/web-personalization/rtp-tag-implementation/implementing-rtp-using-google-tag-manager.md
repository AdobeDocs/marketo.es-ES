---
unique-page-id: 4720145
description: Implementación de RTP mediante Google Tag Manager - Marketo Docs - Documentación del producto
title: Implementación de RTP mediante Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Implementación de RTP mediante Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de Administrador de etiquetas de Google.

1. Agregue una etiqueta > Configuraciones de etiquetas > Etiqueta de HTML personalizada**.** Llámelo **RTP**.

1. Inicie sesión en su cuenta RTP**.**

1. Vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript de Asistencia, continúe con el paso 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie la etiqueta RTP JavaScript y péguela en la nueva **Etiqueta HTML personalizada** ha creado (paso 1).

1. Haga clic en **+Añadir regla a la etiqueta de activación**. Select **Todas las páginas**.

1. Haga clic en **Guardar** y [publicar la nueva versión](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   a. Para ello, haga clic con el botón derecho en la página de su sitio web. Vaya a **Elemento Inspect**, Buscar **RTP** para localizar la etiqueta .
