---
unique-page-id: 557339
description: Buscar y combinar personas de Duplicado - Documentos de marketing - Documentación del producto
title: Buscar y combinar personas de Duplicado
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---


# Buscar y combinar personas de Duplicado {#find-and-merge-duplicate-people}

El marketing elimina automáticamente los duplicados cuando entran nuevos usuarios en el sistema. Sin embargo, es posible que su CRM haya enviado inicialmente duplicados a Marketing. Así es como combinarlos.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Marketo no desduplicará automáticamente con una sincronización de Salesforce o Microsoft Dynamics, ni cuando introduzca personas manualmente.

>[!PREREQUISITES]
>
>Encontrar y combinar duplicados implica el uso de listas [inteligentes](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)integradas/del sistema.

## Buscar Duplicados {#find-duplicates}

1. Vaya al área **Base de datos** .

   ![](assets/db.png)

   >[!CAUTION]
   >
   >Es posible que la combinación de personas en Marketing no funcione si utiliza una cuenta de persona de Salesforce. Si es posible, combine los registros en Salesforce.

1. Seleccione la lista inteligente del sistema de **Posibles** **Duplicados** y haga clic en la ficha **Personas** .

   ![](assets/two.png)

   >[!NOTE]
   >
   >También puede [buscar personas Duplicados con lógica](find-duplicate-people-with-custom-logic.md)personalizada.

## Combinar personas manualmente {#merge-people-manually}

>[!CAUTION]
>
>Al combinar personas, si la persona perdedora tiene un objeto personalizado de marketing, **no se volverá** a asociar con la persona ganadora. Vuelva a propagar el objeto personalizado antes de realizar la combinación.

Para seleccionar los duplicados, mantenga presionada la tecla Ctrl/Cmd y haga clic en Combinar personas.
![](assets/three.png)

>[!TIP]
>
>Podría tener dos o más duplicados para la misma persona; selecciónelos todos a la vez.

1. Verá los valores entre los registros que *no* coinciden. Seleccione el valor que desee conservar para cada campo. Haga clic en **Combinar** cuando termine. Si no desea ningún valor, puede marcar **Personalizado** e introducir un valor de su elección.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Al combinar personas manualmente, la primera persona seleccionada será la &quot;ganadora&quot;. Así que en la ficha Personas si se combinan los ID de registro 198 y 199, y se hace clic en 1999 primero, 199 será el ID de registro de las personas combinadas. Esto también se aplica si se combinan más de dos registros.

   >[!TIP]
   >
   >Combinar es mejor que eliminar. Conservará todo el historial (visitas a páginas, clics en vínculos, aperturas de correo electrónico, rellenos de formularios, etc.).

## Efecto en Salesforce {#effect-in-salesforce}

Si tiene la integración de Salesforce, hay algunas notas sobre el efecto de Fusionar leads en Salesforce.

    * Cuando se combinan solo los posibles clientes o solo los contactos, se combinan según las reglas normales de Salesforce.
    * Al combinar leads y contactos, todos los leads se convierten en Contactos antes de combinarse según las reglas normales de Salesforce.

Para conocer los detalles del comportamiento de Salesforce al combinar posibles clientes o contactos, consulte los siguientes documentos de Salesforce:

    * [Fusión de leads de Duplicado](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
    * [Fusión de contactos de Duplicado](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Fusión masiva {#bulk-merging}

Si tiene demasiados duplicados para combinar manualmente, póngase en contacto con el administrador de éxito del cliente para analizar sus opciones.

¡Super! Si está conectado a un CRM, los registros se combinarán allí según las reglas siguientes.