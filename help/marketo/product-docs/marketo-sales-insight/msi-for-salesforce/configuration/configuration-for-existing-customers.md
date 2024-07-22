---
unique-page-id: 42762519
description: Configuración para clientes existentes - Documentos de Marketo - Documentación del producto
title: Configuración para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Configuración para clientes existentes {#configuration-for-existing-customers}

Configure la siguiente configuración para empezar a utilizar el nuevo panel de perspectivas.

>[!PREREQUISITES]
>
>Asegúrese de haber actualizado el paquete de Salesforce a la versión más reciente

## Configuración de Sales Insight en Marketo {#configure-sales-insight-in-marketo}

1. Abra una nueva pestaña en el navegador para obtener las credenciales de Marketo Sales Insights de su cuenta de Marketo.

1. Vaya al área de **Admin**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Haga clic en **Información de ventas**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Haga clic en **Ver** para rellenar las credenciales de la API de REST.

   ![](assets/configuration-for-existing-customers-3.png)

1. Verá una ventana emergente de confirmación. Haga clic en **Aceptar**.

## Configuración de Sales Insight en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Busque y seleccione **Configuración del sitio remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoRestAPI&quot;) y la URL del sitio remoto (su URL de API desde el panel Configuración de la API de REST en Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Haga clic en **Guardar**.

   ![](assets/configuration-for-existing-customers-8.png)

   Ahora ha creado la configuración del sitio remoto para la API de REST.

## Acceder a Sales Insight de Marketo {#access-marketo-sales-insight}

1. Copie las credenciales del panel de API de REST en la página de administración de Sales Insight de Marketo. Péguelos en la sección API de REST de la página Configuración de Sales Insight de Salesforce.

1. Introduzca la clave secreta de la API.

   ![](assets/configuration-for-existing-customers-9.png)
