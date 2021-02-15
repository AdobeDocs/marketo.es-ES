---
unique-page-id: 42762519
description: Configuración para clientes existentes - Documentos de marketing - Documentación del producto
title: Configuración para clientes existentes
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# Configuración para clientes existentes {#configuration-for-existing-customers}

Configure la siguiente configuración para empezar a utilizar el nuevo Panel de perspectivas.

>[!PREREQUISITES]
>
>Asegúrese de haber actualizado el paquete de Salesforce a la versión más reciente

## Configurar la perspectiva de ventas en Marketing {#configure-sales-insight-in-marketo}

1. Abra una nueva ficha en el explorador para obtener las credenciales de perspectivas de ventas de marketing de su cuenta de Marketing to.

1. Vaya al área **Administración**.

   ![](assets/configure-1.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/configure-2.png)

1. Haga clic en **Vista** para rellenar las credenciales de API de descanso.

   ![](assets/configure-3.png)

1. Verá una ventana emergente de confirmación. Haga clic en **Aceptar**.

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/sfdc-1.png)

1. Busque y seleccione **Configuración del sitio remoto**.

   ![](assets/sfdc-2.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/sfdc-3.png)

1. Escriba el nombre del sitio remoto (puede ser algo así como &quot;MarketoRestAPI&quot;) y la dirección URL del sitio remoto (su dirección URL de API desde el panel Configuración de API de Rest en Marketing).

   ![](assets/sfdc-4.png)

1. Haga clic en **Guardar**.

   ![](assets/sfdc-5.png)

   Ha creado la configuración de sitio remoto para la API de descanso.

## Acceder a la perspectiva de ventas de marketing {#access-marketo-sales-insight}

1. Copie las credenciales del panel API de Rest en la página de administración de perspectiva de ventas de Marketing Cloud. Pégalas en la sección Rest API de la página de configuración de Sales Insight de Salesforce.

1. Introduzca la clave secreta de API.

   ![](assets/config.png)
