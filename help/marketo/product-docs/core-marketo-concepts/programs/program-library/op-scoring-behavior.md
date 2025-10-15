---
description: OP-Scoring-Behavior - Documentos de Marketo - Documentación del producto
title: OP-Comportamiento de puntuación
feature: Programs
exl-id: c564a301-0054-431a-8f0f-0299cd91b59c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 30%

---

# OP-Comportamiento de puntuación {#op-scoring-behavior}

Este ejemplo es un programa operativo avanzado (con token) para puntuación de comportamiento mediante un programa predeterminado de Marketo Engage. Vea y edite los valores de puntuación en la pestaña &quot;Mis tokens&quot; del programa. Requiere un campo de puntuación personalizado llamado &quot;Puntuación de comportamiento&quot;.

Para obtener más ayuda sobre la estrategia o para personalizar un programa, comuníquese con el equipo de cuenta de Adobe o visite la página de [Adobe Professional Services](https://business.adobe.com/es/customers/consulting-services/main.html){target="_blank"}.

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

## Campos de requisitos previos {#prerequisite-fields}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nombre descriptivo</th>
   <th>Nombre de API</th>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td>Puntuación de comportamiento</td>
   <td>Puntuación de comportamiento</td>
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
   <td>Correo electrónico: vínculos de clics en el correo electrónico</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Formulario: Rellena El Formulario De Contacto</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Formulario: Rellena El Formulario De Contenido</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Formulario: rellena el formulario predeterminado</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Formulario: Rellena El Formulario De Eventos</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Web: descarga cualquier PDF</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Web: Puntuación PPC</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Web: Visitas en páginas web clave</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Web: visita varias páginas web en un día</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Evento en directo: asistencia</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Feria - Influenciada</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Feria - Cabina visitada</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Seminario web: asistencia</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Disminuir puntuación: sin actividad</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Disminuir puntuación: visitas a páginas web no deseadas</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Interacciones</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Cambios de estado del programa</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Deterioro de puntuación</td>
  </tr>
 </tbody>
</table>

![](assets/op-scoring-behavior-1.png)

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo de token</th>
   <th>Nombre del token</th>
   <th>Valor</th>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr>
   <td>Puntuación</td>
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr>
   <td>Puntuación</td>
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr>
   <td>Puntuación</td>
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr>
   <td>Puntuación</td>
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Puntuación</td>
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
  </tr>
 </tbody>
</table>

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

* Cada campaña creada debe ser un ejemplo de la compilación de prácticas recomendadas y no específica para sus casos de uso. Recuerde actualizar las campañas inteligentes para abordar sus puntos problemáticos específicos y los desafíos en materia de datos.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.
