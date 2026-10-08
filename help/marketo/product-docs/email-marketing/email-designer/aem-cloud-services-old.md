---
title: Conectar documento de Experience Manager
description: Obtenga información sobre cómo conectar AEM Cloud Services a Marketo Engage. Utilice sus recursos de AEM al crear correos electrónicos en el diseñador.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: 'yes'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 8%
---
# Conectar Adobe Experience Manager Cloud Services {#connect-adobe-experience-manager-cloud-services}

Obtenga información sobre cómo conectar su cuenta de AEM Assets Cloud Services a su instancia de Adobe Marketo Engage para poder aprovechar el repositorio de recursos de AEM en Marketo Engage Email Designer.

>[!NOTE]
>
>**Se requieren permisos de administrador**

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

1. El repositorio configurado se muestra a continuación junto con el estado y la caducidad. Haga clic en el botón de los tres puntos (**...**) para ver el certificado. De lo contrario, habrá terminado.

CAPTURA DE PANTALLA

Ahora se puede acceder a todas las imágenes de la biblioteca de administración de recursos digitales de ese repositorio desde Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Trabajar con recursos de Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
