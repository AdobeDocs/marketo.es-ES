---
description: Obtenga información sobre los modelos de Audiencias predictivas y los factores que influyen. Utilice las perspectivas de IA para ajustar la segmentación y mejorar el rendimiento de la campaña.
title: Modelos y recomendaciones
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
TQID: https://experienceleague.adobe.com/ikS8VQJfQ9ndHrtDY5K8GYbNYwJjk1nYkuqxnwfcWPY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: b4dd41a7-ccf8-4e9d-918e-acaab534a307
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 234
ht-degree: 5%

---

# Modelos y recomendaciones {#models-and-insights}

El rendimiento de los modelos depende de la calidad y la integridad de los datos de entrada. Consulte el factor de influencia principal para cada uno de los modelos de IA de probabilidad. Además, consulte los factores principales que resultan en un registro de evento más alto/más bajo, asistencia a un evento o cancelaciones de suscripción.

>[!NOTE]
>
>Los comportamientos marcados con (+) influyen positivamente en las predicciones (y viceversa).

Utilice lo siguiente para evaluar el estado del modelo.

Vaya a la sección **[!UICONTROL Modelos y estado de datos]** en **[!UICONTROL Audiencias predictivas]** en el área de **[!UICONTROL Administración]** de Marketo Engage. Aquí se muestran todos los modelos y sus estados.

![Imagen uno](assets/models-and-insights-1.png)

* **Estado de formación**: indica si el modelo se está entrenando activamente (mejorando las predicciones). El entrenamiento se realiza automáticamente cada dos semanas. Cualquier modelo que esté _procesando_ puede tardar hasta 24 horas en finalizar. Para cualquier modelo _failed_, comuníquese con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.
* **Estado de puntuación**: indica si el modelo está calculando predicciones de forma activa (porcentajes de probabilidad) para los miembros del programa.
* **Rendimiento**: categorización del estado del modelo en función de la integridad y calidad de los datos (ver a continuación).
* **Complejidad de datos**: porcentaje de atributos de datos presentes/completos.
* **Calidad de los datos**: porcentaje de atributos que contienen datos útiles y buenos.
* **Última formación**: La fecha del modelo que es la mejor de la evaluación entre el modelo actual y el nuevo modelo que se forma cada dos semanas.
