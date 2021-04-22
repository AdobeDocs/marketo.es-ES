---
unique-page-id: 4719291
description: 'Definir apellidos de persona y nombre de empresa predeterminados: documentos de Marketo: documentación del producto'
title: Definir los apellidos de la persona y el nombre de la empresa predeterminados
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Definir los apellidos de la persona y el nombre de la empresa predeterminados {#set-default-person-last-name-and-company-name}

Salesforce requiere un apellido (mínimo) y un nombre de empresa para sus posibles clientes y contactos. Los registros incompletos no se sincronizarán con Salesforce. Si desea sincronizar registros parciales, debe establecer los valores predeterminados para que Marketo los utilice con Salesforce.

1. Vaya a **Admin** y haga clic en **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Haga clic en **Editar opciones de sincronización**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Introduzca un **Default person last name** y una **Default person company** y haga clic en **Save**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo solo asigna un valor predeterminado cuando el registro se sincroniza inicialmente con Salesforce y solo si alguno de los campos obligatorios está vacío.

¡Y eso es todo! Cada vez que a una persona le falten un apellido o un nombre de empresa, Marketo agregará el valor predeterminado a medida que sincronice el registro.
