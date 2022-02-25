---
description: Comportamiento esperado - Documentos de Marketo - Documentación del producto
title: Comportamiento esperado
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Comportamiento esperado {#expected-behavior}

En este artículo, encontrará información sobre el comportamiento esperado asociado con Predictive Audiences (PA).

## Consideraciones de privacidad y datos

* Todo el procesamiento de datos necesario para los modelos AI/ML tiene lugar en Norteamérica.
* Los modelos AI/ML no utilizan información específica sobre posibles clientes, como nombres o apellidos, sexo, correos electrónicos, números de contacto, etc. Los modelos solo utilizan atributos generales derivados de firmografías y registros de actividad.

**Para Predictive Audiences, se espera el siguiente comportamiento**

* Se puede acceder a AP tanto en la experiencia de Marketo Sky como en la de Marketo Classic. La disponibilidad de funciones específicas es la siguiente:
   * Filtros predictivos - [!DNL Sky/Classic]
   * Registros proyectados - [!DNL Sky/Classic]
   * Predicciones de probabilidad de nivel de posible cliente: [!DNL Sky/Classic]
   * Objetivos y seguimiento - [!DNL Sky] only
   * Información y recomendaciones: [!DNL Sky] only
* [Activación inicial](/help/marketo/product-docs/marketo-sky/getting-started-with-predictive-audiences.md) take **24 a 48 horas** para que todos los procesos se completen después de haber habilitado la PA. Verá todas las funcionalidades de Predictive Audiences y Predictive Filters en la interfaz, pero estas funciones pueden tardar hasta 24 horas en empezar a funcionar.
* **Las predicciones solo se generarán para las nuevas campañas que se creen después de activar la función.**

**Hay algunas consideraciones adicionales específicas de los filtros predictivos**:

* Los filtros de probabilidad de registro y asistencia solo se pueden usar con programas de eventos o seminarios web. Los filtros de igual parecido y de cancelación de suscripción se pueden utilizar en programas de correo electrónico, eventos y seminarios web.
* Puede aplicar filtros predictivos a una campaña inteligente incluso si el programa principal se ha creado antes de que se habiliten los filtros predictivos.
* Los filtros predictivos no están disponibles para campañas de déclencheur.
* Para ejecutar una campaña inteligente, es necesario usar filtros de probabilidad junto con otros filtros normales.
* La función Reglas guardadas no está disponible para su uso en campañas que contienen filtros predictivos.
* Puede usar **hasta 5** filtros predictivos en una lista inteligente.
* Los filtros predictivos pueden procesar un **máximo de 1 millón de posibles clientes cualificados**.
* Puede tener **hasta 50 programas activos** con filtros predictivos. Un programa activo es cualquier programa que utiliza filtros predictivos y que se ha programado al menos una vez.

## ¿Cuándo no están disponibles los registros proyectados?

Los registros proyectados no estarán disponibles en los siguientes casos de uso:

* si el programa se creó antes de agregar Predictive Audiences
* cuando los estados del programa no están asignados a estados del sistema
* cuando no haya miembros en el programa
* cuando no haya programas similares pasados en los últimos 6 meses que coincidan con los criterios requeridos
