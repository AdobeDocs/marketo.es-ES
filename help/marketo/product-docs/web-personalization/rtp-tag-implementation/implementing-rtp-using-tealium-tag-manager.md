---
unique-page-id: 9437340
description: Implementación de RTP mediante el Administrador de etiquetas de torio - Documentos de marketing - Documentación del producto
title: Implementación de RTP mediante el Administrador de etiquetas de torio
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implementación de RTP mediante el Administrador de etiquetas de torio {#implementing-rtp-using-tealium-tag-manager}

Para implementar la etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta del Administrador de etiquetas de torio.
1. Vaya a la ficha Etiquetas y agregue la etiqueta de Contenedor personalizado de torio, ubicada en la ficha Misc del mercado de etiquetas.
1. En el campo Título, introduzca **Marketo RTP** y haga clic en **Finalizar**.
1. Guarde los cambios.

   >[!NOTE]
   >
   >Todavía no hay necesidad de publicar el nuevo contenedor.

1. Una vez guardado el perfil, haga clic en su nombre o dirección de correo electrónico en la esquina superior derecha de la consola de iQ de Tealium.
1. En el menú Administración, haga clic en **Administrar plantillas** en Administración de cuentas.
1. Seleccionar Contenedor personalizado **de torio: Marque RTP** desde la lista desplegable para abrir la plantilla Tag.
1. Inicie sesión en su cuenta RTP.
1. Vaya a Configuración de cuenta.

   >[!NOTE]
   >
   >Si ya ha recibido la etiqueta JavaScript de la asistencia técnica, continúe con el paso 11.

1. En Dominio, busque el dominio relevante y haga clic en **Generar etiqueta**.
1. Copie la etiqueta de JavaScript de RTP y péguela entre el código de la biblioteca de etiquetas de Inicio y el código de la biblioteca de etiquetas final en la plantilla de Perfil de torio.

   >[!NOTE]
   >
   >**Pasos importantes**
   >
   >Elimine las etiquetas `<!-- RTP tag -->` y `<!-- End of RTP tag -->` del código que coloque en este archivo.
   >
   >Elimine las etiquetas `<script type='text/javascript'>` y `</script>` del código que coloque en este archivo.

1. **Haga clic en Guardar plantilla** de Perfil y publique el nuevo perfil.

