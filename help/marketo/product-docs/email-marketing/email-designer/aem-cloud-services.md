---
title: Documento de Experience Manager de Connect
description: Obtenga información sobre cómo conectar Cloud Service de Adobe Experience Manager a Adobe Marketo Engage AEM para poder aprovechar sus recursos de.
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Conexión de Cloud Service de Adobe Experience Manager {#connect-adobe-experience-manager-cloud-services}

Obtenga información sobre cómo conectar su cuenta de Cloud Service de AEM Assets a la de Adobe Marketo Engage para poder aprovechar el repositorio de recursos de la instancia de AEM en el Designer de correo electrónico del Marketo Engage.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. En Marketo Engage, vaya al área de **Admin** y seleccione **Adobe Experience Manager** en el árbol de navegación izquierdo.

   ![Seleccione Adobe Experience Manager en la sección de administración](assets/connect-adobe-experience-manager-cloud-services-1.png){width="800"}

1. Haga clic en **Editar** junto a _Cloud Service de Adobe Experience Manager_.

   ![Haga clic en Editar](assets/connect-adobe-experience-manager-cloud-services-2.png){width="400"}

1. Seleccione uno o varios repositorios.

   ![Seleccionar un repositorio](assets/connect-adobe-experience-manager-cloud-services-3.png){width="800"}

   >[!NOTE]
   >
   >Solo se muestran los repositorios que se han asociado en la misma organización de IMS que su suscripción de Marketo Engage.

1. Debe agregar un [certificado de credencial de servicio](https://experienceleague.adobe.com/es/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) para configurar el repositorio. Haga clic en el botón **+ Agregar certificado**.

   ![Agregar certificado](assets/connect-adobe-experience-manager-cloud-services-4.png){width="800"}

1. Arrastre y suelte el certificado (solo archivo JSON) o selecciónelo en el equipo. Haga clic en **Agregar** cuando haya terminado.

   ![Busque el certificado en su equipo](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

1. El repositorio configurado se muestra a continuación junto con el estado y la caducidad. Haga clic en el botón de los tres puntos (**...**) para ver el certificado. De lo contrario, has terminado.

   ![Se ha agregado el certificado](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

Ahora se puede acceder a todas las imágenes de la biblioteca de administración de recursos digitales de ese repositorio desde el correo electrónico del Marketo Engage Designer.

>[!MORELIKETHIS]
>
>[Trabajar con recursos de Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
