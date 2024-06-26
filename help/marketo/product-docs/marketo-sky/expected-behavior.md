---
description: 'Comportamiento esperado: documentos de Marketo, documentación del producto'
title: Comportamiento esperado
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Comportamiento esperado {#expected-behavior}

En este artículo, encontrará información sobre el comportamiento esperado asociado con Predictive Audiences (PA).

## Consideraciones sobre datos y privacidad

* Todo el procesamiento de datos requerido para los modelos AI/ML tiene lugar en Norteamérica.
* Los modelos de IA/ML no utilizan información de posible cliente específica, como nombre o apellidos, sexo, correos electrónicos, números de contacto, etc. Los modelos solo utilizan atributos generales derivados de los firmográficos y los registros de actividad.

**Para Predictive Audiences, se espera el siguiente comportamiento**

* Se puede acceder a PA tanto en Marketo Sky como en la experiencia de Marketo Classic. La disponibilidad de funciones específicas es la siguiente:
   * Filtros predictivos: [!DNL Sky/Classic]
   * Registros proyectados - [!DNL Sky/Classic]
   * Predicciones de probabilidad de nivel de posible cliente - [!DNL Sky/Classic]
   * Objetivos y seguimiento: [!DNL Sky] solamente
   * Información y recomendaciones: [!DNL Sky] solamente
* La activación inicial tarda **24 a 48 horas** para que todos los procesos se completen después de habilitar PA. Verá todas las funcionalidades de Audiencias predictivas y Filtros predictivos en la interfaz, pero estas funciones pueden tardar hasta 24 horas en empezar a funcionar.
* **Las predicciones solo se generarán para las nuevas campañas que se creen después de activar la función.**

**Hay algunas consideraciones adicionales específicas de los filtros predictivos**:

* Los filtros de Registro y Probabilidad de asistencia solo se pueden utilizar con programas de eventos o seminarios web. Los filtros de similitud y cancelación de suscripción se pueden utilizar en programas de correo electrónico, eventos y seminarios web.
* Puede aplicar filtros predictivos a una campaña inteligente incluso si el programa principal se crea antes de habilitar los filtros predictivos.
* Los filtros predictivos no están disponibles para campañas de déclencheur.
* Para ejecutar una campaña inteligente, es necesario utilizar filtros de probabilidad junto con otros filtros normales.
* La función Reglas guardadas no está disponible para su uso en campañas que contienen filtros predictivos.
* Puede utilizar **hasta 5** filtros predictivos en una lista inteligente.
* Los filtros predictivos pueden procesar una **máximo de 1 millón de posibles clientes cualificados**.
* Puede tener **hasta 50 programas activos** con filtros predictivos. Un programa activo es cualquier programa que utiliza filtros predictivos y que se ha programado al menos una vez.

## ¿Cuándo no están disponibles los registros proyectados?

Los registros proyectados no estarán disponibles en los siguientes casos de uso:

* si el programa se creó antes de que se agregara Audiencias predictivas
* cuando los estados de programa no están asignados a estados del sistema
* cuando no hay miembros en el programa
* cuando no haya programas similares pasados en los últimos 6 meses que coincidan con los criterios requeridos
