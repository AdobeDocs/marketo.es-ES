---
unique-page-id: 4720151
description: Implementación de RTP en Páginas de aterrizaje de marketing - Documentos de marketing - Documentación del producto
title: Implementación de RTP en Páginas de aterrizaje de marketing
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Implementación de RTP en Páginas de aterrizaje de marketing {#implementing-rtp-on-marketo-landing-pages}

Para implementar la etiqueta RTP, siga las instrucciones de instalación a continuación:

1. Vaya a **Design Studio.** Abra el elemento que desee editar. Seleccionar acciones **** de plantilla, seleccione **Editar borrador**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Realice los cambios de plantilla en la ficha Origen **** HTML.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. En su cuenta RTP, vaya a Configuración de cuenta**.**

1. Si ya ha recibido la etiqueta JavaScript de la asistencia técnica, continúe con el paso 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. En Dominio, busque el dominio relevante y haga clic en **Generar etiqueta**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie la etiqueta RTP JavaScript y péguela en todas las plantillas de página de aterrizaje entre las **`<head> </head>`** etiquetas.
1. Haga clic en **Guardar** y **Cerrar** la ventana.
1. De nuevo en **Design Studio**, apruebe la página de aterrizaje desde Acciones **de** plantilla y haga clic en **Aprobar**.\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por último, deberá **volver a aprobar** cualquier página de aterrizaje que utilice esa plantilla para que los cambios de plantilla surtan efecto. Puede volver a aprobarlos todos a la vez desde la sección de Páginas de aterrizaje principales.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Compruebe que aparece en todas las `pages including` páginas de aterrizaje y subdominios.

   Para ello, haga clic con el botón derecho en la `website’s` página. Vaya a Origen de página de **Vista.** Busque **RTP** para localizar la etiqueta.
