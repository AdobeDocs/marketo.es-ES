---
unique-page-id: 10100266
description: Información general sobre las actividades personalizadas para rastrear acciones de personas específicas del negocio, en qué se diferencian de los objetos personalizados y la configuración en dos pasos de la creación de la actividad y la implementación de la API.
title: Explicación de actividades personalizadas
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
TQID: https://experienceleague.adobe.com/QwH82DomS1BDHbK3wfoP14N8xDBKZ28gOLyZ-L8fAeY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 286
ht-degree: 8%

---

# Explicación de actividades personalizadas {#understanding-custom-activities}

Realice un seguimiento de una acción que una persona ha realizado que sea específica a su negocio con actividades personalizadas.

## Qué son las actividades {#what-are-activities}

Existen varias formas en las que una persona puede interactuar con su organización. Pueden visitar el sitio web de su empresa, asistir a una de sus ferias comerciales o hacer clic en un vínculo de un correo electrónico enviado a ellos. Estas acciones son actividades y, independientemente de las acciones que realicen, Marketo las captura para que su equipo de marketing pueda comprender mejor cómo enviarles una comunicación oportuna y relevante.

## Actividades personalizadas {#custom-activities}

Las actividades personalizadas le ayudan a rastrear una actividad que no está relacionada con un formulario, un correo electrónico o una página de aterrizaje de Marketo. Para realizar un seguimiento de cuándo deposita un cheque, utilice una actividad personalizada. Para realizar un seguimiento de cuándo asiste un usuario a un seminario web, utilice una actividad personalizada.

>[!NOTE]
>
>Las actividades personalizadas difieren de los objetos personalizados. Utilice objetos personalizados cuando el valor pueda cambiar (por ejemplo, el &quot;color del coche&quot; cambia de azul a rojo). Utilice actividades personalizadas cuando rastree momentos que se produjeron y sus detalles no puedan cambiar (por ejemplo, &quot;coche comprado&quot;).

## Campos {#fields}

Puede agregar [campos adicionales](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md) que desee asociar con su actividad. Al igual que el campo principal, se pueden utilizar como criterios de filtrado en una lista inteligente.

## Introducción {#getting-started}

Las actividades personalizadas funcionan igual que las actividades estándar. Sin embargo, la configuración es un proceso de dos pasos.

Paso 1: [Cree una actividad personalizada](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md) en su cuenta de Marketo

Paso 2: El empleado de su organización que trabaja con la API de Marketo puede comenzar la implementación. Encontrará más información aquí: [API de actividad personalizada](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST)
