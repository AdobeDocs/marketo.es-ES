---
unique-page-id: 2951044
description: 'Notas de la versión, mayo de 2014, Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2014
exl-id: c7b5b2c1-ea3d-483b-8a65-c4d6313bfe31
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Notas de la versión: mayo de 2014 {#release-notes-may}

En la versión de mayo de 2014 de se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition. Después del lanzamiento, asegúrese de volver para encontrar vínculos a artículos detallados de la Base de conocimiento para cada función.

## Eliminar espacio de trabajo {#delete-workspace}

Ahora puede [eliminar un espacio de trabajo sin usar](/help/marketo/product-docs/administration/workspaces-and-person-partitions/delete-a-workspace.md). Asegúrese de mover todos los recursos a otro espacio de trabajo antes de intentar eliminarlo.

## Programar primer lanzamiento {#schedule-first-cast}

En los programas de participación, puede programar la fecha para que [se ejecute por primera vez](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) la conversión. Por ejemplo, especifique la cadencia que debe ser cada 2 semanas y seleccione la fecha del primer lanzamiento.

![](assets/image2014-9-22-11-3a57-3a36.png)

![](assets/image2014-9-22-11-3a57-3a54.png)

## Programas de participación mejorados {#enhanced-engagement-programs}

Ahora todos tienen múltiples programas, flujos y límites de comunicación.

## Seguimiento de vínculos en correos electrónicos de texto {#link-tracking-in-text-emails}

[Agregue corchetes dobles](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-tracked-links-to-a-text-email.md) alrededor de las direcciones URL en la versión de texto de sus correos electrónicos para indicar cuándo se deben convertir los vínculos en vínculos de seguimiento de Marketo redirigidos

>[!NOTE]
>
>**Ejemplo**
>
>`[[https://www.marketo.com]]`

De forma predeterminada, no se realiza un seguimiento de los vínculos en la versión de texto de los correos electrónicos. Añada esta nueva sintaxis para indicar cuándo se debe convertir un vínculo en un vínculo de seguimiento. El comportamiento de los vínculos de HTML no cambia.  Para añadir vínculos rastreados a los correos electrónicos:

* **Versión de HTML:** Inserte el vínculo. Se rastreará de forma predeterminada.
* **Versión de texto:** Escriba la dirección URL entre corchetes dobles.

Para añadir vínculos sin rastrear a los correos electrónicos:

* **Versión de HTML:** Inserte el vínculo y agregue la clase &quot;mktNoTrack&quot; al vínculo.
* **Versión de texto:** Solamente ingrese la dirección URL. Se desrastreará de forma predeterminada.

![](assets/image2014-9-22-12-3a1-3a34.png)

## Marcado de vínculos en correos electrónicos de muestra {#link-markup-in-sample-emails}

Vea cómo se comportarán los vínculos en los correos electrónicos con antelación. Los correos electrónicos de muestra ahora muestran vínculos exactamente como aparecerían a los posibles clientes. Obtenga una vista previa de los vínculos que se han convertido en vínculos de seguimiento, lo que le permite tener una mejor idea de cómo aparecerá realmente el mensaje para los destinatarios.

## [!UICONTROL Anular campaña] {#abort-campaign}

¡No se preocupe! Si encuentra un error, use el nuevo botón [cancelar campaña](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md) para detener inmediatamente las campañas en su seguimiento. Recibirá una notificación que indica cuántos posibles clientes estaban pendientes en cada paso del flujo cuando se detuvo la campaña.

## [!UICONTROL Insight de ventas] en japonés, portugués y español {#sales-insight-in-japanese-portuguese-and-spanish}

Descargue la última versión de [!UICONTROL Sales Insight] de AppExchange para que sus agentes de ventas que hablan japonés, portugués y español vean el contenido de [!UICONTROL Sales Insight] en su idioma preferido.

![](assets/image2014-9-22-12-3a2-3a12.png)

## Estado del programa y plazo de éxito en el análisis de pertenencia a programas {#program-status-and-success-timeframe-in-program-membership-analysis}

Vea cuántos [miembros hay en cada estado de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/build-a-program-membership-analysis-report-that-lists-leads.md) y cuándo cambiaron a cada estado, incluida la fecha en que lograron el éxito del programa.

## Correos electrónicos de prueba A/B en [!UICONTROL análisis de correo electrónico] {#a-b-test-emails-in-email-analysis}

Informe sobre cada una de sus [variantes de correo electrónico de prueba A/B](/help/marketo/product-docs/reporting/revenue-cycle-analytics/email-analysis/build-an-email-analysis-report-that-shows-program-information.md) en [!UICONTROL Análisis de correo electrónico].

## Cambios en paquetes de Analytics {#analytics-packaging-changes}

Revenue Cycle Modeler y Success Path Analyzer ahora se incluyen en MA Standard Edition.

## Información de plataforma móvil {#mobile-platform-info}

[Segmento y déclencheur](/help/marketo/product-docs/reporting/basic-reporting/report-activity/build-a-people-performance-report-with-mobile-platform-columns.md) de posibles clientes que abren y hacen clic en correos electrónicos desde sus dispositivos móviles.
