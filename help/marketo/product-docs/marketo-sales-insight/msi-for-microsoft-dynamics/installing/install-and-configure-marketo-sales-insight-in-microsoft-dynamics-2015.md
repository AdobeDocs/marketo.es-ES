---
unique-page-id: 7513865
description: Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2015 - Marketo Docs - Documentación del producto
title: Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2015
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight es una herramienta fantástica para ofrecer a su equipo de ventas una &quot;ventana&quot; de la riqueza de datos que posee el equipo de marketing. A continuación se explica cómo instalarlo y configurarlo en Microsoft Dynamics 201

>[!PREREQUISITES]
>
>Complete la integración Marketo-Microsoft.
>
>[Descargar la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

Bien, ahora es el momento de importar la solución de perspectiva de ventas de Marketo en Microsoft Dynamics. A continuación se muestra cómo:

1. En Microsoft Dynamics CRM, haga clic en **Configuración**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. En CONFIGURACIÓN, haga clic en **Personalizaciones**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Haga clic en **Soluciones**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado la solución Marketo antes de seguir adelante.

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. En la nueva ventana, haga clic en **Examinar**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Busque y seleccione la solución que descargó anteriormente.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Se cargará la solución. Puede ver el contenido del paquete si lo desea. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Siéntase libre de descargar el archivo de registro y luego haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. ¡Increíble! Debería ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Conectar Marketo y perspectivas de ventas {#connect-marketo-and-sales-insight}

Vincule su instancia de Marketo con la perspectiva de ventas en Dynamics. A continuación se muestra cómo:

>[!NOTE]
>
>Se requieren derechos de administrador.

1. Inicie sesión en Marketo y vaya a la **Administrador** para obtener más información.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección Perspectiva de ventas , haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **Host de Marketo**, **URL de API** y **ID de usuario de API** para su uso en un paso posterior. Introduzca una clave secreta de API de su elección y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No use un signo &amp; en la clave secreta de API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Los campos siguientes deben sincronizarse con Marketo para *posible cliente y contacto* para que funcione Sales Insight:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo

   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para corregir esto, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De vuelta a Microsoft Dynamics, vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. En **Configuración**, haga clic en **Configuración de la API de Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Introduzca la información que tomó de Marketo anteriormente y haga clic en **Guardar**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Establecer acceso de usuario {#set-user-access}

Por último, debe dar acceso a usuarios específicos para que utilicen la perspectiva de ventas de Marketo.

1. Vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Vaya a **Seguridad**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Seleccione a los usuarios a los que desea conceder acceso a la perspectiva de ventas y haga clic en **Administrar funciones**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Seleccione la función Perspectiva de ventas de Marketo y haga clic en **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   ¡Y todos deberían haber terminado! Finalmente, para probar, inicie sesión en Dynamics como usuario que tiene acceso a Marketo Sales Insight y observe un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ahora ha desbloqueado la potencia de Marketo Sales Insight para su equipo de ventas.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de posible cliente/contacto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
