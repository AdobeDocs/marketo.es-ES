---
unique-page-id: 4719302
description: Habilitar la sincronización de objetos personalizados que no están en inglés - Documentos de marketing - Documentación del producto
title: Habilitar sincronización de objetos personalizados que no están en inglés
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Habilitar la sincronización de objetos personalizados que no están en inglés {#enable-non-english-custom-object-sync}

Si el usuario de sincronización de Marketing to está configurado en un idioma distinto al inglés, puede producirse un error al intentar habilitar una sincronización de objetos personalizada.

## El error {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Alcanzar su entorno {#getting-around-it}

1. Inicie sesión en Salesforce con el usuario de sincronización de marketing.

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

1. De nuevo en Marketing, en **Administración > Salesforce > Objetos** haga clic en **Actualizar Esquema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Esto extraerá la lista de objetos en inglés. Ahora seleccione el objeto que desee y haga clic en **Habilitar sincronización**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que el objeto personalizado está ahora activado y se está sincronizando.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ahora vuelva a Salesforce y siga los pasos anteriores para cambiar el usuario de sincronización a su idioma preferido.

>[!NOTE]
>
>**Recordatorio**
>
>No olvide actualizar el Esquema una última vez para recuperar los objetos en su idioma.

