---
description: Obtenga información sobre cómo configurar el seguimiento de dominios personalizados para que los vínculos a los que se puede realizar un seguimiento utilicen el dominio de la empresa.
title: Cómo configurar el seguimiento del dominio personalizado
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/gn3uC4uxpwp35IVYcUs-cZJFqbmPc-7vTmgbIPm8lTk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 197
ht-degree: 7%

---

# Cómo configurar el seguimiento del dominio personalizado {#how-to-set-up-custom-domain-tracking}

El seguimiento personalizado de dominios permite a su equipo utilizar su propio nombre de empresa en todos los vínculos a los que se puede realizar un seguimiento y que se añaden a los correos electrónicos de ventas. Una vez configurado, lista de permitidos cualquier vínculo que tenga en su correo electrónico para que aparezca como go.yourcompany.com, de modo que cuando alguien pase el ratón sobre un vínculo, lea go.yourcompany.com en lugar de go.toutapp.com.

Necesitará ayuda de su equipo de TI para configurar un registro CNAME para su dominio que apunte a go.toutapp.com. Este CNAME es lo que aparece en todos los vínculos de seguimiento (por ejemplo, go.yourcompany.com).

Una vez que haya confirmado con su equipo de TI que el CNAME está configurado correctamente, puede agregarlo a la página [!UICONTROL Seguimiento de dominios personalizados] en Acciones.

>[!NOTE]
>
>Si el CNAME no está configurado correctamente y lo activa como dominio personalizado en Acciones, puede interrumpir los vínculos de seguimiento y los píxeles.

## Habilitar seguimiento de dominio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>Se requieren **privilegios de administrador.**

1. Haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. En [!UICONTROL Configuración de administración], seleccione **[!UICONTROL Seguimiento]**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. En la ficha [!UICONTROL Seguimiento personalizado de dominios], escriba su CNAME y haga clic en **[!UICONTROL Conectar]**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
