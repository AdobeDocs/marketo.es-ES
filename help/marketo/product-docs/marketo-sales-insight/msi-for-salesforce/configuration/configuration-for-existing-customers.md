---
unique-page-id: 42762519
description: Configuración para clientes existentes - Documentos de Marketo - Documentación del producto
title: Configuración para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Configuración para clientes existentes {#configuration-for-existing-customers}

Configure la siguiente configuración para empezar a usar el nuevo panel de información.

>[!PREREQUISITES]
>
>Asegúrese de haber actualizado el paquete de Salesforce a la última versión

## Configurar la perspectiva de ventas en Marketo {#configure-sales-insight-in-marketo}

1. Abra una nueva pestaña en el explorador para obtener las credenciales de Marketo Sales Insights de su cuenta de Marketo.

1. Vaya al área **Admin**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Haga clic en **Ver** para rellenar las credenciales de la API restante.

   ![](assets/configuration-for-existing-customers-3.png)

1. Verá una ventana emergente de confirmación. Haga clic en **OK**.

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Busque y seleccione **Configuración del sitio remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoRestAPI&quot;) y la URL del sitio remoto (la URL de su API del panel Configuración de la API de descanso en Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Haga clic en **Guardar**.

   ![](assets/configuration-for-existing-customers-8.png)

   Ahora ha creado la configuración del sitio remoto para la API de Rest.

## Acceso a la perspectiva de ventas de Marketo {#access-marketo-sales-insight}

1. Copie las credenciales del panel de la API Rest en la página de administración de la perspectiva de ventas de Marketo. Péguelos en la sección API de Rest de la página Configuración de la perspectiva de ventas de Salesforce.

1. Introduzca la clave secreta de API.

   ![](assets/configuration-for-existing-customers-9.png)
