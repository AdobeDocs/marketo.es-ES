---
description: Obtenga información acerca del comportamiento esperado para Predictive Audiences en Marketo Sky. Comprenda la privacidad de datos, el tiempo de activación y los límites de filtro.
title: Comportamiento esperado
hide: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
TQID: https://experienceleague.adobe.com/MtbP3re-wJJg-x1NJsdmXFLSEY8IdIMuloYhSRGploQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 394
ht-degree: 1%

---

# Comportamiento esperado {#expected-behavior}

En este artículo, encontrarás información sobre el comportamiento esperado asociado con [!UICONTROL Predictive Audiences] (PA).

## Consideraciones sobre datos y privacidad

* Todo el procesamiento de datos requerido para los modelos AI/ML tiene lugar en Norteamérica.
* Los modelos de IA/ML no utilizan información de posible cliente específica, como nombre o apellidos, sexo, correos electrónicos, números de contacto, etc. Los modelos solo utilizan atributos generales derivados de los firmográficos y los registros de actividad.

**Para [!UICONTROL Audiencias predictivas], se espera el siguiente comportamiento**

* Se puede acceder a la PA tanto en [!DNL Marketo Sky] como en la experiencia [!DNL Marketo Classic]. La disponibilidad de funciones específicas es la siguiente:
   * Filtros predictivos: [!DNL Sky/Classic]
   * Registros proyectados - [!DNL Sky/Classic]
   * Predicciones de probabilidad de nivel de posible cliente - [!DNL Sky/Classic]
   * Seguimiento y objetivos: solo [!DNL Sky]
   * Información y recomendaciones - [!DNL Sky] solamente
* La activación inicial tarda de **24 a 48 horas** en completarse para todos los procesos una vez habilitada la PA. Verá todas las funcionalidades de Audiencias predictivas y Filtros predictivos en la interfaz, pero estas funciones pueden tardar hasta 24 horas en empezar a funcionar.
* **Solo se generarán predicciones para las nuevas campañas que se creen después de activar la característica.**

**Hay algunas consideraciones adicionales específicas de los filtros predictivos**:

* Los filtros de Registro y Probabilidad de asistencia solo se pueden utilizar con programas de eventos o seminarios web. Los filtros de similitud y cancelación de suscripción se pueden utilizar en programas de correo electrónico, eventos y seminarios web.
* Puede aplicar filtros predictivos a una campaña inteligente incluso si el programa principal se crea antes de habilitar los filtros predictivos.
* Los filtros predictivos no están disponibles para campañas de déclencheur.
* Para ejecutar una campaña inteligente, es necesario utilizar filtros de probabilidad junto con otros filtros normales.
* La función Reglas guardadas no está disponible para su uso en campañas que contienen filtros predictivos.
* Puede usar **hasta 5** filtros predictivos en una lista inteligente.
* Los filtros predictivos pueden procesar un **máximo de 1 millón de posibles clientes calificados**.
* Puede tener **hasta 50 programas activos** con filtros predictivos. Un programa activo es cualquier programa que utiliza filtros predictivos y que se ha programado al menos una vez.

## ¿Cuándo no están disponibles los registros proyectados?

Los registros proyectados no estarán disponibles en los siguientes casos de uso:

* si el programa se creó antes de que se agregara Audiencias predictivas
* cuando los estados de programa no están asignados a estados del sistema
* cuando no hay miembros en el programa
* cuando no haya programas similares pasados en los últimos 6 meses que coincidan con los criterios requeridos
