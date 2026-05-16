---
unique-page-id: 2951103
description: 'Notas de la versión, febrero de 2013, Documentos de Marketo: documentación del producto'
title: Notas de la versión, febrero de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
TQID: https://experienceleague.adobe.com/kfCE5HGsWooeFGDlCgr6zPrl7o7tIbx2-3NwUB9fxnY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 252
ht-degree: 1%

---

# Notas de la versión: febrero de 2013 {#release-notes-february}

La versión de febrero incluye una característica muy solicitada, compatibilidad con [!DNL Apple Safari] y otras pequeñas mejoras.

## Soporte oficial para [!DNL Apple Safari] {#official-support-for-apple-safari}

Las versiones más recientes de [!DNL Apple Safari] para Mac y [!DNL Windows] son totalmente compatibles para su uso con la administración de posibles clientes de Marketo. Nota: [!DNL Safari] en iOS no es totalmente compatible.

## Mejoras de Webhooks {#webhooks-enhancements}

Los webhooks se han mejorado para que escapen a los tokens en la dirección URL/carga útil y también pueden actualizar los campos de posibles clientes de Marketo analizando las respuestas XML/JSON de sistemas de terceros (no disponibles en [!DNL Spark SMB Edition]).

## Punto final de API de SOAP actualizado {#updated-soap-api-endpoint}

Se ha actualizado el extremo de la API de SOAP preferido, que se muestra en [!UICONTROL Administración] -> API de SOAP. Actualice las llamadas para utilizar este nuevo punto de conexión. Las llamadas de API al extremo anterior están obsoletas, pero seguirán funcionando. (La API de SOAP no está disponible en [!DNL Spark SMB Edition])

## Compatibilidad móvil con [!DNL Facebook] fichas {#mobile-support-for-facebook-tabs}

[!DNL Facebook] fichas publicadas desde Marketo detectarán dispositivos móviles y los enrutarán a una página de aterrizaje. Esto garantizará que el usuario obtenga el contenido adecuado en los dispositivos móviles que no admiten las fichas [!DNL Facebook] (disponibles en [!DNL Spark], [!DNL Standard], [!DNL Select SMB Editions] y [!DNL Marketo Social Marketing]).

## Próximamente: compatibilidad con varios modelos {#coming-soon-support-for-multiple-models}

Estamos sentando las bases para admitir varios modelos de ciclo de ingresos, votados #1 idea para RCA en la Comunidad, en una versión futura. En esta versión, verá algunos cambios, incluidos los filtros de listas inteligentes y Agregar opciones en Pasos de flujo, para admitir la selección de un modelo y una fase. También estamos moviendo los campos Etapa de ingresos de clientes potenciales y Modelo de ciclo de ingresos de clientes potenciales fuera de la pestaña de cuadrícula de clientes potenciales de listas inteligentes.
