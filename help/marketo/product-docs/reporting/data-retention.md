---
description: Descubra cómo las políticas de retención de datos de 25 meses y 90 días de Marketo afectan a los informes de Analytics, con un desglose por informe y sugerencias para retener los datos durante más tiempo.
title: Retención de datos
feature: Reporting
source-git-commit: 8eb9fd285e5dd055603579fbb5e7a4c4eb681172
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 5%

---

# Política de retención de datos de la actividad de Marketo: impacto en la creación de informes

Marketo conserva los datos de actividad de marketing de forma gradual. Los datos de actividad y pertenencia a campañas se almacenan durante un periodo móvil de 25 meses a partir de la fecha de actividad y los datos de actividad de gran volumen se conservan durante un periodo móvil de 90 días a partir de la fecha de actividad de forma predeterminada, que se puede ajustar por usuario. Más allá de estos períodos de retención, los datos ya no están disponibles a través de la interfaz de usuario de Marketo.

## Informes de Marketo Analytics

Debido a que los datos de actividad se conservan durante un máximo de 25 meses, algunos informes de Marketo Analytics se ven afectados por esta directiva, mientras que otros no. Los informes que obtienen datos de los registros de actividad de las personas solo mostrarán datos durante un máximo de 25 meses. Los informes que no hacen referencia a la actividad de la persona en absoluto se ven afectados.

Sin embargo, incluso los informes que no hacen referencia a la actividad de la persona de forma predeterminada pueden verse afectados si se añaden filtros a la lista inteligente del informe. Los filtros que hacen referencia a atributos de persona (información de los campos del registro de persona) no provocan ningún cambio en el informe. Los filtros que buscan actividades que la persona ha realizado solo pueden acceder a actividades dentro de la ventana de retención, por lo que si la actividad se produjo hace más tiempo que eso, los resultados del informe se alterarán.

La siguiente tabla resume cómo se comporta cada informe, incluidos los escenarios de filtro comunes.

## Referencia del informe

| Tipo de informe | Escenario de filtro | ¿Afectado por la política de retención? |
|---|---|---|
| **Informes del Explorador del Ciclo de Ingresos** | No hay filtros disponibles | No: Los usuarios del Explorador del ciclo de ingresos y de Analytics avanzado están totalmente exentos de estos límites de retención. Los datos RCE se envían de la noche a la mañana a un servidor de base de datos independiente que administra los informes RCE. Debido a que se aloja por separado y no en los registros de actividad de las personas, esta directiva no afecta a estos informes. El Explorador del ciclo de ingresos no extrae datos directamente de la base de datos de personas, por lo que los filtros no están disponibles. |
| **Informe de rendimiento de personas** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Personas por estado** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Personas por etapa de ingresos** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Analizador de rutas de éxito** | No incluye listas inteligentes | N/A |
| **Informe de influencia social** | No hay filtros de listas inteligentes | Sí |
| | Filtros en atributos de persona (por ejemplo: Nombre) | Sí |
| | Filtros en las actividades de personas en los últimos 25 meses | Sí |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Analizador de influencia de oportunidad** | No incluye listas inteligentes | No |
| **Rendimiento de correo electrónico** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Rendimiento de vínculo de correo electrónico** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Perspectivas de correo electrónico** | No utiliza listas inteligentes | No |
| **Rendimiento de correo electrónico de Insight de ventas** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Rendimiento de página de aterrizaje** | No hay filtros de listas inteligentes | No: los datos de Rendimiento de la página de aterrizaje se conservan indefinidamente y no están sujetos a la política de retención. |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | No |
| **Actividad de página web** | No hay filtros de listas inteligentes | Sí: sujeto al período de retención predeterminado de 90 días (ajustable por usuario) |
| | Filtros en atributos de persona (por ejemplo: Nombre) | Sí |
| | Filtros en las actividades de personas en los últimos 25 meses | Sí |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Actividad web de la compañía** | No hay filtros de listas inteligentes | Sí |
| | Filtros en atributos de persona (por ejemplo: Nombre) | Sí |
| | Filtros en las actividades de personas en los últimos 25 meses | Sí |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Rendimiento del programa** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Rendimiento de flujo de participación** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Analizador de programas** | No utiliza listas inteligentes | No |
| **Actividad de campaña** | No hay filtros de listas inteligentes | No |
| | Filtros en atributos de persona (por ejemplo: Nombre) | No |
| | Filtros en las actividades de personas en los últimos 25 meses | No |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |
| **Rendimiento de correo electrónico de Campaign** | No hay filtros de listas inteligentes | Sí |
| | Filtros en atributos de persona (por ejemplo: Nombre) | Sí |
| | Filtros en las actividades de personas en los últimos 25 meses | Sí |
| | Filtros en actividades de persona sin restricciones de fecha | Sí |

## Solución alternativa al informe

Muchos usuarios pueden considerar obsoletos los datos de actividad anteriores a la ventana de retención. Sin embargo, es posible que tenga un caso de uso en el que se necesite esta información. A continuación se indican las formas de conservar estos datos más allá del período de retención estándar.

## Exportación de datos

Marketo ofrece la [API de REST de extracción masiva](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/bulk-extract/bulk-extract), que le permite exportar actividades de personas y hospedarlas localmente. Una vez que los datos se extraen a través de la API, puede almacenarlos y ordenarlos según sea necesario para su caso de uso.

>[!TIP]
>
>Exporte los datos de su persona con regularidad, no solo una vez. Las actividades de la persona se conservan en un ciclo móvil de 25 meses. Establece un recordatorio para volver a exportar _antes de_ el final de ese periodo de tiempo de 25 meses.

## Uso de campos personalizados

Los valores de los campos de persona no se ven afectados por la política de retención de datos. Puede utilizar campañas inteligentes para rellenar campos personalizados con valores basados en las actividades que realizan sus recursos. Esto permite filtrar las personas por estos atributos de persona (no sujetos a la directiva de retención) en lugar de por las propias actividades (sujetas a la directiva de retención).

Una ventaja adicional de este enfoque es que la búsqueda por atributos de persona es más rápida que la búsqueda a través de los registros de actividad de la persona.
