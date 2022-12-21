---
unique-page-id: 4720232
description: 'Crear una nueva lista de cuentas: Documentos de Marketo: Documentación del producto'
title: Crear una nueva lista de cuentas
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Crear una nueva lista de cuentas {#create-a-new-account-list}

Cree y cargue una lista de nombres de dominio y organización para dirigirse a estas cuentas clave con campañas personalizadas.

>[!NOTE]
>
>Este artículo aplica solo a clientes Web ABM heredados. Si adquirió Web ABM después de septiembre de 2016, siga los pasos indicados en [este artículo](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) en su lugar.

## Crear una nueva lista de cuentas {#create-a-new-account-list-1}

1. Vaya a **Listas de cuentas**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Select **Crear nuevo**.

   ![](assets/create-new-account-list-hand.jpg)

1. Select **Examinar** y cargue el archivo CSV (asegúrese de que el archivo CSV cumpla los criterios). Agregue un **Nombre** y **Descripción**. Haga clic en **Guardar**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**¿Cuál es el formato del archivo CSV?**
   >
   >Asegúrese de que el archivo CSV de cuenta con nombre cumpla los siguientes requisitos:
   >
   >* Guardado como formato CSV
   >* No supera los 10 MB
   >* Solo 4 columnas con el encabezado Columna A: Nombre, Columna B: Dominio, columna C: País, columna D: Estado de EE. UU.
   >* El archivo cargado puede tardar hasta 2 días hábiles antes de la aprobación.
   >* Recibirá una notificación por correo electrónico de aprobación o comprobará el estado del archivo en la página Cuentas con nombre .
   >* El número total de registros/filas acumulados para todas las listas cargadas comienza en 10K, con el paquete más grande en total 100K.


   >[!NOTE]
   >
   >**Ejemplo del archivo CSV**
   >
   >* Fila 1 Columna A valor = Organización
   >* Fila 1 Valor de columna B = Dominio
   >* Fila 1 Valor de columna C = País
   >* Fila 1 Valor D de columna = Estado de EE. UU.
   >* Uno de los valores de columna es obligatorio. Sin embargo, al proporcionar nombres de organización y de dominio, se mejoran las tasas de coincidencia de la lista de cuentas.
   >* El país y el estado son valores opcionales.
      >
      >   * Para el nombre del país, utilice el nombre completo del país o el código de abreviatura. Por ejemplo. Estados Unidos o Estados Unidos.
      >   * Para un estado de EE. UU., utilice el código de abreviación de 2 letras, por ejemplo CA. Solo se reconocen los estados de EE. UU.

   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Editar una lista de cuentas {#edit-an-account-list}

En el **Listas de cuentas** , haga clic en el botón **Editar** en la lista.

![](assets/create-new-account-list-edit.jpg)

Select **Examinar** y cargue el nuevo archivo CSV. Este archivo reemplazará al archivo original. Haga clic en **Guardar**. El nuevo archivo cargado estará en estado pendiente hasta que lo apruebe el equipo de asistencia de Marketo, cuando en un estado pendiente el archivo original permanezca activo.

![](assets/set-account-list-edit-hands.jpg)

El archivo CSV reemplazará al archivo existente. La lista existente permanecerá activa hasta que se complete el procesamiento del nuevo archivo.

## Eliminar una lista de cuentas con nombre {#delete-a-named-account-list}

1. En el **Listas de cuentas** , haga clic en el icono Eliminar de la lista que desee eliminar.

   ![](assets/create-new-account-list-delete.jpg)

1. Aparecerá un mensaje para confirmar si desea eliminar la lista. Haga clic en **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Crear un segmento mediante una lista de cuentas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
