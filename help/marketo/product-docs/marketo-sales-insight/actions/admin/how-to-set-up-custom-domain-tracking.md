---
description: 'Configuración del seguimiento de dominio personalizado: documentos de Marketo, documentación del producto'
title: Cómo configurar el seguimiento de dominios personalizados
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Cómo configurar el seguimiento de dominios personalizados {#how-to-set-up-custom-domain-tracking}

El seguimiento personalizado de dominios permite a su equipo utilizar su propio nombre de empresa en todos los vínculos a los que se puede realizar un seguimiento y que se añaden a los correos electrónicos de ventas. Una vez configurado, lista de permitidos cualquier vínculo que tenga en su correo electrónico para que aparezca como go.yourcompany.com, de modo que cuando alguien pase el ratón sobre un vínculo, lea go.yourcompany.com en lugar de go.toutapp.com.

Necesitará ayuda de su equipo de TI para configurar un registro CNAME para su dominio que apunte a go.toutapp.com. Este CNAME es lo que aparece en todos los vínculos de seguimiento (por ejemplo, go.yourcompany.com).

Una vez que haya confirmado con su equipo de TI que el CNAME está configurado correctamente, puede añadirlo a la página Seguimiento de dominios personalizados en Acciones.

>[!NOTE]
>
>Si el CNAME no está configurado correctamente y lo activa como dominio personalizado en Acciones, puede interrumpir los vínculos de seguimiento y los píxeles.

## Habilitar seguimiento de dominio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>Se requieren **privilegios de administrador.**

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. En Configuración de administración, seleccione **Seguimiento**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. En la pestaña Seguimiento de dominio personalizado, escriba su CNAME y haga clic en **Conectar**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
