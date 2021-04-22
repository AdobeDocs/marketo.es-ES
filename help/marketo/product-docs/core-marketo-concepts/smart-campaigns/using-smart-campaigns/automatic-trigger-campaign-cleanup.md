---
unique-page-id: 1147074
description: Limpieza automática de campañas de Déclencheur - Documentos de Marketo - Documentación del producto
title: Limpieza automática de campañas de Déclencheur
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Limpieza automática de campañas de Déclencheur {#automatic-trigger-campaign-cleanup}

Marketo tiene un servicio agradable/gratuito para desactivar las campañas inteligentes activadas que ya no obtienen actividad. Esto acelera el rendimiento general del sistema y le ahorra tiempo.

## ¿Qué pasa? {#what-happens}

Una vez al trimestre, Marketo encontrará campañas inteligentes que se hayan mantenido inactivas (sin personas) durante 6 meses o más y las desactivará.

## ¿Me avisarás primero? {#will-you-notify-me-first}

¡Por supuesto! Una vez al trimestre, recibirá una notificación con una semana de antelación que muestra cada campaña que planeamos desactivar.

1. Vaya a la pestaña **Notifications**.

   ![](assets/notifications.png)

1. Haga clic en **Limpieza de campaña de Déclencheur inactivo programada**. A continuación, haga clic en el enlace **Estas campañas de Déclencheur inactivo se desactivarán**.

   ![](assets/image2015-4-27-20-3a48-3a35.png)

   Verá una lista de campañas inteligentes programadas para desactivarse.

   ![](assets/image2015-4-27-20-3a35-3a29.png)

## ¿Qué campañas se desactivarán? {#which-campaigns-will-be-deactivated}

Solo desactivaremos las campañas de déclencheur que hayan estado activas durante más de 6 meses pero que tengan 0 personas cualificadas en ese período de tiempo.

## ¡Espera! ¡No esta campaña! {#wait-not-this-campaign}

No se preocupe: el reloj de cualquier campaña inteligente se puede restablecer mediante:

* Una persona que reúne los requisitos para la campaña.
* Desactivación y reactivación manuales de la campaña.

Se restablecerá el contador de 6 meses.

## ¿Me avisará de qué campañas se desactivaron? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolutamente: una semana después de la notificación original, desactivaremos las campañas enumeradas (menos las que cualificaron al menos a una persona o que se desactivaron o reactivaron) y publicaremos una notificación de confirmación.

1. Seleccione la notificación **Idle Déclencheur Campaign Cleanup Scheduled**. Haga clic en el vínculo **Estas campañas de Déclencheur inactivo**.

   ![](assets/image2015-4-27-20-3a56-3a41.png)

1. Verá una lista de campañas desactivadas.

   ![](assets/image2015-4-27-20-3a58-3a38.png)
