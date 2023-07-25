---
unique-page-id: 3571735
description: 'Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2011: documentos de Marketo, documentación del producto'
title: Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight es una herramienta fantástica para su equipo de ventas. Esta es una instrucción paso a paso de cómo instalarla y configurarla en las instalaciones locales de Microsoft Dynamics 2011.

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

1. Inicie sesión en Microsoft Dynamics CRM. Clic **Configuración** en el menú inferior izquierdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccionar **Soluciones** en el árbol.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Clic **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Ya debería haberlo hecho [instalado y configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solución Marketo antes de continuar.

1. Clic **Examinar**. Seleccione la solución Marketo Sales Insight que desee [descargado](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Clic **Siguiente**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Compruebe los detalles de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Asegúrese de que la opción de mensaje del SDK esté seleccionada. Clic **Siguiente**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ahora espere a que finalice la importación.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Haga clic en **Cerrar**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight aparecerá ahora en la lista de soluciones. ¡Yay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Seleccione Marketo Sales Insight y haga clic en **Publicar todas las personalizaciones** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Conectar Marketo y perspectivas de ventas  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Inicie sesión en Marketo y haga clic en **Administrador**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En el **Perspectiva de ventas** clic en sección **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **Host de Marketo**, **URL de API**, y **ID de usuario de API** para su uso en un paso posterior. Introduzca una **Clave secreta de API** y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Los siguientes campos deben sincronizarse con Marketo para _Posible cliente y contacto_ para que funcione la perspectiva de ventas:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice lo siguiente [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Vuelva a Dynamics y seleccione **Configuración**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccionar **Configuración de API de Marketo** en el árbol.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Clic **Configuración predeterminada**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Escriba la información que tomó de Marketo anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Clic **Guardar**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Definir acceso de usuario {#set-user-access}

Configure las funciones de usuario para que determinados usuarios tengan acceso a la Información sobre ventas.

1. Seleccionar **Configuración**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Seleccionar **Administration** en el árbol.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Clic **Usuarios**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Seleccione los usuarios a los que desea conceder acceso y haga clic en **Administrar funciones**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Seleccione el **Perspectiva de ventas de Marketo** función y clic **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   ¡Y eso es todo! Todos los usuarios que tengan acceso ahora podrán ver la sección de perspectiva de ventas en la vista de detalles del posible cliente/contacto.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Enhorabuena. Ahora ha desatado el poder de Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Configuración de Estrellas y Llamas para Registros de Plomo/Contacto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
