---
unique-page-id: 2360309
description: Descubra cómo los espacios de trabajo organizan los recursos de marketing y cómo las particiones de persona actúan como bases de datos independientes.
title: Explicación de espacios de trabajo y particiones de personas
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 97%

---

# Explicación de espacios de trabajo y particiones de personas {#understanding-workspaces-and-person-partitions}

## Espacios de trabajo {#workspaces}

>[!CAUTION]
>
>La configuración de los espacios de trabajo puede ser compleja. Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para averiguar si son adecuados para usted.

Los espacios de trabajo son áreas independientes en Marketo que contienen recursos de marketing como programas, páginas de aterrizaje, correos electrónicos y mucho más. Pueden ser utilizados por varias personas. Cada usuario tiene acceso a uno o más espacios de trabajo.

>[!NOTE]
>
>**Ejemplo**
>
>Algunas razones por las que podría utilizar un espacio de trabajo:
>
>* Geografía: los departamentos de marketing de Europa, Asia y América del Norte tienen cada uno un espacio de trabajo
>* Unidad de negocio: [!DNL Quicken], [!DNL Quickbooks] y [!DNL TurboTax] tienen cada uno un espacio de trabajo
>
>En cada caso, la separación se debe a que los recursos de marketing son completamente diferentes. Si comparten recursos de marketing, es posible que los espacios de trabajo no sean la herramienta adecuada para usted.

>[!NOTE]
>
>Obtenga información sobre cómo [crear un nuevo espacio de trabajo](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Uso compartido entre espacios de trabajo {#sharing-across-workspaces}

A continuación se indica cómo compartir recursos entre varios espacios de trabajo. Funciona igual con todo lo que desee compartir; este ejemplo muestra segmentaciones.

>[!NOTE]
>
>La carpeta principal que contiene los recursos es la única carpeta que se puede compartir, no las carpetas secundarias.

1. Haga clic en la **[!UICONTROL base de datos]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Haga clic con el botón derecho en la carpeta Segmentación y luego haga clic en **[!UICONTROL Nueva carpeta]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Póngale un nombre a la carpeta y haga clic en **[!UICONTROL Crear]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Mueva los recursos que desee compartir a esa carpeta.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **[!UICONTROL Compartir carpeta]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta y haga clic en **[!UICONTROL Guardar]**. El cuadro de diálogo Compartir carpeta solo muestra los espacios de trabajo para los que tenga permiso de visualización.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >La carpeta de origen ahora tendrá una pequeña flecha verde que indica que es una carpeta compartida. En el espacio de trabajo compartido, la carpeta tiene un candado para indicar que es de solo lectura.

Puede compartir estos elementos en varios espacios de trabajo.

* Plantillas de correo electrónico
* Plantillas de página de aterrizaje
* Modelos
* Campañas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentación](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Fragmentos

## Clonación entre espacios de trabajo {#cloning-across-workspaces}

En el caso de recursos que no sean plantillas, es mejor clonarlos como recursos locales dentro de un programa. Con el nivel de acceso adecuado, puede arrastrar y soltar estos recursos en otro espacio de trabajo:

* Programas
* Correos electrónicos
* Páginas de aterrizaje
* Formularios

>[!IMPORTANT]
>
>Aunque todos los elementos enumerados anteriormente se pueden clonar entre los espacios de trabajo, los mensajes de correo electrónico, los formularios y las páginas de aterrizaje _deben estar dentro de un programa_ en el momento de la clonación.

>[!NOTE]
>
>Al clonar recursos que tienen plantillas, dichas plantillas deben compartirse con el espacio de trabajo de destino.

## Mover recursos a otros espacios de trabajo {#moving-assets-to-other-workspaces}

Para mover recursos a un nuevo espacio de trabajo, colóquelos en una carpeta y arrastre la carpeta hasta el otro espacio de trabajo.

>[!NOTE]
>
>No puede mover un programa que contenga miembros de un espacio de trabajo a otro.

## Particiones de personas {#person-partitions}

Las particiones de personas actúan como bases de datos independientes. Cada partición tiene su propio grupo de personas que no se desduplica ni se mezcla con otras particiones. Si cree que tiene un caso de uso empresarial que podría necesitar tener registros duplicados con la misma dirección de correo electrónico, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Puede asignar particiones de personas a [espacios de trabajo](create-a-new-workspace.md) con las siguientes configuraciones:

* un espacio de trabajo a una partición de personas (1:1)
* un espacio de trabajo a muchas particiones de personas (1:x)
* varios espacios de trabajo a una partición de personas (x:1)

>[!NOTE]
>
>Razones por las que utilizaría una partición de personas:
>
>* Los espacios de trabajo no solo tienen recursos diferentes, tampoco comparten personas
>* Desea duplicados por otros motivos empresariales

>[!CAUTION]
>
>Las particiones de personas no interactúan entre sí, por lo que debe tener cuidado al configurarlas.

>[!NOTE]
>
>Obtenga información acerca de cómo [crear una partición de personas](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
