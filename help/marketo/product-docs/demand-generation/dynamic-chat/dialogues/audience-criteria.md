---
description: 'Criterios de audiencia: Documentos de Marketo: documentación del producto'
title: Criterios de audiencia
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Criterios de audiencia {#audience-criteria}

Al igual que las listas inteligentes de Marketo, los atributos de criterios de audiencia le permiten definir la audiencia de destino. Puede dirigirse a personas conocidas o desconocidas mediante atributos inferidos, personales o de empresa (o una combinación de estos).

**Personas conocidas**

Hay _many_ combinaciones de atributos entre las que elegir. En este ejemplo estamos dirigiendo todos los objetivos **personas conocidas** en California que trabajan en una empresa con más de 50 empleados.

1. Tome el **Estado de la persona** y arrástrelo a la derecha.

   ![](assets/audience-criteria-1.png)

1. _Is_ está configurado de forma predeterminada. En el campo Seleccionar valores , escriba CA (también puede hacer clic en la lista desplegable y seleccionar en la lista).

   ![](assets/audience-criteria-2.png)

1. Tome el **Tamaño de la empresa** y arrástrela a donde dice _arrastre y suelte un atributo aquí_.

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >También puede elegir un atributo haciendo clic en su **+** icono.

1. Haga clic en la lista desplegable de operadores y seleccione **Bueno que**.

   ![](assets/audience-criteria-4.png)

1. Escriba 50 y haga clic en cualquier otra parte de la pantalla para guardar.

   ![](assets/audience-criteria-5.png)

¡Y eso es todo!

**Personas anónimas**

Existe una manera fácil de dirigirse específicamente a personas que aún no están en su base de datos. En este ejemplo, estamos segmentando todos **personas anónimas** situado en el área de Nueva York.

1. Tome el **Correo electrónico de persona** y arrástrelo a la derecha.

   ![](assets/audience-criteria-6.png)

1. Haga clic en la lista desplegable de operadores y seleccione **Está vacío**.

   ![](assets/audience-criteria-7.png)

1. Tome el **Estado afectado** y arrástrela a donde dice _arrastre y suelte un atributo aquí_.

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >Cuando alguien visita su sitio web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) las cookies y las coloca en el sistema. Buscamos su IP en una base de datos especial e infamos todo tipo de información buena.

1. _Is_ está configurado de forma predeterminada. En el campo Seleccionar valores , escriba NY (también puede hacer clic en la lista desplegable y seleccionar en la lista).

   ![](assets/audience-criteria-9.png)

## Agregar grupos {#add-groups}

También tiene la opción de agrupar atributos, en caso de que desee tener todos los atributos junto con &quot;todos o cualquiera&quot; de otro. Puede agregar varios grupos.

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

## Destino {#target}

Aquí es donde introduce las direcciones URL en las que desea que se muestre un cuadro de diálogo específico.

Formatos aceptables:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>El uso de un asterisco actúa como comodín global. So `https://*.website.com` colocaría el cuadro de diálogo en todas las páginas del sitio, incluidos los subdominios (por ejemplo: `support.website.com`). Y `https://website.com/folder/*` colocaría el cuadro de diálogo en todas las páginas del HTML en la carpeta siguiente (por ejemplo: en este caso, digamos que la carpeta es &quot;deportes&quot;, así que: website.com/sports/baseball.html, website.com/sports/football.html, etc.).

>[!MORELIKETHIS]
>
>* [Crear un cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Diseñador de secuencias](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Informes](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

