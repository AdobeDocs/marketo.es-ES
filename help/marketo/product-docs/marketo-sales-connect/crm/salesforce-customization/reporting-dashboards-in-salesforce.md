---
unique-page-id: 14352464
description: Paneles de informes en Salesforce - Documentos de Marketo - Documentación del producto
title: Informes de paneles en Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Informes de paneles en Salesforce {#reporting-dashboards-in-salesforce}

Aprenda a configurar los paneles a continuación.

## Abrir y hacer clic en informe {#open-and-click-report}

1. Seleccione el tipo de registro **Tareas y eventos**.
1. Defina los parámetros del informe en función del lapso de tiempo y la estructura de jerarquía deseados.
1. Añada un filtro para eliminar los correos electrónicos internos registrados en Salesforce (por ejemplo, Empresa/Cuenta distinta de Marketo).
1. Seleccione el formato de informe **Resumen**.
1. Añada al informe los campos Asunto, Asignado y Ventas Marketo en las que se hizo clic/Ventas Marketo vistas.
1. Haga doble clic en **Agregar fórmula** en el panel Campos.
1. Agregue un nombre a la fórmula, seleccione **Porcentaje** con el formato y seleccione **Agrupación 1**.
1. Seleccione **Ventas Marketo en las que se hizo clic/Ventas Marketo que se vieron** y luego **Sum** en los campos de resumen.
1. Agregue un signo de división a la fórmula y, a continuación, seleccione **Recuento de registros** en los campos Resumen - _Guardar como_.

## Informe de rendimiento de plantilla {#template-performance-report}

1. Personalice el informe Abrir y hacer clic para incluir los siguientes campos: _Guardar como_.

## Informe de volumen de plantilla {#template-volume-report}

1. Modifique el Informe de Rendimiento de la Plantilla e incluya el filtro &quot;Plantilla de Ventas Marketo no es igual a en blanco&quot;.
1. Elimine el campo Ventas de Marketo en las que se hizo clic - _Guardar como_.

## Informe Cuentas de tendencias {#trending-accounts-report}

1. Seleccione el tipo de registro Actividades con cuentas.
1. Configure los parámetros y campos del informe como se indica a continuación - _Guardar como_.
