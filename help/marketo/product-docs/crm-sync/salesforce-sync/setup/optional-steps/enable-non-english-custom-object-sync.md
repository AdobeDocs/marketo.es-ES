---
unique-page-id: 4719302
description: Habilitar la sincronización de objetos personalizados sin inglés - Documentos de Marketo - Documentación del producto
title: Habilitar la sincronización de objetos personalizados sin inglés
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Habilitar la sincronización de objetos personalizados sin inglés {#enable-non-english-custom-object-sync}

Si el usuario de sincronización de Marketo está configurado en un idioma distinto del inglés, puede que se produzca un error al intentar habilitar una sincronización de objetos personalizada.

## El error {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Cómo evitarlo {#getting-around-it}

1. Inicie sesión en Salesforce utilizando el marketing para sincronizar al usuario.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Bajo el nombre de usuario, vaya a **Configuración**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. En **Información personal**, haga clic en **Mi información personal**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Haga clic en **Editar**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Cambie el **Idioma** a **Inglés**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Vuelva a Marketo, en **Administración > Salesforce > Objetos** click **Actualizar esquema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Esto extraerá la lista de objetos en inglés. A continuación, seleccione el objeto que desee y haga clic en **Habilitar sincronización**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que el objeto personalizado ahora está habilitado y sincronizándose.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Vuelva a Salesforce y siga los pasos anteriores para cambiar el usuario de sincronización a su idioma preferido.

>[!NOTE]
>
>No olvide actualizar esquema una última vez para extraer los objetos de nuevo en su idioma.
