---
unique-page-id: 11382593
description: Configuración de Web Personalization para no realizar el seguimiento - Documentos de Marketo - Documentación del producto
title: Configuración de la personalización web para no realizar el seguimiento
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 3%

---

# Configurando [!UICONTROL Web Personalization] para no rastrear {#setting-web-personalization-to-do-not-track}

Los visitantes web pueden configurar su navegador para evitar el seguimiento de cualquier sitio web, eligiendo &quot;No rastrear&quot; (DNT). Esto evita el seguimiento de ese explorador y dispositivo en particular.

En [!UICONTROL Web Personalization] y [!UICONTROL Contenido predictivo], un especialista en mercadotecnia puede establecer una opción para indicar si se admite o se ignora la configuración No rastrear (DNT) del explorador. La opción para cuentas está desactivada de forma predeterminada, lo que significa que la aplicación no respeta el DNT.

## Habilitar o deshabilitar la opción de alternancia {#enable-or-disable-the-toggle}

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. En [!UICONTROL Dominio] y [!UICONTROL Configuración del dominio], seleccione **[!UICONTROL Activado]** para habilitar la opción [!UICONTROL Honrar DNT].

   ![](assets/two-1.png)

   Cuando la opción se establece en [!UICONTROL Activado], Web Personalization respetará y admitirá la configuración No rastrear (DNT) del explorador, y no rastreará ninguna actividad web ni ejecutará campañas ni recomendaciones de contenido en el sitio web.

   >[!NOTE]
   >
   >Si establece la opción en [!UICONTROL Activado], el valor y la funcionalidad de Marketo podrían verse afectados en áreas específicas.

1. Para deshabilitar la opción [!UICONTROL Respetar DNT] e ignorar la configuración Do No Track (DNT) del explorador, seleccione **[!UICONTROL Desactivado]** en [!UICONTROL Respetar DNT].
