---
unique-page-id: 4720151
description: 'Implementación de RTP en páginas de destino de Marketo: Documentos de Marketo: documentación del producto'
title: Implementación de RTP en páginas de destino de Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Implementación de RTP en páginas de destino de Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Vaya a la **Estudio de diseño.** Abra el elemento que desee editar. Seleccionar **Acciones de plantilla**, seleccione **Editar borrador**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Realice los cambios de la plantilla en **Origen del HTML** pestaña.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. En su cuenta de RTP, vaya a **Configuración de cuenta**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie la etiqueta JavaScript de RTP y péguela en todas las plantillas de página de aterrizaje entre las etiquetas **`<head> </head>`** etiquetas.

1. Clic **Guardar** y **Cerrar** la ventana.

1. De nuevo en **Design Studio**, apruebe la página de aterrizaje desde **Acciones de plantilla**, haga clic en **Aprobar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por último, debe hacer lo siguiente **volver a aprobar** cualquier página de aterrizaje que utilice esa plantilla para que los cambios en la plantilla surtan efecto. Puede volver a aprobarlos todos a la vez desde la sección principal de Páginas de aterrizaje.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   Para ello, haga clic con el botón derecho en la página del sitio web. Ir a **Ver origen de página.** Buscar por **RTP** para localizar la etiqueta.
