---
unique-page-id: 1147074
description: Limpieza automática de campañas de Déclencheur - Documentos de Marketo - Documentación del producto
title: Limpieza automática de campañas de Déclencheur
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
source-git-commit: 073a136953f1997436396cf3f2c87fdc1a3b9c1d
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Limpieza automática de campañas de Déclencheur {#automatic-trigger-campaign-cleanup}

Marketo tiene un servicio agradable/gratuito para desactivar las campañas inteligentes activadas que ya no obtienen actividad. Esto acelera el rendimiento general del sistema y le ahorra tiempo.

## ¿Qué pasa? {#what-happens}

Una vez al trimestre, Marketo encontrará campañas inteligentes que se hayan mantenido inactivas (sin personas) durante 6 meses o más y las desactivará.

## ¿Me avisarás primero? {#will-you-notify-me-first}

¡Por supuesto! Una vez al trimestre, recibirá una notificación con una semana de antelación que muestra cada campaña que planeamos desactivar.

1. Haga clic en el **Notificaciones** icono.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Haga clic en **Limpieza de campaña de Déclencheur inactivo programada**. A continuación, haga clic en el **Estas campañas de Déclencheur inactivo se desactivarán** vínculo.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Verá una lista de campañas inteligentes programadas para desactivarse.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## ¿Qué campañas se desactivarán? {#which-campaigns-will-be-deactivated}

Solo desactivaremos las campañas de déclencheur que hayan estado activas durante más de 6 meses pero que tengan 0 personas cualificadas en ese período de tiempo.

## Esperar! ¡No esta campaña! {#wait-not-this-campaign}

No se preocupe: el reloj de cualquier campaña inteligente se puede restablecer mediante:

* Una persona que reúne los requisitos para la campaña.
* Desactivación y reactivación manuales de la campaña.

Se restablecerá el contador de 6 meses.

## ¿Me avisará de qué campañas se desactivaron? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolutamente: una semana después de la notificación original, desactivaremos las campañas enumeradas (menos las que cualificaron al menos a una persona o que se desactivaron o reactivaron) y publicaremos una notificación de confirmación.

1. Seleccione el **Limpieza de campaña de Déclencheur inactivo programada** notificación. Haga clic en el **Estas campañas de Déclencheur inactivo** vínculo.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Verá una lista de campañas desactivadas.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
