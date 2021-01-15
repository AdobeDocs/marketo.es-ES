---
unique-page-id: 2360309
description: Explicación de los espacios de trabajo y las particiones personales - Documentos de marketing - Documentación del producto
title: Explicación de los espacios de trabajo y las particiones personales
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---


# Explicación de los espacios de trabajo y las particiones personales {#understanding-workspaces-and-person-partitions}

## Espacios de trabajo {#workspaces}

>[!CAUTION]
>
>Los espacios de trabajo pueden ser complejos de configurar. Póngase en contacto con [Soporte técnico de marketing](https://nation.marketo.com/t5/Support/ct-p/Support) para averiguar si son los correctos para usted.

Los espacios de trabajo son áreas independientes en Marketing que contienen recursos de marketing como programas, páginas de aterrizaje, correos electrónicos y más. Pueden ser usadas por varias personas. Cada usuario tiene acceso a uno o varios espacios de trabajo.

>[!NOTE]
>
>**Ejemplo**
>
>Algunas razones por las que puede utilizar un espacio de trabajo:
>
>* Geografía: Los departamentos de mercadotecnia de Europa, Asia y América del Norte obtienen un espacio de trabajo
>* Unidad de negocio: Quicken, Quickbooks y TurboTax obtienen un espacio de trabajo

>
>
En cada caso, la separación se debe a que los recursos de marketing son completamente diferentes. Si comparten recursos de marketing, es posible que los espacios de trabajo no sean la herramienta adecuada para usted.

>[!NOTE]
>
>Obtenga información sobre cómo crear [un nuevo espacio de trabajo](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Uso compartido entre espacios de trabajo {#sharing-across-workspaces}

A continuación se muestra cómo compartir recursos entre espacios de trabajo. Funciona igual para cualquier cosa que quieras compartir; este ejemplo muestra las segmentaciones.

>[!NOTE]
>
>La carpeta principal que contiene los recursos es la única carpeta que se puede compartir, no las carpetas secundarias.

1. Cree una nueva carpeta.

   ![](assets/one.png)

1. Asigne un nombre a la carpeta que va a compartir.

   ![](assets/two.png)

1. Mueva los recursos que desee compartir a la carpeta.

   ![](assets/three.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **Compartir carpeta**.

   ![](assets/four.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta y haga clic en **Guardar**. El cuadro de diálogo Compartir carpeta solo mostrará los espacios de trabajo que tiene permiso para vista.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >La carpeta de origen tendrá ahora una pequeña flecha verde que indica que se ha compartido. En el espacio de trabajo compartido, la carpeta tendrá un cerrojo, que indica que es de sólo lectura.

Puede compartir estos elementos entre espacios de trabajo.

* Plantillas de correo electrónico
* Plantillas de página de aterrizaje
* Modelos
* Campañas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentaciones](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Recortes

## Clonación en espacios de trabajo {#cloning-across-workspaces}

Para los recursos que no son plantillas, es mejor clonar los recursos como recursos locales dentro de un programa.  Con el nivel de acceso adecuado, puede arrastrar y soltar estos recursos en otro espacio de trabajo:

* Programas
* Correos electrónicos
* páginas de aterrizaje
* Forms

>[!NOTE]
>
>Al clonar recursos que tienen plantillas, estas plantillas deben compartirse con el espacio de trabajo de destino.

## Mover recursos a otros espacios de trabajo {#moving-assets-to-other-workspaces}

Para mover recursos a un nuevo espacio de trabajo, colóquelos en una carpeta y arrastre la carpeta al otro espacio de trabajo.

>[!NOTE]
>
>No puede mover un programa que contenga miembros de un espacio de trabajo a otro.

## Particiones de persona {#person-partitions}

Las particiones personales actúan como bases de datos separadas. Cada partición tiene su propia gente que no desduplica ni combina con otras particiones. Si cree que tiene un caso de uso comercial que puede requerir tener registros de duplicados con la misma dirección de correo electrónico, póngase en contacto con [Asistencia técnica de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

Puede asignar particiones de persona a [espacios de trabajo](create-a-new-workspace.md) en las siguientes configuraciones:

* partición de un espacio de trabajo a una persona (1:1)
* un espacio de trabajo para muchas particiones personales (1:x)
* muchos espacios de trabajo en una partición de persona (x:1)

>[!NOTE]
>
>Razones por las que usaría una partición de persona:
>
>* Los espacios de trabajo no solo tienen recursos diferentes, sino que tampoco comparten ninguna persona
>* Desea duplicados por otras razones comerciales


>[!CAUTION]
>
>Las particiones personales no interactúan entre sí, por lo tanto tenga cuidado al configurarlas.

>[!NOTE]
>
>Obtenga información sobre cómo [crear una partición de persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
