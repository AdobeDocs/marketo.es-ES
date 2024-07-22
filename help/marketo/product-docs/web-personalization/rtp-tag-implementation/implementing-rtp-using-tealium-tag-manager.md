---
unique-page-id: 9437340
description: 'Implementación de RTP con Tealium Tag Manager: Documentos de Marketo, documentación del producto'
title: Implementación de RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Implementación de RTP con Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de Tealium Tag Manager.

1. Vaya a la pestaña Etiquetas y añada la etiqueta de contenedor personalizada Tealium, ubicada en la pestaña Varios del mercado de etiquetas.

1. En el campo Título, escriba **Marketo RTP** y haga clic en **Finalizar**.

1. Guarde los cambios.

   >[!NOTE]
   >
   >Aún no es necesario publicar el nuevo contenedor.

1. Una vez guardado el perfil, haga clic en su nombre/dirección de correo electrónico en la esquina superior derecha de la consola de Tealium iQ.

1. En el menú Administración, haga clic en **Administrar plantillas** en Administración de cuentas.

1. Seleccione **Contenedor personalizado Tealium: Marketo RTP** de la lista desplegable para abrir la plantilla de etiqueta.

1. Inicie sesión en su cuenta de RTP.

1. Vaya a Configuración de la cuenta.

   >[!NOTE]
   >
   >Si ya ha recibido su etiqueta JavaScript del equipo de asistencia, continúe con el paso 11.

1. En Dominio, busque el dominio correspondiente y haga clic en **Generar etiqueta**.

1. Copie la etiqueta RTP JavaScript y péguela entre Start Tag Library Code y End Tag Library Code en la plantilla de perfil de Tealium.

   >[!NOTE]
   >
   >**Pasos importantes**
   >
   >Quite las etiquetas `<!-- RTP tag -->` y `<!-- End of RTP tag -->` del código que coloque en este archivo.
   >
   >Elimine las etiquetas `<script type='text/javascript'>` y `</script>` del código que coloque en este archivo.

1. **Haga clic en Guardar plantilla de perfil** y publique su nuevo perfil.
