---
unique-page-id: 2951103
description: 'Notas de la versión, febrero de 2013, Documentos de Marketo: documentación del producto'
title: Notas de la versión, febrero de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Notas de la versión: febrero de 2013 {#release-notes-february}

La versión de febrero incluye una función muy solicitada, compatibilidad con Apple Safari y otras pequeñas mejoras.

## Soporte oficial para Apple Safari {#official-support-for-apple-safari}

Las versiones más recientes de Apple Safari para Mac y Windows son totalmente compatibles para su uso con la administración de posibles clientes de Marketo. Nota: Safari en iOS no es totalmente compatible.

## Mejoras de Webhooks {#webhooks-enhancements}

Los webhooks se han mejorado para que escapen a los tokens en la URL/carga útil y también pueden actualizar los campos de posibles clientes de Marketo analizando las respuestas XML/JSON de sistemas de terceros (no disponibles en Spark SMB Edition).

## SOAP Punto final de API de actualizado {#updated-soap-api-endpoint}

SOAP SOAP Se ha actualizado el extremo de la API de preferida, que se muestra en Administración -> API de. Actualice las llamadas para utilizar este nuevo punto de conexión. Las llamadas de API al extremo anterior están obsoletas, pero seguirán funcionando. SOAP (La API de no está disponible en Spark SMB Edition)

## Compatibilidad móvil con fichas de Facebook {#mobile-support-for-facebook-tabs}

Las pestañas de facebook publicadas desde Marketo detectan los dispositivos móviles y los dirigen a una página de aterrizaje. Esto garantizará que el usuario obtenga el contenido adecuado en los dispositivos móviles en los que no se admiten las pestañas de Facebook (disponibles en Spark, Standard, Select SMB Editions y Marketo Social Marketing).

## Próximamente: compatibilidad con varios modelos {#coming-soon-support-for-multiple-models}

Estamos sentando las bases para admitir varios modelos de ciclo de ingresos, votados #1 idea para RCA en la Comunidad, en una versión futura. En esta versión, notará algunos cambios, incluidos [filtros de listas inteligentes y Agregar opciones en pasos de flujo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) para admitir la selección de un modelo y una fase. También estamos moviendo los campos Etapa de ingresos de posibles clientes y Modelo de ciclo de ingresos de posibles clientes fuera de la pestaña de cuadrícula de posibles clientes de listas inteligentes.
