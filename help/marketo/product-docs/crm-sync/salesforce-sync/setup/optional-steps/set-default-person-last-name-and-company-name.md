---
unique-page-id: 4719291
description: Establecer apellidos y nombre de empresa de la persona predeterminada - Documentos de Marketo - Documentación del producto
title: Establecer apellidos de persona y nombre de compañía predeterminados
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Establecer apellidos de persona y nombre de compañía predeterminados {#set-default-person-last-name-and-company-name}

Salesforce requiere (como mínimo) apellidos y nombre de compañía para sus posibles clientes y contactos. Los registros incompletos no se sincronizarán con Salesforce. Si desea sincronizar registros parciales, debe establecer los valores predeterminados que Marketo utilizará con Salesforce.

1. Ir a **Administrador** y haga clic en **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clic **Editar opciones de sincronización**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Introduzca una **Apellidos de la persona predeterminada** y una **Compañía de persona predeterminada** luego haga clic en **Guardar**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo solo asigna un valor predeterminado cuando el registro se sincroniza inicialmente con Salesforce y solo si alguno de los campos obligatorios está vacío.

¡Y eso es todo! Cada vez que a una persona le falta un apellido o un nombre de empresa, Marketo agrega el valor predeterminado a medida que sincroniza el registro.
