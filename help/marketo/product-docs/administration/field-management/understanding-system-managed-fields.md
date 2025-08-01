---
unique-page-id: 5472615
description: Explicación de los campos administrados por el sistema - Documentos de Marketo - Documentación del producto
title: Explicación de los campos administrados por el sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# Explicación de los campos administrados por el sistema {#understanding-system-managed-fields}

Es posible que haya observado que la [página de detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} tiene una serie de campos no editables creados por Marketo. Estos datos provienen de varias fuentes y hay infinidad de valores que podrían mostrarse.

## Tipos de campo {#field-types}

<table><thead>
  <tr>
    <th>Nombre del campo</th>
    <th>Definición</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Tipo de origen original</td>
    <td>La ubicación en la que se descubrió por primera vez una persona o visitante de un sitio web (Ejemplo: importación de lista, visita de página web)</td>
  </tr>
  <tr>
    <td>Información de origen original</td>
    <td>Detalles específicos sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web)</td>
  </tr>
  <tr>
    <td>Motor de búsqueda original</td>
    <td>Si procede, el motor de búsqueda que refirió a la persona a la fuente de entrada original</td>
  </tr>
  <tr>
    <td>Frase de búsqueda original</td>
    <td>Si procede, el término de búsqueda utilizado que refirió a la persona a la fuente de entrada original</td>
  </tr>
  <tr>
    <td>Remitente original</td>
    <td>URL que alojó el origen de entrada original</td>
  </tr>
  <tr>
    <td>Tipo de origen del registro</td>
    <td>La ubicación de una actividad se convirtió en una persona por primera vez (Ejemplo: importación de lista, visita de página web)</td>
  </tr>
  <tr>
    <td>Información de origen del registro</td>
    <td>Detalles específicos sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web)</td>
  </tr>
  <tr>
    <td>IP anónima</td>
    <td>Indica la dirección IP de una persona</td>
  </tr>
  <tr>
    <td>Compañía inferida</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) de la compañía de la persona</td>
  </tr>
  <tr>
    <td>Ciudad inferida</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) de la ciudad de la persona</td>
  </tr>
  <tr>
    <td>Región del estado inferida</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) del estado o la región de la persona</td>
  </tr>
  <tr>
    <td>Código postal inferido</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) del código postal de la persona</td>
  </tr>
  <tr>
    <td>País inferido</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) del país de la persona</td>
  </tr>
  <tr>
    <td>Área metropolitana inferida</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) del área metropolitana de la persona</td>
  </tr>
  <tr>
    <td>Código de área telefónico inferido</td>
    <td>Mejor estimación de Marketo (basada en la dirección IP) del código de área de la persona</td>
  </tr>
</tbody></table>

## Valores posibles para el tipo de Source original y de registro {#possible-values-for-original-and-registration-source-type}

A continuación se muestran algunos valores posibles y lo que significan.

<table><thead>
  <tr>
    <th>Tipo de origen original</th>
    <th>Definición</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>Se detectó la persona a partir de la sincronización de Salesforce</td>
  </tr>
  <tr>
    <td>Visitas a páginas web</td>
    <td>La persona se ha descubierto desde una página web</td>
  </tr>
  <tr>
    <td>Rellenado de formulario web</td>
    <td>La persona se descubrió después de rellenar un formulario</td>
  </tr>
  <tr>
    <td>Lista de importación</td>
    <td>Se descubrió una persona a partir de una importación de lista</td>
  </tr>
  <tr>
    <td>Nueva persona</td>
    <td>La persona se ha introducido manualmente en la base de datos</td>
  </tr>
  <tr>
    <td>Clic en vínculo web</td>
    <td>Se descubrió una persona después de hacer clic en un vínculo</td>
  </tr>
  <tr>
    <td>Correo electrónico de ventas</td>
    <td>Se ha enviado un correo electrónico a la persona mediante el complemento de correo electrónico de Sales Insight</td>
  </tr>
  <tr>
    <td>Persona</td>
    <td>La persona se ha sincronizado desde Salesforce como persona</td>
  </tr>
  <tr>
    <td>Contacto</td>
    <td>La persona se ha sincronizado desde Webhook como contacto</td>
  </tr>
  <tr>
    <td>API de Munchkin</td>
    <td>La API de Munchkin de Marketo Engage ha descubierto la persona</td>
  </tr>
  <tr>
    <td>Aplicación social</td>
    <td>La persona fue descubierta por un widget social</td>
  </tr>
  <tr>
    <td>API de servicios web</td>
    <td>Una API de servicio web descubrió la persona</td>
  </tr>
  <tr>
    <td>Socio del evento</td>
    <td>La persona se ha descubierto mediante un servicio de seminario web sincronizado</td>
  </tr>
  <tr>
    <td>Asociar posible cliente</td>
    <td>Persona que se fusionó mediante la llamada a la API de Associate Lead</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Tipo de origen del registro</th>
    <th>Definición</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Lista de importación</td>
    <td>Se convirtió en una persona a través de una importación de lista</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Convertirse en persona mediante la sincronización de Salesforce</td>
  </tr>
  <tr>
    <td>Rellenado de formulario web</td>
    <td>Se convierte en persona después de rellenar un formulario</td>
  </tr>
  <tr>
    <td>Correo electrónico de ventas</td>
    <td>Se ha enviado un correo electrónico a la persona mediante el complemento de correo electrónico de Sales Insight</td>
  </tr>
  <tr>
    <td>API de servicios web</td>
    <td>La persona se ha creado mediante la API de SOAP/REST</td>
  </tr>
  <tr>
    <td>Nueva persona</td>
    <td>La persona se ha introducido manualmente en la base de datos</td>
  </tr>
  <tr>
    <td>API de Munchkin</td>
    <td>Convertirse en persona mediante la API de Munchkin de Marketo</td>
  </tr>
  <tr>
    <td>Aplicación social</td>
    <td>Convertirse en una persona a través de un widget social</td>
  </tr>
  <tr>
    <td>Socio del evento</td>
    <td>Convertirse en persona mediante un servicio de seminario web vinculado</td>
  </tr>
</tbody>
</table>
