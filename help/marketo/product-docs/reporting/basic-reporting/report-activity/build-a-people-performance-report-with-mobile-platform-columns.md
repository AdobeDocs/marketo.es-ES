---
unique-page-id: 2951220
description: 'Creación de un informe de rendimiento de personas con columnas de plataforma móvil: Documentos de Marketo: documentación del producto'
title: Generar un informe de rendimiento de personas con columnas de plataforma móvil
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 6%

---

# Generar un informe de rendimiento de personas con columnas de plataforma móvil {#build-a-people-performance-report-with-mobile-platform-columns}

Siga estos pasos para crear un informe de rendimiento de personas con columnas de plataforma móvil (iOS/Android).

## Crear listas inteligentes móviles {#create-mobile-smart-lists}

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/ma.png)

1. Elija un programa.

   ![](assets/two-1.png)

1. En **[!UICONTROL Nuevo]**, seleccione **[!UICONTROL Nuevo recurso local]**.

   ![](assets/three-1.png)

1. Haga clic en **[!UICONTROL Lista inteligente]**.

   ![](assets/four-1.png)

1. Escriba un nombre y haga clic en **[!UICONTROL Crear]**.

   ![](assets/five-1.png)

1. Busque y arrastre el filtro [!UICONTROL Correo electrónico abierto] al lienzo.

   ![](assets/six-1.png)

1. Establecer correo electrónico en **[!UICONTROL es cualquiera]**.

   ![](assets/seven.png)

1. Haga clic en **[!UICONTROL Agregar restricción]** y seleccione **[!UICONTROL Plataforma]**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >En este ejemplo usamos el filtro [!UICONTROL Correo electrónico abierto]. También puede usar el filtro [!UICONTROL Correo electrónico en el que se hizo clic] porque tiene la restricción de plataforma.

1. Establezca [!UICONTROL Platform] en **[!UICONTROL iOS]**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Al menos una persona debe haber abierto uno de sus correos electrónicos en un dispositivo iOS para que la sugerencia automática de Marketo lo encuentre. Si no aparece, puede escribirlo manualmente y guardarlo.

   Ahora cree una segunda lista inteligente para la plataforma Android. Una vez hecho esto, pase a la siguiente sección.

## Creación de un informe de rendimiento de personas {#create-a-people-performance-report}

1. En Actividades de marketing, seleccione el programa que hospeda sus listas inteligentes **[!UICONTROL iOS]** y **[!UICONTROL Android]**.

   ![](assets/ten.png)

1. En **[!UICONTROL Nuevo]**, seleccione **[!UICONTROL Nuevo recurso local]**.

   ![](assets/eleven.png)

1. Haga clic en **[!UICONTROL Informe]**.

   ![](assets/twelve.png)

1. Establezca el tipo en **[!UICONTROL Rendimiento de personas]**.

   ![](assets/thirteen.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/fourteen.png)

   ¡Lo estás haciendo genial! Ahora, a la siguiente sección.

## Agregar listas inteligentes móviles como columnas {#add-mobile-smart-lists-as-columns}

1. En el informe que acaba de crear, haga clic en **[!UICONTROL Configuración]** y, a continuación, arrastre **[!UICONTROL Columnas personalizadas]** al lienzo.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >De forma predeterminada, el informe Rendimiento de las personas examina los últimos 7 días. Puede cambiar el periodo de tiempo haciendo doble clic en él.

1. Busque y seleccione las listas inteligentes que creó anteriormente y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/sixteen.png)

1. Haga clic en **[!UICONTROL Informe]** para ejecutar el informe y ver los datos.

   ![](assets/seventeen.png)

   Bastante genial, ¿verdad? ¡Bien hecho!
