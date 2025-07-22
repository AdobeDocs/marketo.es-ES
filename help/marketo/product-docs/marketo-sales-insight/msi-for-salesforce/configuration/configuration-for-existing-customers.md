---
unique-page-id: 42762519
description: Configuración para clientes existentes - Documentos de Marketo - Documentación del producto
title: Configuración para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 4%

---

# Configuración para clientes existentes {#configuration-for-existing-customers}

Configure la siguiente configuración para empezar a utilizar el nuevo panel de perspectivas.

>[!PREREQUISITES]
>
>Asegúrese de haber actualizado el paquete [!DNL Salesforce] a la versión más reciente

## Configurar [!DNL Sales Insight] en Marketo {#configure-sales-insight-in-marketo}

1. Abra una ficha nueva en el explorador para obtener las credenciales de [!DNL Marketo Sales Insights] de su cuenta de Marketo.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Haga clic en **[!UICONTROL Insight de ventas]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Haga clic en **[!UICONTROL Ver]** para rellenar las credenciales de la API de REST.

   ![](assets/configuration-for-existing-customers-3.png)

1. Verá una ventana emergente de confirmación. Haga clic en **[!UICONTROL Aceptar]**.

## Configurar [!DNL Sales Insight] en [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Busque y seleccione **[!UICONTROL Configuración del sitio remoto]**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Haga clic en **[!UICONTROL Nuevo sitio remoto]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Escriba el [!UICONTROL Nombre de sitio remoto] (puede ser algo como &quot;MarketoRestAPI&quot;) y la [!UICONTROL URL de sitio remoto] (su URL de API del panel Configuración de API de REST en Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/configuration-for-existing-customers-8.png)

   Ahora ha creado la configuración del sitio remoto para la API de REST.

## Acceder a Sales Insight de Marketo {#access-marketo-sales-insight}

1. Copie las credenciales del panel API de REST en la página de administración [!DNL Marketo’s Sales Insight]. Péguelos en la sección API de REST de la página de configuración de [!DNL Sales Insight] de Salesforce.

1. Escriba la [!UICONTROL clave secreta de la API].

   ![](assets/configuration-for-existing-customers-9.png)
