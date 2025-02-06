---
title: Trabajar con Experience Manager Assets
description: Aprenda a utilizar recursos de imagen de un repositorio de AEM Assets conectado al crear contenido en Adobe Marketo Engage.
exl-id: c2172042-a35c-4179-bf81-6e96323bd4d4
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---

# Uso de recursos de Experience Manager {#work-with-experience-manager-assets}

Cuando _Adobe Experience Manager Assets as a Cloud Service_ esté integrado con Adobe Marketo Engage, podrá acceder fácilmente a los recursos digitales para usarlos en el contenido de marketing.

>[!PREREQUISITES]
>
>[Conecte los Cloud Service de Adobe Experience Manager a su instancia de Adobe Marketo Engage](/help/marketo/product-docs/email-marketing/email-designer/aem-cloud-services.md){target="_blank"}

>[!NOTE]
>
>Actualmente, solo se admiten en Marketo Engage los recursos de imagen de _Adobe Experience Manager Assets_. Los cambios en los recursos deben realizarse desde el repositorio central de Adobe Experience Manager Assets. [Más información](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets){target="_blank"}

Cuando usa estos recursos digitales, los cambios más recientes en _Assets as a Cloud Service_ se propagan automáticamente a las campañas de correo electrónico activas a través de referencias vinculadas. Si las imágenes se eliminan en _Adobe Experience Manager Assets as a Cloud Service_, aparecerán con una referencia rota en los correos electrónicos. Cuando se modifican o eliminan recursos que se utilizan actualmente en Marketo Engage, se notifica a los autores de correo electrónico sobre los cambios de imagen. Todos los cambios en los recursos deben realizarse en el repositorio central de Adobe Experience Manager Assets.

## Usar AEM Assets como origen de imagen {#use-aem-assets-as-the-image-source}

Si su entorno tiene una o más conexiones de repositorio de recursos, puede designar AEM Assets como origen de los recursos al crear o ver los detalles de un correo electrónico, una plantilla de correo electrónico o un fragmento visual.

* Al crear contenido nuevo, elija `AEM Assets` como el elemento **[!UICONTROL Image Source]** del cuadro de diálogo.

![Seleccionar AEM Assets como origen de imagen en el cuadro de diálogo de creación](assets/work-with-experience-manager-assets-1.png){width="400"}

* Al abrir un recurso de contenido existente, elija `AEM Assets` en la sección _[!UICONTROL Cuerpo]_ de la derecha.

![Seleccionar AEM Assets como origen de imagen en las propiedades](assets/work-with-experience-manager-assets-2.png){width="700" zoomable="yes"}

## Acceso a recursos para la creación {#access-assets-for-authoring}

>[!IMPORTANT]
>
>Un administrador debe añadir usuarios que necesiten acceder a los recursos a los perfiles de producto de Usuarios consumidores de Assets o Usuarios de Assets. [Más información](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

En el editor de contenido visual, haga clic en el icono _Selector de recursos del Experience Manager_ en la barra lateral izquierda. Esto cambia el panel Herramientas a una lista de recursos disponibles en el repositorio seleccionado.

![Haga clic en el icono del selector de Assets para acceder a los recursos de imagen](assets/work-with-experience-manager-assets-3.png){width="700" zoomable="yes"}

AEM Si tiene más de un repositorio conectado, haga clic en el botón **[!UICONTROL Administrar como]** para seleccionar el repositorio que desea usar.

![Elija un repositorio de AEM Assets para acceder a los recursos de imagen](assets/work-with-experience-manager-assets-4.png){width="700" zoomable="yes"}

Elija el repositorio que desee.

![Elija un repositorio de AEM Assets para acceder a los recursos de imagen](assets/work-with-experience-manager-assets-5.png)

Existen varios métodos para agregar un recurso de imagen al lienzo visual:

* Arrastre y suelte una miniatura de imagen desde el panel de navegación izquierdo.

![Elija un repositorio de AEM Assets para acceder a los recursos de imagen](assets/work-with-experience-manager-assets-6.png){width="700" zoomable="yes"}

* Agregue un componente de imagen al lienzo y haga clic en **[!UICONTROL Examinar]** para abrir el cuadro de diálogo _[!UICONTROL Seleccionar Assets]_.

  En el cuadro de diálogo, puede elegir una imagen del repositorio seleccionado.

  Hay varias herramientas disponibles para ayudarle a localizar el recurso que necesita.

![Use la herramienta en el cuadro de diálogo Seleccionar Assets para buscar y seleccionar un recurso de imagen](assets/work-with-experience-manager-assets-7.png){width="700" zoomable="yes"}

* Cambie **[!UICONTROL Repositorio]** en la parte superior derecha.

* Haga clic en **[!UICONTROL Administrar recursos]** en la parte superior derecha para abrir el repositorio de Assets en otra pestaña del explorador y usar las herramientas de administración de AEM Assets.

* Haga clic en el selector _Tipo de vista_ en la parte superior derecha para cambiar la pantalla a **[!UICONTROL Vista de lista]**, **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de galería]** o **[!UICONTROL Vista de cascada]**.

* Haga clic en el icono _Orden_ para cambiar el orden de clasificación entre ascendente y descendente.

* Haga clic en la flecha de menú **[!UICONTROL Ordenar por]** para cambiar los criterios de ordenación a **[!UICONTROL Nombre]**, **[!UICONTROL Tamaño]** o **[!UICONTROL Modificado]**.

* Haga clic en el icono _Filtrar_ en la parte superior izquierda para filtrar los elementos mostrados según sus criterios.

* Introduzca texto en el campo Buscar para filtrar los elementos mostrados para buscar una coincidencia del nombre del recurso.

![Use los filtros y el campo de búsqueda para localizar el recurso](assets/work-with-experience-manager-assets-8.png){width="700" zoomable="yes"}
