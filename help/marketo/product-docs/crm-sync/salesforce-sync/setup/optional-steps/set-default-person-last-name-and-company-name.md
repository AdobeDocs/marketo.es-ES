---
unique-page-id: 4719291
description: Definir el nombre de la persona y el nombre de la Compañía predeterminados - Documentos de marketing - Documentación del producto
title: Definir el nombre de la persona y el nombre de la Compañía predeterminados
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Definir el apellido de la persona y el nombre de la Compañía predeterminados {#set-default-person-last-name-and-company-name}

Salesforce requiere un apellido (mínimo) y un nombre de compañía para sus posibles clientes y contactos. Los registros incompletos no se sincronizarán con Salesforce. Si desea sincronizar registros parciales, debe establecer los valores predeterminados para que Marketing pueda usarlos con Salesforce.

1. Vaya a **Administración** y haga clic en **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Haga clic en **Editar opciones de sincronización**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Introduzca un **apellido de persona predeterminado** y un **Predeterminado ****compañía de persona** y haga clic en **Guardar**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo sólo asigna un valor predeterminado cuando el registro se sincroniza inicialmente con Salesforce y solo si alguno de los campos obligatorios está vacío.

¡Y eso es eso! Cada vez que a una persona le falta un apellido o un nombre de compañía, Marketo agrega el valor predeterminado a medida que sincroniza el registro.
