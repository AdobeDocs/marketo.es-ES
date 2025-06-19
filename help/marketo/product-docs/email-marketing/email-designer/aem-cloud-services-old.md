---
title: Conectar documento de Experience Manager
description: Obtenga información sobre cómo conectar Adobe Experience Manager Cloud Services a Adobe Marketo Engage para poder aprovechar los recursos de AEM.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Conectar Adobe Experience Manager Cloud Services {#connect-adobe-experience-manager-cloud-services}

Obtenga información sobre cómo conectar su cuenta de AEM Assets Cloud Services a su instancia de Adobe Marketo Engage para poder aprovechar el repositorio de recursos de AEM en Marketo Engage Email Designer.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. En Marketo Engage, vaya al área **Admin** y seleccione **Adobe Experience Manager** en el árbol de navegación izquierdo.

CAPTURA DE PANTALLA

1. Haga clic en **Editar** junto a _Adobe Experience Manager Cloud Services_.

CAPTURA DE PANTALLA

1. Seleccione uno o varios repositorios.

CAPTURA DE PANTALLA

>[!NOTE]
>
>Solo se muestran los repositorios que se han asociado en la misma organización de IMS que su suscripción a Marketo Engage.

1. Debe agregar un [certificado de credencial de servicio](https://experienceleague.adobe.com/es/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) para configurar el repositorio. Haga clic en el botón **+ Agregar certificado**.

CAPTURA DE PANTALLA

1. Arrastre y suelte el certificado (solo archivo JSON) o selecciónelo en el equipo. Haga clic en **Agregar** cuando haya terminado.

CAPTURA DE PANTALLA

1. El repositorio configurado se muestra a continuación junto con el estado y la caducidad. Haga clic en el botón de los tres puntos (**...**) para ver el certificado. De lo contrario, has terminado.

CAPTURA DE PANTALLA

Ahora se puede acceder a todas las imágenes de la biblioteca de administración de recursos digitales de ese repositorio desde Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Trabajar con recursos de Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
