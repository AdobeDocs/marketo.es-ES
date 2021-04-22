---
unique-page-id: 2360309
description: 'Explicación de los espacios de trabajo y las particiones de persona: Documentos de Marketo: Documentación del producto'
title: Explicación de los espacios de trabajo y las particiones de persona
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Explicación de los espacios de trabajo y las particiones de persona {#understanding-workspaces-and-person-partitions}

## Espacios de trabajo {#workspaces}

>[!CAUTION]
>
>Los espacios de trabajo pueden ser complejos de configurar. Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para averiguar si son adecuados para usted.

Los espacios de trabajo son áreas independientes en Marketo que contienen recursos de marketing como programas, páginas de aterrizaje, correos electrónicos y más. Pueden utilizarlas varias personas. Cada usuario tiene acceso a uno o más espacios de trabajo.

>[!NOTE]
>
>**Ejemplo**
>
>Algunas razones por las que puede utilizar un espacio de trabajo:
>
>* Geografía: Los departamentos de marketing de Europa, Asia y Norteamérica disponen de un espacio de trabajo
>* Unidad empresarial: Quicken, Quickbooks y TurboTax cuentan con un espacio de trabajo

>
>
En cada caso, la separación se debe a que los recursos de marketing son completamente diferentes. Si comparten recursos de marketing, es posible que los espacios de trabajo no sean la herramienta adecuada para usted.

>[!NOTE]
>
>Aprenda a crear [crear un nuevo espacio de trabajo](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Uso compartido entre espacios de trabajo {#sharing-across-workspaces}

A continuación se muestra cómo compartir recursos entre espacios de trabajo. Funciona igual para cualquier cosa que desee compartir; en este ejemplo se muestran las segmentaciones.

>[!NOTE]
>
>La carpeta principal que contiene los recursos es la única carpeta que se puede compartir, no las carpetas secundarias.

1. Cree una nueva carpeta.

   ![](assets/one.png)

1. Asigne un nombre a la carpeta que va a compartir.

   ![](assets/two.png)

1. Mueva los recursos que desea compartir a la carpeta .

   ![](assets/three.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **Compartir carpeta**.

   ![](assets/four.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta y haga clic en **Guardar**. El cuadro de diálogo Compartir carpeta solo mostrará los espacios de trabajo que tenga permiso para ver.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >La carpeta de origen ahora tendrá una pequeña flecha verde que indica que se compartió. En el espacio de trabajo compartido, la carpeta tendrá un candado que indica que es de solo lectura.

Puede compartir estos elementos entre espacios de trabajo.

* Plantillas de correo electrónico
* Plantillas de página de aterrizaje
* Modelos
* Campañas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentaciones](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Fragmentos

## Clonación entre espacios de trabajo {#cloning-across-workspaces}

Para los recursos que no son plantillas, es mejor clonarlos como recursos locales dentro de un programa.  Con el nivel de acceso adecuado, puede arrastrar y soltar estos recursos en otro espacio de trabajo:

* Programas
* Correos electrónicos
* Páginas de aterrizaje
* Forms

>[!NOTE]
>
>Al clonar recursos que tienen plantillas, estas plantillas deben compartirse con el espacio de trabajo de destino.

## Mover recursos a otros espacios de trabajo {#moving-assets-to-other-workspaces}

Para mover recursos a un nuevo espacio de trabajo, colóquelos en una carpeta y arrastre la carpeta al otro espacio de trabajo.

>[!NOTE]
>
>No se puede mover un programa que contenga miembros de un espacio de trabajo a otro.

## Particiones de personas {#person-partitions}

Las particiones de persona actúan como bases de datos independientes. Cada partición tiene su propia gente que no desduplica ni combina con otras particiones. Si cree que tiene un caso de uso empresarial que puede requerir tener registros duplicados con la misma dirección de correo electrónico, póngase en contacto con el [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Puede asignar particiones de persona a [espacios de trabajo](create-a-new-workspace.md) en las siguientes configuraciones:

* partición de espacio de trabajo a una persona (1:1)
* un espacio de trabajo para muchas particiones de persona (1:x)
* muchos espacios de trabajo en una partición de persona (x:1)

>[!NOTE]
>
>Razones por las que usaría una partición de persona:
>
>* Sus espacios de trabajo no solo tienen recursos diferentes, sino que tampoco comparten ninguna persona
>* Desea duplicados por otros motivos comerciales


>[!CAUTION]
>
>Las particiones de persona no interactúan entre sí, por lo que debe tener cuidado al configurarlas.

>[!NOTE]
>
>Aprenda a [crear una partición de persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
