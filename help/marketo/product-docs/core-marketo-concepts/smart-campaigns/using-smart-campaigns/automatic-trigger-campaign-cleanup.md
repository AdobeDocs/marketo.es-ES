---
unique-page-id: 1147074
description: Limpieza automática de campañas de Déclencheur - Documentos de Marketo - Documentación del producto
title: Limpieza de campañas de activador automático
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 3%

---

# Limpieza de campañas de activador automático {#automatic-trigger-campaign-cleanup}

Marketo tiene un servicio agradable/gratuito para desactivar las campañas inteligentes activadas que ya no reciben actividad. Esto acelera el rendimiento general del sistema y le ahorra tiempo.

## ¿Qué pasa? {#what-happens}

Una vez al trimestre, Marketo encontrará campañas inteligentes que han permanecido inactivas (sin personas) durante 6 meses o más y las desactivará.

## ¿Me avisarás primero? {#will-you-notify-me-first}

¡Por supuesto! Una vez al trimestre, recibirá una notificación una semana antes que se mostrarán todas las campañas que planeamos desactivar.

1. Haga clic en el icono **[!UICONTROL Notificaciones]**.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Haga clic en **[!UICONTROL Limpieza programada de campaña de Déclencheur inactiva]**. Luego haga clic en el vínculo **[!UICONTROL Se desactivarán estas campañas de Déclencheur inactivas]**.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Verá una lista de campañas inteligentes programadas para desactivarse.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## ¿Qué campañas se desactivarán? {#which-campaigns-will-be-deactivated}

Solo desactivaremos las campañas de déclencheur que hayan estado activas durante más de 6 meses pero que hayan tenido 0 personas cualificadas en ese período de tiempo.

## ¡Espera! ¡Esta campaña no! {#wait-not-this-campaign}

No se preocupe: el reloj de cualquier campaña inteligente se puede restablecer haciendo lo siguiente:

* Persona que cumple los requisitos para la campaña.
* Desactivación y reactivación manuales de la campaña.

Cualquiera restablecerá el contador de 6 meses.

## ¿Me permite saber qué campañas se desactivaron? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolutamente: una semana después de la notificación original, desactivaremos las campañas enumeradas (menos todas que cumplan los requisitos de al menos una persona o que se hayan desactivado/reactivado) y publicaremos una notificación de confirmación.

1. Seleccione la notificación **[!UICONTROL Limpieza programada de la campaña de Déclencheur inactiva]**. Haga clic en el vínculo **[!UICONTROL Estas campañas de Déclencheur inactivas]**.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Verá una lista de campañas desactivadas.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
