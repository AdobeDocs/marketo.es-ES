---
unique-page-id: 4720232
description: 'Creación de una nueva lista de cuentas: documentos de Marketo, documentación del producto'
title: Crear una nueva lista de cuentas
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 1%

---

# Crear una nueva lista de cuentas {#create-a-new-account-list}

Cree y cargue una lista de nombres de organización y dominio para dirigirse a estas cuentas clave con campañas personalizadas.

>[!NOTE]
>
>Este artículo se aplica solo a los clientes de Web ABM heredados. Si adquirió Web ABM después de septiembre de 2016, siga los pasos de [este artículo](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList).

## Crear una nueva lista de cuentas {#create-a-new-account-list-1}

1. Ir a **[!UICONTROL Listas de cuentas]**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Seleccione **[!UICONTROL Crear nuevo]**.

   ![](assets/create-new-account-list-hand.jpg)

1. Seleccione **[!UICONTROL Examinar]** y cargue el archivo CSV (asegúrese de que el archivo CSV cumpla los criterios). Agregar **[!UICONTROL nombre de lista]** y **[!UICONTROL descripción]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**¿Cuál es el formato del archivo CSV?**
   >
   >Asegúrese de que el archivo CSV de la cuenta con nombre cumple los siguientes requisitos:
   >
   >* Guardado como formato CSV
   >* No supera los 10 MB
   >* Solo 4 columnas con el encabezado Columna A: Nombre, Columna B: Dominio, Columna C: País, Columna D: Estado de EE. UU.
   >* El archivo cargado puede tardar hasta dos días hábiles antes de la aprobación.
   >* Recibirá una notificación de correo electrónico de aprobación o comprobará el estado del archivo en la página Cuentas con nombre.
   >* El número total de registros/filas acumulados para todas las listas cargadas comienza en 10K, con un total de 100K en el paquete más grande.

   >[!NOTE]
   >
   >**Ejemplo del archivo CSV**
   >
   >* Fila 1 Columna A valor = Organización
   >* Valor de columna B de fila 1 = Dominio
   >* Fila 1 Columna C valor = País
   >* Valor D de columna de fila 1 = Estado de EE. UU.
   >* Uno de los valores de columna es obligatorio. Sin embargo, si se proporcionan los nombres Organización y Dominio, mejoran las tasas de coincidencia de la Lista de cuentas.
   >* País y Estado son valores opcionales.
   >
   >   * Para el nombre del país, utilice un nombre de país completo o un código de abreviatura. P. ej. Estados Unidos o EE. UU.
   >   * Para un estado de EE. UU., utilice el código de abreviatura de 2 letras, es decir, CA. Solo se reconocen los estados de EE. UU.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Editar una lista de cuentas {#edit-an-account-list}

En la página **Listas de cuentas**, haga clic en el icono **Editar** de la lista.

![](assets/create-new-account-list-edit.jpg)

Seleccione **[!UICONTROL Examinar...]** y cargue el nuevo archivo CSV. Este archivo reemplazará el archivo original. Haga clic en **[!UICONTROL Guardar]**. El nuevo archivo cargado estará en estado pendiente hasta que el soporte técnico de Marketo lo apruebe; cuando esté en estado pendiente, el archivo original permanecerá activo.

![](assets/set-account-list-edit-hands.jpg)

El archivo CSV reemplazará al archivo existente. La lista existente permanecerá activa hasta que se complete el procesamiento del nuevo archivo.

## Eliminar una lista de cuentas con nombre {#delete-a-named-account-list}

1. En la página **[!UICONTROL Listas de cuentas]**, haga clic en el icono Eliminar de la lista que desee eliminar.

   ![](assets/create-new-account-list-delete.jpg)

1. Aparecerá un mensaje para confirmar si desea eliminar la lista. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Crear un segmento con una lista de cuentas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
