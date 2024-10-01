---
description: Tablero de métricas de observación de sincronización de Salesforce - Documentos de Marketo - Documentación del producto
title: Tablero de métricas de observabilidad de sincronización de Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 2457f0f51c6365c29a040e908678e81517327de5
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Métricas de registro de sincronización de Salesforce  {#salesforce-sync-backlog-metrics}

Revise el rendimiento de la sincronización y los trabajos pendientes de sincronización con este tablero.

## Rendimiento de sincronización y registro de pendientes {#sync-throughput-and-backlog}

1. En Marketo Engage, vaya al área de Administración.

   CAPTURA DE PANTALLA

1. Seleccione Salesforce.

   CAPTURA DE PANTALLA

Las estadísticas reflejan el rendimiento y el estado del registro de pendientes de cada tipo de objeto sincronizado durante las últimas 24 horas. Los tipos de objeto incluyen todos los objetos sincronizados, incluidos: Posible cliente, Contacto, Cuenta, Oportunidad, Campaña, Usuario y Objetos personalizados. Las estadísticas de rendimiento se actualizan automáticamente cada 15 minutos, pero puede hacerlo manualmente con el icono de actualización. El registro de pendientes se recupera cada hora.

>[!NOTE]
>
>Las estadísticas se actualizan de forma gradual, no por día natural.

CAPTURA DE PANTALLA

<table><thead>
  <tr>
    <th>Campo</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Máximo de registros sincronizados por hora</td>
    <td>El número máximo de registros sincronizados por hora (rendimiento máximo) observado en las últimas 24 horas para el tipo de objeto. El periodo de 24 horas se desplaza con el tiempo, no con el día del calendario.</td>
  </tr>
  <tr>
    <td>Registros mínimos sincronizados por hora</td>
    <td>Número mínimo de registros sincronizados por hora (rendimiento mínimo) observados en las últimas 24 horas para el tipo de objeto. El periodo de 24 horas se desplaza con el tiempo, no con el día del calendario.</td>
  </tr>
  <tr>
    <td>Registros promedio sincronizados por hora</td>
    <td>Número promedio de registros sincronizados por hora (rendimiento mínimo) observados en las últimas 24 horas para el tipo de objeto. El periodo de 24 horas se desplaza con el tiempo, no con el día del calendario. Se calcula como el número total de registros sincronizados en las últimas 24 horas.</td>
  </tr>
  <tr>
    <td>Sincronizar registro de pendientes</td>
    <td>El registro de registros pendientes de sincronización para el tipo de objeto. Es la suma total de la sincronización pendiente de registro en ambas direcciones (de Salesforce a Marketo Engage y viceversa). El registro de pendientes de Salesforce se obtiene mediante una llamada de API a Salesforce y el registro de pendientes de Marketo Engage se calcula mediante las estadísticas obtenidas del registro de datos de cambios. Se calcula cada hora. Los dos campos siguientes de esta tabla informan de cuándo se calculó por última vez el registro de pendientes y la siguiente programación para el cálculo, respectivamente.</td>
  </tr>
  <tr>
    <td>Registro de pendientes estimado (tiempo)</td>
    <td>Estimación del tiempo necesario para sincronizar el registro de pendientes por tipo de objeto. Se calcula como Registro de pendientes de sincronización/Promedio de registros sincronizados por hora.</td>
  </tr>
  <tr>
    <td>Último registro de pendientes recuperado</td>
    <td>Hora del último cálculo del registro de pendientes.</td>
  </tr>
  <tr>
    <td>Siguiente captura de registro pendiente</td>
    <td>Hora del siguiente cálculo del registro de pendientes.</td>
  </tr>
  <tr>
    <td>Estado de trabajo pendiente</td>
    <td>Esto muestra si el registro de pendientes ha aumentado en las últimas 6 horas. Se deduce como "Creciente" si el registro de asuntos pendientes actual es mayor que el registro de asuntos pendientes hace seis horas. De lo contrario, se muestra como "Normal". El objetivo de esto es mostrar si el rendimiento de la sincronización se está poniendo al día con el registro de pendientes.</td>
  </tr>
</tbody></table>

## Tendencia de trabajos pendientes {#backlog-trend}

La tendencia del registro de pendientes refleja los cambios en los registros de asuntos pendientes registrados durante los últimos 5 días. El registro de pendientes se muestra en un intervalo de tiempo de 4 horas dividido en 5 días. Por lo tanto, el gráfico mostrará 6 intervalos por día por 5 días, lo que equivale a 30 intervalos.

El registro de pendientes se observa a un intervalo de tiempo particular de 4 horas en el eje x. Este valor es para todos los objetos sincronizados. Este es el total del registro de pendientes en Salesforce y Marketo Engage que esperan sincronizarse.

CAPTURA DE PANTALLA
