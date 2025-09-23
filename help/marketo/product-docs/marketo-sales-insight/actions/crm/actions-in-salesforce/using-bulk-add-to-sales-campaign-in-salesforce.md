---
description: Uso de la campaña de adición masiva a ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Uso de la adición masiva a la campaña de ventas en Salesforce
exl-id: e518fe82-e37d-4edd-8a31-19268f6fd4b1
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# Uso de la adición masiva a la campaña de ventas en Salesforce {#using-bulk-add-to-sales-campaign-in-salesforce}

Aprenda a añadir elementos por lotes a la campaña de ventas en Salesforce para escalar la comunicación saliente mediante las acciones de ventas.

>[!NOTE]
>
>Salesforce aplica un límite de 200 registros que se pueden seleccionar a la vez.

>[!PREREQUISITES]
>
>Asegúrese de que ha instalado el [último paquete de Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} en su instancia de Salesforce y de que ha configurado los [botones de acción](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} en las vistas de contactos y listas de posibles clientes en Salesforce.

## Añadir masivamente a la campaña de ventas en Salesforce Lightning {#bulk-add-to-sales-campaign-in-salesforce-lightning}

1. En Salesforce, vaya a la página de inicio de los posibles clientes o contactos haciendo clic en la ficha **Posibles clientes o contactos**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-1.png)

1. En el menú desplegable **Vista**, seleccione la vista que desee de los posibles clientes/contactos que desee enviar por correo electrónico.

   >[!TIP]
   >
   >Para crear una vista nueva, haz clic en el icono de engranaje a la derecha y selecciona **Nuevo**. Una vez que le haya dado a la vista un nuevo nombre y lo haya guardado, puede hacer clic en el icono de filtro de la derecha para ayudar a filtrar hasta el conjunto deseado de posibles clientes/contactos que desee enviar por correo electrónico.

1. Elija la lista de contactos o posibles clientes que desee y haga clic en el botón **Agregar a la campaña de ventas**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-2.png)

1. Se le dirigirá al modal Actions Sales Campaign, con los destinatarios seleccionados añadidos.

1. Realice las modificaciones necesarias para eliminar personas o grupos y, a continuación, haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-3.png)

1. Seleccione la categoría de campaña de ventas que desee utilizar en la lista desplegable Categorías.

1. Seleccione la campaña de ventas a la que desee agregar a las personas seleccionadas y haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-4.png)

1. Puede ver diferentes opciones en función del primer paso de la campaña. Si el primer paso es un correo electrónico, tiene la opción de editar el correo electrónico para cada destinatario, como se muestra a continuación. Una vez hecho esto, haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-5.png)

1. De nuevo, si el primer paso es un correo electrónico y lo configuró para permitirle seleccionar cuándo se inicia la campaña, tendrá la opción de **Comenzar ahora** o **Programar una nueva hora de inicio**. Una vez que haya completado esto, haga clic en **Iniciar**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-6.png)

Después de hacer clic en Inicio, verá una pantalla de confirmación que le permite saber cuántas personas se han agregado.

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-7.png)

## Añadir de forma masiva a la campaña de ventas en Salesforce Classic {#bulk-add-to-sales-campaign-in-salesforce-classic}

1. En Salesforce, haga clic en la ficha **Posibles clientes/contactos**.

1. En el menú desplegable Ver, selecciona la vista que desees de los posibles clientes o contactos que deseas enviar por correo electrónico y haz clic en **Ir**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-8.png)

   >[!TIP]
   >
   >Puede crear una nueva vista haciendo clic en Create New View y configurando los filtros disponibles para reducir la lista de destinatarios que enviará por correo electrónico.

1. Elija el posible cliente o la lista de contactos que desee y haga clic en el botón **Agregar a la campaña de ventas**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-9.png)

1. Se le dirigirá al modal de campañas de ventas de acciones con las personas seleccionadas añadidas.

1. Realice las modificaciones necesarias para eliminar personas o grupos y, a continuación, haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-10.png)

1. Seleccione la categoría de campaña de ventas que desee usar en la lista desplegable **Categorías**.

1. Seleccione la campaña de ventas a la que desee agregar a las personas seleccionadas y haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-11.png)

1. Puede ver diferentes opciones en función del primer paso de la campaña. Si el primer paso es un correo electrónico, tiene la opción de editar el correo electrónico para cada destinatario, como se muestra a continuación. Una vez hecho esto, haga clic en **Siguiente**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-12.png)

1. De nuevo, si el primer paso es un correo electrónico y lo configuró para permitirle seleccionar cuándo se inicia la campaña, tendrá la opción de **Comenzar ahora** o **Programar una nueva hora de inicio**. Una vez que haya completado esto, haga clic en **Iniciar**.

   ![](assets/using-bulk-add-to-sales-campaign-in-salesforce-13.png)

Después de hacer clic en Inicio, verá una pantalla de confirmación que le permite saber cuántas personas se han agregado.

![](assets/using-bulk-add-to-sales-campaign-in-salesforce-14.png)
