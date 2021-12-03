---
description: Configuración del seguimiento de dominios personalizado - Documentos de Marketo - Documentación del producto
title: Configuración del seguimiento de dominio personalizado
hide: true
hidefromtoc: true
source-git-commit: ec78e047c9dc126553fe8a4b6a4c21b0d11aea5c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Configuración del seguimiento de dominio personalizado {#how-to-set-up-custom-domain-tracking}

El seguimiento de dominio personalizado permite que su equipo use su propio nombre de empresa en todos los vínculos rastreables que se agregan a los correos electrónicos de ventas. Una vez que tenga esto configurado, lista de permitidos cualquier vínculo que tenga en su correo electrónico para que aparezca como go.yourcompany.com, de modo que cuando alguien pase el ratón sobre un vínculo, lea go.yourcompany.com en lugar de go.toutapp.com.

Necesitará la asistencia de su equipo de TI para configurar un registro CNAME para su dominio que apunte a go.toutapp.com. Este CNAME es lo que aparece en todos sus vínculos de seguimiento (por ejemplo, go.yourcompany.com).

Una vez que haya confirmado con su equipo de TI que el CNAME está configurado correctamente, puede agregarlo a la página Seguimiento de dominios personalizado en Acciones.

>[!NOTE]
>
>Si el CNAME no está configurado correctamente y lo activa como su dominio personalizado en Acciones, puede romper los vínculos de seguimiento y los píxeles.

## Habilitar el seguimiento de dominio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Se requieren privilegios de administrador.**

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. En Configuración de administración, seleccione **Seguimiento**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. En la pestaña Seguimiento de dominios personalizado , introduzca su CNAME y haga clic en **Connect**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
