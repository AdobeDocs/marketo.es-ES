---
unique-page-id: 11382593
description: Configuración de Web Personalization para no realizar el seguimiento - Documentos de Marketo - Documentación del producto
title: Configuración de Web Personalization para que no realice el seguimiento
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Configuración de Web Personalization para que no realice el seguimiento {#setting-web-personalization-to-do-not-track}

Los visitantes web pueden configurar su navegador para evitar el seguimiento de cualquier sitio web, eligiendo &quot;No rastrear&quot; (DNT). Esto evita el seguimiento de ese explorador y dispositivo en particular.

En Web Personalization y Contenido predictivo, un experto en marketing puede establecer una opción para indicar si se admite o se ignora la configuración No rastrear (DNT) del explorador. La opción para cuentas está desactivada de forma predeterminada, lo que significa que la aplicación no respeta el DNT.

## Habilitar o deshabilitar la opción de alternancia {#enable-or-disable-the-toggle}

1. Vaya a **Configuración de la cuenta**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. En Configuración de dominio y dominio, seleccione **Activado** para habilitar la opción Honrar DNT.

   ![](assets/two-1.png)

   Cuando la opción está Activada, Web Personalization respetará y admitirá la configuración No rastrear (DNT) del explorador, y no rastreará ninguna actividad web ni ejecutará campañas ni recomendaciones de contenido en el sitio web.

   >[!NOTE]
   >
   >Si establece el conmutador en Activado, puede afectar al valor y la funcionalidad de Marketo en áreas específicas.

1. Para deshabilitar la opción Honrar DNT e ignorar la configuración No rastrear (DNT) del explorador, seleccione **Desactivado** en Honrar DNT.
