---
description: OP-Acquisition-API - Documentos de Marketo - Documentación del producto
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 19%

---

# OP-Acquisition-API {#op-acquisition-api}

Este programa de ejemplo es para procesos operativos para rastrear la adquisición de registros de fuentes de API utilizando un programa predeterminado de Marketo Engage.

## Resumen del canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Estado de abono</th>
   <th>Comportamiento de análisis</th>
   <th>Tipo de programa</th>
  </tr>
  <tr>
   <td>Operativo</td>
   <td>Miembro 01</td>
   <td>Operativo</td>
   <td>Predeterminado</td>
  </tr>
 </tbody>
</table>

## El programa contiene el siguiente Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nombre de plantilla</th>
   <th>Nombre del recurso</th>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Configurar adquisición - Lote</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Configurar adquisición - Déclencheur</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Campaigns (contiene todas las campañas inteligentes)</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

## Reglas de conflicto {#conflict-rules}

* **Etiquetas de programas**
   * Crear etiquetas en esta suscripción: _Recomendado_
   * Ignorar

* **Plantilla de página de aterrizaje con el mismo nombre**
   * Copiar plantilla original: _Recomendado_
   * Usar plantilla de destino

* **Imágenes con el mismo nombre**
   * Conservar ambos archivos: _Recomendado_
   * Reemplazar elemento en esta suscripción

* **Plantillas de correo electrónico con el mismo nombre**
   * Mantener ambas plantillas: _Recomendado_
   * Reemplazar plantilla existente

## Mejores prácticas {#best-practices}

* Ejecute primero la campaña por lotes si necesita ponerse al día en la administración de datos.

* Considere la posibilidad de utilizar programas similares para garantizar la alineación con las prácticas recomendadas en todas las fuentes de entrada e incluir su CRM o integraciones de datos.

* Dentro de las iniciativas de marketing de canal específicas, asegúrese de capturar la adquisición cuando sea necesario.
