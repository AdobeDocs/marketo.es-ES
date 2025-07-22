---
unique-page-id: 4720151
description: 'Implementación de RTP en páginas de destino de Marketo: Documentos de Marketo: documentación del producto'
title: Implementación de RTP en páginas de destino de Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementación de RTP en páginas de destino de Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar su [!UICONTROL etiqueta RTP], siga las instrucciones de instalación a continuación:

1. Vaya a **[!UICONTROL Design Studio].** Abra el elemento que desee editar. Seleccione **[!UICONTROL Acciones de plantilla]**, seleccione **[!UICONTROL Editar borrador]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Realice los cambios de plantilla en la ficha **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. En su cuenta RTP, vaya a **[!UICONTROL Configuración de la cuenta]**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. En [!UICONTROL Dominio], busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie la etiqueta RTP JavaScript y péguela en todas las plantillas de página de aterrizaje entre las etiquetas **`<head> </head>`**.

1. Haz clic en **[!UICONTROL Guardar]** y **[!UICONTROL Cerrar]** la ventana.

1. De nuevo en **[!UICONTROL Design Studio]**, apruebe la página de aterrizaje de **[!UICONTROL Acciones de plantilla]**, haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por último, tendrá que **volver a aprobar** cualquier página de aterrizaje que use esa plantilla para que los cambios en la plantilla surtan efecto. Puede volver a aprobarlas todas a la vez desde la sección principal [!UICONTROL Páginas de aterrizaje].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Para ello, haga clic con el botón derecho en la página del sitio web. Vaya a **[!UICONTROL Ver página Source].** busque **[!UICONTROL RTP]** para encontrar la etiqueta.
