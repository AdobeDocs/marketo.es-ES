---
unique-page-id: 37355602
description: 'Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics Online: documentos de Marketo, documentación del producto'
title: Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 1%

---

# Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight es una herramienta fantástica para ofrecer a su equipo de ventas una &quot;ventana&quot; sobre la gran cantidad de datos que tiene el equipo de marketing. Así se instala y configura en Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

>[!NOTE]
>
>Si está usando la interfaz unificada, antes del paso 1 siguiente, haga clic en el icono Configuración en la esquina superior derecha y seleccione **Configuración avanzada**.

1. En Microsoft Dynamics CRM, haga clic en **Configuración**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. En Configuración, haga clic en **Personalizaciones**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Haga clic en **Soluciones**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado la solución de Marketo antes de continuar.

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. En la nueva ventana, haz clic en **Examinar**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. En el equipo, busque e instale la solución que acaba de descargar.

1. Haga clic en **Siguiente**.

   ![](assets/seven.png)

1. Se cargará la solución. Si lo desea, puede ver el contenido del paquete. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. No dude en descargar el archivo de registro y, a continuación, haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. ¡Fantástico! Debería ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/eleven.png)

1. Haga clic en **Personalización de Publish**.

   >[!NOTE]
   >
   >Asegúrese de habilitar la sincronización global de MS Dynamics.

## Conectar Marketo y perspectivas de ventas {#connect-marketo-and-sales-insight}

Vinculemos su instancia de Marketo al conocimiento de ventas en Dynamics. A continuación se muestra cómo:

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketo y vaya a la sección **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. En la sección Perspectiva de ventas, haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie **Marketo Host**, **API URL** y **API User Id** para usarlos en un paso posterior. Escriba una clave secreta de API de su elección y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Los campos siguientes se deben sincronizar con Marketo para que _el posible cliente y el contacto_ funcionen con la perspectiva de ventas:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Cuando vuelva a Microsoft Dynamics, vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. En **Configuración**, haga clic en **Configuración de la API de Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Escriba la información que tomó de Marketo anteriormente y haga clic en **Guardar**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Habilitar sincronización {#enable-sync}

1. En Marketo, haga clic en **Administrador**.

   ![](assets/enable-one.png)

1. En Integración, seleccione **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Haga clic en **Habilitar sincronización**.

   ![](assets/enable-three.png)

1. Haga clic en **Editar** junto a Detalles de sincronización de campos.

   ![](assets/enable-four.png)

1. Se _seleccionarán automáticamente_ los campos MSI que anteriormente estaban deshabilitados (Urgencia, Puntuación relativa y Prioridad). Simplemente haz clic en **Guardar** en para comenzar a sincronizar los datos.

   ![](assets/enable-five.png)

## Definir acceso de usuario {#set-user-access}

Por último, debe proporcionar a usuarios específicos acceso para utilizar Marketo Sales Insight.

1. Vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vaya a **Seguridad**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Seleccione a los usuarios a los que desea otorgar acceso a la Información de ventas y haga clic en **Administrar roles**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Seleccione el rol de Marketo Sales Insight y haga clic en **Aceptar**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   ¡Y tú deberías haber terminado! Por último, para realizar pruebas, inicie sesión en Dynamics como un usuario que tiene acceso a Marketo Sales Insight y observe a un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
