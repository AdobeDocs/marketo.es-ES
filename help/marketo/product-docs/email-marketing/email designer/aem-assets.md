---
title: Trabajar con Experience Manager Assets
description: Descubra cómo puede utilizar recursos de imagen de un repositorio de AEM Assets conectado al crear contenido en Adobe Marketo Engage.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Uso de recursos de Experience Manager

Cuando Adobe Experience Manager Assets as a Cloud Service está integrado con Adobe Marketo Engage, puede descubrir fácilmente recursos digitales y acceder a ellos para utilizarlos en su contenido de marketing. A medida que crea su contenido, se puede acceder a los recursos desde el elemento _[!UICONTROL Assets]_ en el panel de navegación izquierdo y durante la creación de contenido de correo electrónico para un recorrido de cuenta. También puede cargar recursos en el repositorio as a Cloud Service de AEM Assets conectados directamente desde Adobe Journey Optimizer B2B edition.

>[!NOTE]
>
>Actualmente, solo se admiten recursos de imagen de Adobe Experience Manager Assets en Adobe Journey Optimizer B2B edition. Los cambios en los recursos deben realizarse desde el repositorio central de Adobe Experience Manager Assets. [Más información](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Al utilizar estos recursos digitales, los cambios más recientes en Assets as a Cloud Service se propagan automáticamente a las campañas de correo electrónico en directo a través de referencias vinculadas. Si las imágenes se eliminan en Adobe Experience Manager Assets as a Cloud Service, estas aparecerán con una referencia rota en los correos electrónicos. Cuando se modifican o eliminan recursos que se utilizan actualmente en recorridos de cuenta, se notifica a los autores del recorrido sobre los cambios de imagen y la lista de recorridos que utilizan la imagen. Todos los cambios en los recursos deben realizarse en el repositorio central de Adobe Experience Manager Assets.

## Usar AEM Assets como origen de imagen

Si su entorno tiene una o más conexiones de repositorios de Assets, puede designar AEM Assets como origen de los recursos al crear o ver los detalles de un correo electrónico, una plantilla de correo electrónico o un fragmento visual.

* Cuando cree contenido nuevo, elija `AEM Assets` como el elemento **[!UICONTROL Image Source]** del cuadro de diálogo.

CAPTURA DE PANTALLA

* Cuando abra un recurso de contenido existente, elija `AEM Assets` en el panel _[!UICONTROL Cuerpo]_ de la derecha.

CAPTURA DE PANTALLA

## Acceso a recursos para la creación

>[!IMPORTANT]
>
>Un administrador debe añadir usuarios que necesiten acceder a Assets a los perfiles de producto Usuarios consumidores de Assets y Usuarios de Assets. [Más información](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

En el editor de contenido visual, haga clic en el icono _Selector de recursos_ en la barra lateral izquierda. Esto cambia el panel Herramientas a una lista de recursos disponibles en el repositorio seleccionado.

CAPTURA DE PANTALLA

AEM Si tiene más de un repositorio conectado, haga clic en la flecha de menú de **[!UICONTROL Repositorio]** para elegir el repositorio que desea utilizar.

CAPTURA DE PANTALLA

Existen varios métodos para agregar un recurso de imagen al lienzo visual:

* Arrastre y suelte una miniatura de imagen desde el panel de navegación izquierdo.

CAPTURA DE PANTALLA

* Agregue un componente de imagen al lienzo y haga clic en **[!UICONTROL Examinar]** para abrir el cuadro de diálogo _[!UICONTROL Seleccionar Assets]_.

  En el cuadro de diálogo, puede elegir una imagen del repositorio seleccionado.

  Hay varias herramientas disponibles para ayudarle a localizar el recurso que necesita.

CAPTURA DE PANTALLA

* Cambie **[!UICONTROL Repositorio]** en la parte superior derecha.

* Haga clic en **[!UICONTROL Administrar recursos]** en la parte superior derecha para abrir el repositorio de Assets en otra pestaña del explorador y usar las herramientas de administración de AEM Assets.

* Haga clic en el selector _Tipo de vista_ en la parte superior derecha para cambiar la pantalla a **[!UICONTROL Vista de lista]**, **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de galería]** o **[!UICONTROL Vista de cascada]**.

* Haga clic en el icono _Orden_ para cambiar el orden de clasificación entre ascendente y descendente.

* Haga clic en la flecha de menú **[!UICONTROL Ordenar por]** para cambiar los criterios de ordenación a **[!UICONTROL Nombre]**, **[!UICONTROL Tamaño]** o **[!UICONTROL Modificado]**.

* Haga clic en el icono _Filtrar_ en la parte superior izquierda para filtrar los elementos mostrados según sus criterios.

* Introduzca texto en el campo Buscar para filtrar los elementos mostrados para buscar una coincidencia del nombre del recurso.

CAPTURA DE PANTALLA
