---
unique-page-id: 4720151
description: 'Implementación de RTP en páginas de aterrizaje de Marketo: Marketo Docs: documentación del producto'
title: Implementación de RTP en páginas de aterrizaje de Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Implementación de RTP en páginas de aterrizaje de Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Vaya a la **Design Studio.** Abra el elemento que desee editar. Select **Acciones de plantilla**, seleccione **Editar borrador**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Realice los cambios de plantilla en la variable **Fuente de HTML** pestaña .

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. En su cuenta RTP, vaya a **Configuración de la cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript de Asistencia : siga con el paso 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie la etiqueta RTP JavaScript y péguela en todas las plantillas de página de aterrizaje entre las **`<head> </head>`** etiquetas.

1. Haga clic en **Guardar** y **Cerrar** la ventana .

1. Atrás en el **Design Studio**, apruebe la página de aterrizaje desde **Acciones de plantilla**, haga clic en **Aprobar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por último, tendrá que **volver a aprobar** cualquier página de aterrizaje que use esa plantilla para la plantilla cambiará para que surta efecto. Puede volver a aprobarlos todos a la vez desde la sección principal de Páginas de aterrizaje.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Para ello, haga clic con el botón derecho en la página de su sitio web. Vaya a **Ver origen de página.** Buscar **RTP** para localizar la etiqueta .
