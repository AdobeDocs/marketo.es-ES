---
unique-page-id: 2951220
description: 'Creación de un informe de rendimiento de personas con columnas de plataforma móvil: Documentos de Marketo: documentación del producto'
title: Creación de un informe de rendimiento de personas con columnas de plataforma móvil
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Creación de un informe de rendimiento de personas con columnas de plataforma móvil {#build-a-people-performance-report-with-mobile-platform-columns}

Siga estos pasos para crear un informe de rendimiento de personas con columnas de plataforma móvil (iOS/Android).

## Crear listas inteligentes móviles {#create-mobile-smart-lists}

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Elija un programa.

   ![](assets/two-1.png)

1. En **Nuevo**, seleccione **Nuevo recurso local**.

   ![](assets/three-1.png)

1. Haga clic en **Lista inteligente**.

   ![](assets/four-1.png)

1. Escriba un nombre y haga clic en **Crear**.

   ![](assets/five-1.png)

1. Busque y arrastre el filtro Correo electrónico abierto al lienzo.

   ![](assets/six-1.png)

1. Establecer correo electrónico en **es cualquiera**.

   ![](assets/seven.png)

1. Haga clic en **Agregar restricción** y seleccione **Plataforma**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >En este ejemplo se ha utilizado el filtro Correo electrónico abierto. También puede utilizar el filtro Correo electrónico en el que se hizo clic, ya que tiene la restricción Plataforma.

1. Establezca Platform en **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Al menos una persona debe haber abierto uno de sus correos electrónicos en un dispositivo iOS para que la sugerencia automática de Marketo lo encuentre. Si no aparece, puede escribirlo manualmente y guardarlo.

   Ahora cree una segunda lista inteligente para la plataforma Android. Una vez hecho esto, pase a la siguiente sección.

## Creación de un informe de rendimiento de personas {#create-a-people-performance-report}

1. En Actividades de marketing, seleccione el programa que hospeda sus listas inteligentes **iOS** y **Android**.

   ![](assets/ten.png)

1. En **Nuevo**, seleccione **Nuevo recurso local**.

   ![](assets/eleven.png)

1. Haga clic en **Informe**.

   ![](assets/twelve.png)

1. Establezca el tipo en **Rendimiento de personas**.

   ![](assets/thirteen.png)

1. Haga clic en **Crear**.

   ![](assets/fourteen.png)

   ¡Lo estás haciendo genial! Ahora, a la siguiente sección.

## Agregar listas inteligentes móviles como columnas {#add-mobile-smart-lists-as-columns}

1. En el informe que acaba de crear, haga clic en **Configuración** y, a continuación, arrastre **Columnas personalizadas** al lienzo.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >De forma predeterminada, el informe Rendimiento de las personas examina los últimos 7 días. Puede cambiar el periodo de tiempo haciendo doble clic en él.

1. Busque y seleccione las listas inteligentes que creó anteriormente y haga clic en **Aplicar**.

   ![](assets/sixteen.png)

1. Haga clic en **Informe** para ejecutar el informe y ver los datos.

   ![](assets/seventeen.png)

   Bastante genial, ¿verdad? ¡Bien hecho!
