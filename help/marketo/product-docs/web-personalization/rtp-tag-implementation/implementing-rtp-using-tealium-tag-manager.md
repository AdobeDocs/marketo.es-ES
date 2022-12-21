---
unique-page-id: 9437340
description: Implementación de RTP mediante el Administrador de etiquetas de torio - Marketo Docs - Documentación del producto
title: Implementación de RTP mediante el Administrador de etiquetas de Tealium
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Implementación de RTP mediante el Administrador de etiquetas de Tealium {#implementing-rtp-using-tealium-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de Tealium Tag Manager.

1. Vaya a la pestaña Etiquetas y añada la etiqueta Contenedor personalizado de torio, ubicada en la pestaña Misc del mercado Etiquetas.

1. En el campo Título , introduzca **Marketo RTP** y haga clic en **Finalizar**.

1. Guarde los cambios.

   >[!NOTE]
   >
   >Aún no es necesario publicar el nuevo contenedor.

1. Una vez guardado el perfil, haga clic en su nombre/dirección de correo electrónico en la esquina superior derecha de la consola de Tealium iQ.

1. En el menú Administración, haga clic en **Administrar plantillas** en Administración de cuentas.

1. Select **Contenedor personalizado de tealium: Marketo RTP** en la lista desplegable para abrir la plantilla Etiqueta .

1. Inicie sesión en su cuenta RTP.

1. Vaya a Configuración de la cuenta.

   >[!NOTE]
   >
   >Si ya ha recibido la etiqueta JavaScript de Asistencia, continúe con el paso 11.

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

1. Copie la etiqueta JavaScript de RTP y péguela entre Iniciar código de biblioteca de etiquetas y Finalizar código de biblioteca de etiquetas en la plantilla de perfil de torio.

   >[!NOTE]
   >
   >**Pasos importantes**
   >
   >Elimine el `<!-- RTP tag -->` y `<!-- End of RTP tag -->` etiquetas del código que coloque en este archivo.
   >
   >Eliminar cualquier `<script type='text/javascript'>` y `</script>` etiquetas del código que coloque en este archivo.

1. **Haga clic en Guardar plantilla de perfil .** y publicar el nuevo perfil.
