---
title: esperado-comportamiento
description: Comportamiento esperado
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---


# Comportamiento esperado

<br> 

En este artículo, encontrará información sobre el comportamiento esperado asociado con Audiencias predictivas (PA).

## Consideraciones sobre datos y privacidad

* Todo el procesamiento de datos necesario para los modelos AI/ML tiene lugar en Norteamérica.
* Los modelos de AI/ML no utilizan información específica sobre los posibles clientes, como nombres o apellidos, sexo, correos electrónicos, números de contacto, etc. Los modelos solo utilizan atributos generales derivados de firmografías y registros de actividad.

## En Audiencias predictivas, puede esperarse el siguiente comportamiento:

* Se puede acceder a la API tanto en la experiencia de Marketo Sky como en la de marketing clásico. La disponibilidad de funciones específicas es la siguiente:
   * Filtros predictivos - [!DNL Sky/Classic]
   * Registros proyectados - [!DNL Sky/Classic]
   * Predicciones de probabilidad de nivel de posible cliente: [!DNL Sky/Classic]
   * Objetivos y seguimiento: solo [!DNL Sky]
   * Perspectivas y recomendaciones: [!DNL Sky] solamente
* [La ](/help/sky/getting-started-with-predictive-audiences.md) activación inicial tarda entre **24 y 48** horas en completar todos los procesos una vez que se ha habilitado PA. Verá todas las funciones de Audiencias predictivas y Filtros predictivos en la interfaz, pero estas funciones pueden tardar hasta 24 horas en empezar a funcionar.
* **Las predicciones solo se generarán para las nuevas campañas que se creen después de activar la función.**

## Existen algunas consideraciones adicionales específicas de los filtros predictivos:

* Los filtros de probabilidad de registro y asistencia solo se pueden usar con programas de evento o seminario web. Los filtros de búsqueda y cancelación de suscripción se pueden utilizar en programas de correo electrónico, evento y seminario web.
* Puede aplicar filtros predictivos a una campaña inteligente incluso si se crea el programa principal antes de habilitar los filtros predictivos.
* Los filtros predictivos no están disponibles para campañas desencadenadoras.
* Para ejecutar una campaña inteligente, es necesario utilizar filtros de probabilidad junto con otros filtros normales.
* La función Reglas guardadas no está disponible para su uso en campañas que contienen filtros predictivos.
* Puede utilizar **hasta 5** filtros predictivos en una lista inteligente.
* Los filtros predictivos pueden procesar un **máximo de 1 millón de posibles clientes calificados**.
* Puede tener **hasta 50 programas activos** con filtros predictivos. Un programa activo es cualquier programa que utiliza filtros predictivos y que se ha programado al menos una vez.

## ¿Cuándo no están disponibles los registros proyectados?

Los registros proyectados no estarán disponibles en los siguientes casos de uso:

* si el programa se creó antes de agregar Audiencias predictivas
* cuando los estados de programa no están asignados a los estados del sistema
* cuando no haya miembros en el programa
* cuando no haya programas similares pasados en los últimos 6 meses que coincidan con los criterios requeridos
