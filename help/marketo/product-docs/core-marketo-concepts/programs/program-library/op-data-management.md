---
description: Administración de datos de OP - Documentos de Marketo - Documentación del producto
title: Administración de datos de OP
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 26%

---

# Administración de datos de OP {#op-data-management}

Este es un ejemplo de flujos de trabajo de prácticas recomendadas de administración de datos operacionales simples que utilizan un programa predeterminado para ayudarle a administrar la coherencia de datos para los registros de la base de datos de Marketo Engage.

Para obtener más ayuda sobre la estrategia o para personalizar un programa, ponte en contacto con el equipo de la cuenta de Adobe o visita la página de [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Normalizar país - Estados Unidos</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Normalizar país - Reino Unido</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Definir Incluido en la lista de bloqueados como verdadero</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Establecer Is Partner en True</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Lista de importación</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Evento en vivo</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Publicidad en línea</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Feria</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Contenido web</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Solicitud web</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Seminario web</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona de la importación de lista</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona a partir de un evento en directo</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona de Online Advertising</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona de la feria</td>
  </tr>
   <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona a partir del contenido web</td>
  </tr>
   <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona a partir de solicitud web</td>
  </tr>
   <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>Nueva persona del seminario web</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Lote nocturno de Source de personas (para instancias de alto tráfico)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Source de persona activado (para instancias de poco tráfico)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Source de persona de captura</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Normalización</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Administración de registros</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Lista de bloqueos</td>
  </tr>
 </tbody> 
</table>

![](assets/op-data-management-1.png)

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

* Cada campaña creada debe ser un ejemplo sobre la compilación de la práctica recomendada y no específica para sus casos de uso. Recuerde actualizar las campañas inteligentes para abordar sus puntos problemáticos específicos y los desafíos en materia de datos.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.
