---
unique-page-id: 2360309
description: Explicación de los espacios de trabajo y las particiones de persona - Documentos de Marketo - Documentación del producto
title: Explicación de espacios de trabajo y particiones de persona
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 91b6460bf0fa7fed85d48887ec38203f2ee7440f
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 3%

---

# Explicación de espacios de trabajo y particiones de persona {#understanding-workspaces-and-person-partitions}

## Espacios de trabajo {#workspaces}

>[!CAUTION]
>
>La configuración de los espacios de trabajo puede ser compleja. Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para averiguar si son adecuados para usted.

Los espacios de trabajo son áreas independientes en Marketo que contienen recursos de marketing como programas, páginas de aterrizaje, correos electrónicos y mucho más. Pueden ser utilizados por varias personas. Cada usuario tiene acceso a uno o más espacios de trabajo.

>[!NOTE]
>
>**Ejemplo**
>
>Algunas razones por las que puede utilizar un espacio de trabajo:
>
>* Geografía: los departamentos de marketing de Europa, Asia y América del Norte tienen cada uno un espacio de trabajo
>* Unidad de negocio: [!DNL Quicken], [!DNL Quickbooks] y [!DNL TurboTax] obtienen un área de trabajo
>
>En cada caso, la separación se debe a que los activos de marketing son completamente diferentes. Si comparten recursos de marketing, es posible que los espacios de trabajo no sean la herramienta adecuada para usted.

>[!NOTE]
>
>Aprenda a crear [un nuevo espacio de trabajo](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Uso compartido entre espacios de trabajo {#sharing-across-workspaces}

A continuación, se muestra cómo compartir recursos entre espacios de trabajo. Funciona igual para todo lo que desee compartir; este ejemplo muestra las segmentaciones.

>[!NOTE]
>
>La carpeta principal que contiene los recursos es la única carpeta que se puede compartir, no las carpetas secundarias.

1. Haga clic en **[!UICONTROL Base de datos]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Haga clic con el botón derecho en la carpeta Segmentación y luego haga clic en **[!UICONTROL Nueva carpeta]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Asigne un nombre a la carpeta y haga clic en **[!UICONTROL Crear]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Mueva los recursos que desee compartir a la carpeta.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **[!UICONTROL Compartir carpeta]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta y haga clic en **[!UICONTROL Guardar]**. El cuadro de diálogo Compartir carpeta sólo mostrará los espacios de trabajo para los que tenga permiso de visualización.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >La carpeta de origen ahora tendrá una pequeña flecha verde, que indica que se compartió. En el espacio de trabajo compartido, la carpeta tendrá un candado que indica que es de solo lectura.

Puede compartir estos elementos en espacios de trabajo.

* Plantillas de correo electrónico
* Plantillas de página de destino
* Modelos
* Campañas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentación](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Fragmentos

## Clonación en espacios de trabajo {#cloning-across-workspaces}

Para los recursos que no son plantillas, es mejor clonarlos como recursos locales dentro de un programa. Con el nivel de acceso adecuado, puede arrastrar y soltar estos recursos en otro espacio de trabajo:

* Programas
* Emails
* Páginas de destino
* Formularios

>[!IMPORTANT]
>
>Aunque todos los elementos enumerados arriba se pueden clonar en los espacios de trabajo, los mensajes de correo electrónico, los formularios y las páginas de aterrizaje _deben estar dentro de un programa_ en el momento de la clonación.

>[!NOTE]
>
>Al clonar recursos que tienen plantillas, estas deben compartirse con el espacio de trabajo de destino.

## Mover Assets a otros espacios de trabajo {#moving-assets-to-other-workspaces}

Para mover recursos a un nuevo espacio de trabajo, colóquelos en una carpeta y arrástrela al otro espacio de trabajo.

>[!NOTE]
>
>No se puede mover un programa que contenga miembros de un área de trabajo a otra.

## Particiones de personas {#person-partitions}

Las particiones de persona actúan como bases de datos independientes. Cada partición tiene su propia gente que no desduplica ni mezcla con otras particiones. Si cree que tiene un caso práctico empresarial que podría necesitar tener registros duplicados con la misma dirección de correo electrónico, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Puede asignar particiones de persona a [espacios de trabajo](create-a-new-workspace.md) con las siguientes configuraciones:

* partición de un espacio de trabajo a una persona (1:1)
* un espacio de trabajo para varias particiones de persona (1:x)
* varios espacios de trabajo para una partición de persona (x:1)

>[!NOTE]
>
>Razones por las que utilizaría una partición de persona:
>
>* Los espacios de trabajo no solo tienen recursos diferentes, sino que tampoco comparten personas
>* Desea duplicados por otros motivos comerciales

>[!CAUTION]
>
>Las particiones de persona no interactúan entre sí, por lo que debe tener cuidado al configurarlas.

>[!NOTE]
>
>Aprenda a [crear una partición de persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
