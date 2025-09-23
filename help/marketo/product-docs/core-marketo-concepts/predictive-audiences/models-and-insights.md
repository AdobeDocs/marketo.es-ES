---
description: Modelos e información - Documentos de Marketo - Documentación del producto
title: Modelos y recomendaciones
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Modelos y recomendaciones {#models-and-insights}

El rendimiento de los modelos depende de la calidad y la integridad de los datos de entrada. Consulte el factor de influencia principal para cada uno de los modelos de IA de probabilidad. Además, consulte los factores principales que resultan en un registro de evento más alto/más bajo, asistencia a un evento o cancelaciones de suscripción.

>[!NOTE]
>
>Los comportamientos marcados con (+) influyen positivamente en las predicciones (y viceversa).

A continuación se muestra cómo evaluar la salud de su modelo.

Vaya a la sección **[!UICONTROL Modelos y estado de datos]** en **[!UICONTROL Audiencias predictivas]** en el área de **[!UICONTROL Administración]** de Marketo Engage. Aquí verá todos sus modelos y sus estados.

![Imagen uno](assets/models-and-insights-1.png)

* **Estado de formación**: indica si el modelo se está entrenando activamente (mejorando las predicciones). El entrenamiento se realiza automáticamente cada dos semanas. Cualquier modelo que esté _procesando_ puede tardar hasta 24 horas en finalizar. Para cualquier modelo _failed_, comuníquese con el [soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.
* **Estado de puntuación**: indica si el modelo está calculando predicciones de forma activa (porcentajes de probabilidad) para los miembros del programa.
* **Rendimiento**: categorización del estado del modelo en función de la integridad y calidad de los datos (ver a continuación).
* **Complejidad de datos**: porcentaje de atributos de datos presentes/completos.
* **Calidad de los datos**: porcentaje de atributos que contienen datos útiles y buenos.
* **Última formación**: La fecha del modelo que es la mejor de la evaluación entre el modelo actual y el nuevo modelo que se forma cada dos semanas.
