---
unique-page-id: 14352464
description: 'Tableros de informes en Salesforce: Documentos de Marketo: Documentación del producto'
title: Tableros de informes en Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Tableros de informes en Salesforce {#reporting-dashboards-in-salesforce}

Aprenda a configurar los paneles a continuación.

## Abrir y hacer clic en el informe {#open-and-click-report}

1. Seleccione el **Tareas y eventos** tipo de registro.
1. Defina los parámetros del informe en función del intervalo de tiempo y la estructura de jerarquía que desee.
1. Añada un filtro para eliminar los correos electrónicos internos registrados en Salesforce (por ejemplo, Empresa/Cuenta no igual a Marketo).
1. Seleccione el **Resumen** formato del informe.
1. Agregue al informe los campos Asunto, Asignado y Marketo Sales Clicked/Marketo Sales Viewed .
1. Haga doble clic en **Agregar fórmula** dentro del panel Campos .
1. Agregar un nombre a la fórmula, seleccione **Porcentaje** en el formato y seleccione **Agrupación 1**.
1. Select **Ventas de Marketo pulsadas/ventas de Marketo vistos,** then **Sum** en los campos de resumen.
1. Agregue un signo de división a la fórmula y, a continuación, seleccione **Recuento de registros** en los campos Resumen: _Guardar como_.

## Informe Rendimiento de la plantilla {#template-performance-report}

1. Personalice el informe Abrir y Haga clic para incluir los siguientes campos: _Guardar como_.

## Informe de volumen de plantilla {#template-volume-report}

1. Modifique el informe Rendimiento de la plantilla e incluya el filtro &quot;Plantilla de ventas de Marketo no igual a en blanco&quot;.
1. Quitar el campo en el que se hizo clic de ventas de Marketo: _Guardar como_.

## Informe de cuentas de tendencias {#trending-accounts-report}

1. Seleccione el tipo de registro Actividades con cuentas .
1. Configure los parámetros y campos del informe como se indica a continuación: _Guardar como_.
