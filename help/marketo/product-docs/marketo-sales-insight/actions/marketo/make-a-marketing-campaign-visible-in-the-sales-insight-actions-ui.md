---
description: Hacer visible una campaña de marketing en la interfaz de usuario de acciones de Sales Insight, documentos de Marketo, documentación del producto
title: Hacer visible una campaña de marketing en la interfaz de usuario de acciones de Sales Insight
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: b037057cb37c830760a5d5bc24591f85ad306ae8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Hacer visible una campaña de marketing en la interfaz de usuario de acciones de Sales Insight {#make-a-marketing-campaign-visible-in-the-sales-insight-actions-ui}

Las campañas solo se pueden compartir si se hacen visibles.

Con las acciones de información de ventas, los usuarios tendrán acceso a una nueva aplicación de ventas llamada toutapp.com. Esta aplicación les ofrece un nuevo conjunto de funcionalidades de acción, pero también hereda la función _Añadir a la campaña de marketing_ disponible en la versión principal de Información sobre ventas. Esto es importante tenerlo en cuenta, ya que según dónde desee que los usuarios accedan a la función Añadir a la campaña de marketing (toutapp.com o la experiencia del paquete MSI SFDC), las campañas de Marketo deberán configurarse de forma diferente. Consulte la nota del paso 4 para obtener más información.

1. Seleccione (o cree) la campaña que desee compartir.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Haga clic en la ficha **Lista inteligente**.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Añada el déclencheur La campaña es solicitada.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Para el origen, elija &quot;es&quot; **API de servicio web**.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Si desea mostrar la campaña de marketing a los usuarios que están utilizando _Agregar a la campaña de marketing_ desde la aplicación web toutapp.com (esto también incluye si tiene la aplicación web incrustada en el CRM mediante el objeto de bandeja de salida de ventas de Marketo), establézcala en &quot;API de servicio web&quot;. Si desea que la campaña de marketing se muestre cuando un usuario utilice las acciones del panel MSI de Salesforce en los botones de posible cliente, contacto, página de cuenta o acción masiva de las vistas de lista de contactos y posibles clientes, actualícela a &quot;Perspectiva de ventas&quot;

1. Haga clic en la ficha **Flujo**.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Añada la acción de flujo Momento interesante.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Para Tipo, seleccione **Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. En el cuadro Descripción, escriba un mensaje al equipo de ventas. En este ejemplo utilizamos tokens para especificar el formulario que se rellenó.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Haga clic en la ficha **Programar** y **Activar** la campaña.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
