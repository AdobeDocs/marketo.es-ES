---
description: 'Criterios de audiencia: Documentos de Marketo: documentación del producto'
title: Criterios de audiencia
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: f71ac0398b3a93d2c46201a696dd41e6ccd89000
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# Criterios de audiencia {#audience-criteria}

Al igual que las listas inteligentes de Marketo, los atributos de criterios de audiencia le permiten definir la audiencia de destino. Puede dirigirse a personas conocidas o desconocidas mediante atributos inferidos, personales o de empresa (o una combinación de estos).

## Prioridad {#priority}

La prioridad determina qué cuadro de diálogo recibe un posible cliente en caso de que cumpla los requisitos para más de uno. Se establece al principio [crear el cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}. Para cambiar la prioridad de un cuadro de diálogo existente, ábralo y vaya a **Detalles del cuadro de diálogo** en la pestaña Criterios de audiencia .

![](assets/audience-criteria-1.png)

## Eventos {#events}

![](assets/audience-criteria-2.png)

Los eventos le permiten dirigirse a los visitantes en función de cuánto se desplazan o cuánto tiempo llevan en su página o sitio. En el siguiente ejemplo, estamos segmentando visitantes que hayan estado en una página específica durante más de 20 segundos.

1. Tome el **Tiempo en la página** y arrástrelo a la derecha.

   ![](assets/audience-criteria-3.png)

1. Establezca el tiempo &quot;Bueno que&quot; en 20 segundos.

   ![](assets/audience-criteria-4.png)

1. Añada la dirección URL de la página deseada en la página [Target](#target) para obtener más información.

   ![](assets/audience-criteria-5.png)

## Atributos {#attributes}

![](assets/audience-criteria-6.png)

**Personas conocidas**

Hay _many_ combinaciones de atributos entre las que elegir. En el ejemplo siguiente, estamos segmentando todos **personas conocidas** en California que trabajan en una empresa con más de 50 empleados.

1. Tome el **Estado de la persona** y arrástrelo a la derecha.

   ![](assets/audience-criteria-7.png)

1. _Is_ está configurado de forma predeterminada. En el campo Seleccionar valores , escriba CA (también puede hacer clic en la lista desplegable y seleccionar en la lista).

   ![](assets/audience-criteria-8.png)

1. Tome el **Tamaño de la empresa** y arrástrela a donde dice _arrastre y suelte un atributo aquí_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >También puede elegir un atributo haciendo clic en su **+** icono.

1. Haga clic en la lista desplegable de operadores y seleccione **Bueno que**.

   ![](assets/audience-criteria-10.png)

1. Escriba 50 y haga clic en cualquier otra parte de la pantalla para guardar.

   ![](assets/audience-criteria-11.png)

¡Y eso es todo!

**Personas anónimas**

Existe una manera fácil de dirigirse específicamente a personas que aún no están en su base de datos. En este ejemplo, estamos segmentando todos **personas anónimas** situado en el área de Nueva York.

1. Tome el **Correo electrónico de persona** y arrástrelo a la derecha.

   ![](assets/audience-criteria-12.png)

1. Haga clic en la lista desplegable de operadores y seleccione **Está vacío**.

   ![](assets/audience-criteria-13.png)

1. Tome el **Estado afectado** y arrástrela a donde dice _arrastre y suelte un atributo aquí_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Cuando alguien visita su sitio web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) las cookies y las coloca en el sistema. Buscamos su IP en una base de datos especial e infamos todo tipo de información buena.

1. _Is_ está configurado de forma predeterminada. En el campo Seleccionar valores , escriba NY (también puede hacer clic en la lista desplegable y seleccionar en la lista).

   ![](assets/audience-criteria-15.png)

## Agregar grupos {#add-groups}

También tiene la opción de agrupar atributos, en caso de que desee tener todos los atributos junto con &quot;todos o cualquiera&quot; de otro. Puede agregar varios grupos.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Destino {#target}

Aquí es donde introduce las direcciones URL en las que desea que se muestre un cuadro de diálogo específico. También tiene la opción de añadir exclusiones.

Formatos aceptables:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>El uso de un asterisco actúa como comodín global. So `https://*.website.com` colocaría el cuadro de diálogo en todas las páginas del sitio, incluidos los subdominios (por ejemplo: `support.website.com`). Y `https://website.com/folder/*` colocaría el cuadro de diálogo en todas las páginas del HTML en la carpeta siguiente (por ejemplo: en este caso, digamos que la carpeta es &quot;deportes&quot;, así que: website.com/sports/baseball.html, website.com/sports/football.html, etc.).

**Exclusiones**

Utilice exclusiones para asegurarse de que el cuadro de diálogo sí lo hace **not** aparecen en una página o área específica del sitio. Las exclusiones siguen el mismo formato que las inclusiones.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Crear un cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Diseñador de secuencias](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Informes](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

