---
description: Estado del modelo y validez de los datos - Documentos de Marketo - Documentación del producto
title: Estado del modelo y validez de los datos
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Estado del modelo y validez de los datos {#model-health-and-data-validity}

El rendimiento de los modelos depende de la calidad y exhaustividad de los datos de entrada. Consulte el factor de influencia superior para cada uno de sus modelos de IA de probabilidad. Consulte también los factores principales que producen un registro de evento más alto/más bajo, asistencia al evento o cancelaciones de suscripción.

>[!NOTE]
>
>Los comportamientos marcados con (+) influyen positivamente en las predicciones (y viceversa).

Así es como evaluar el estado de su modelo.

Vaya a la **[!UICONTROL Modelos y estado de los datos]** sección bajo **[!UICONTROL Predictive Audiences]** en el **[!UICONTROL Administrador]** de Marketo Classic. Aquí podrá ver todos sus modelos y sus estados.

![Imagen uno](assets/model-health-and-data-validity-1.png)

* **Estado de la formación**: Indica si el modelo está formando activamente (mejorando las predicciones). La formación se realiza automáticamente cada 2 semanas. Cualquier modelo que _Procesamiento_ podría tardar hasta 24 horas en terminar. Para cualquier _Error_ modelos, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Estado de puntuación**: Indica si el modelo está calculando activamente las predicciones (porcentajes de probabilidad) para los miembros del programa.
* **Rendimiento**: categorización del estado del modelo basada en la integridad de los datos y la calidad de los datos (consulte a continuación).
* **Complejidad de datos**: Porcentaje de atributos de datos presentes/completados.
* **Calidad de los datos**: Porcentaje de atributos que contienen datos buenos y utilizables.