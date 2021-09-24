---
unique-page-id: 2951103
description: 'Notas de la versión, febrero de 2013: Documentación del producto de Marketo'
title: Notas de la versión, febrero de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Notas de la versión: Febrero de 2013 {#release-notes-february}

La versión de febrero incluye una función muy solicitada, compatibilidad con Apple Safari y otras pequeñas mejoras.

## Compatibilidad oficial con Apple Safari {#official-support-for-apple-safari}

Las versiones más recientes de Apple Safari para Mac y Windows son totalmente compatibles para su uso con Marketo Lead Management. Nota: Safari en iOS no es totalmente compatible.

## Mejoras en los Webhooks {#webhooks-enhancements}

Webhooks se mejora para escapar de los tokens en la URL/carga útil y también puede actualizar los campos de posible cliente de Marketo analizando las respuestas XML/JSON de sistemas de terceros (no disponible en la Spark SMB Edition).

## Punto final de API de SOAP actualizado {#updated-soap-api-endpoint}

Se ha actualizado el extremo preferido de la API SOAP, que se muestra en Administración -> API SOAP. Actualice las llamadas para utilizar este nuevo punto final. Las llamadas de API al punto final antiguo están obsoletas, pero seguirán funcionando. (La API de SOAP no está disponible en Spark SMB Edition)

## Compatibilidad con dispositivos móviles para las fichas de Facebook {#mobile-support-for-facebook-tabs}

Las pestañas de facebook publicadas desde Marketo detectarán dispositivos móviles y los dirigirán a una página de aterrizaje. Esto garantizará que el usuario obtenga el contenido correcto en los dispositivos móviles en los que no se admiten las pestañas de Facebook (disponibles en Spark, Standard, Select SMB Editions y Marketo Social Marketing).

## Próximamente: Compatibilidad con varios modelos {#coming-soon-support-for-multiple-models}

Estamos sentando las bases para apoyar varios modelos de ciclo de ingresos, votado la idea número 1 para RCA en la Comunidad, en una futura versión. En esta versión, observará algunos cambios, como [filtros de lista inteligente y Agregar opciones en pasos de flujo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) para admitir la selección de un modelo y una etapa. También se están moviendo los campos Fase de ingresos de posible cliente y Modelo de ciclo de ingresos de posible cliente fuera de la ficha Cuadrícula de posibles clientes de lista inteligente .
