---
unique-page-id: 2359502
description: 'Usar la prueba A/B "Correo electrónico completo": Documentos de Marketo: Documentación del producto'
title: Usar la prueba A/B "Correo electrónico completo"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Usar la prueba A/B &quot;Correo electrónico completo&quot; {#use-whole-email-a-b-testing}

Puede probar fácilmente los correos electrónicos A/B. Una buena prueba es la **Correo electrónico completo** prueba. Así es como configurarlo.

>[!PREREQUISITES]
>
>[Agregar una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. En el mosaico Correo electrónico , con el correo electrónico seleccionado, haga clic en **Agregar prueba A/B**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Se abre una nueva ventana. Haga clic en el **Tipo de prueba** y seleccione **Correos electrónicos completos**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Si tiene información de prueba anterior (como una prueba de sujeto), puede hacer clic en **Restablecer prueba**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Seleccione su primer correo electrónico.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Haga clic en **Agregar** para aplicar el correo electrónico.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Puede añadir varios correos electrónicos. Sin embargo, si agrega demasiados, puede ralentizar el proceso de prueba.

1. Seleccione su segundo correo electrónico.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Haga clic en **Agregar** para aplicar el segundo correo electrónico. Arrastre el control deslizante para elegir el porcentaje de audiencia que desea que reciba la prueba A/B y haga clic en **Siguiente**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Las diferentes variaciones se envían a partes iguales del **Probar tamaño de muestra**.

   >[!CAUTION]
   >
   >**Le recomendamos que evite establecer el tamaño de la muestra en 100%**. Si utiliza una lista estática, si establece el tamaño de la muestra en 100 %, el correo electrónico se envía a todos los miembros de la audiencia y el ganador no va a nadie. Si está utilizando un **smart** , si establece el tamaño de la muestra en 100 %, el correo electrónico se envía a todos los miembros de la audiencia _en ese momento_. Cuando el programa de correo electrónico se ejecute de nuevo en una fecha posterior, cualquier persona nueva que cumpla los requisitos para la lista inteligente también recibirá el correo electrónico, ya que ahora está incluido en la audiencia.

   Bueno, casi estamos ahí. Ahora necesitamos [definir los criterios del ganador de la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
