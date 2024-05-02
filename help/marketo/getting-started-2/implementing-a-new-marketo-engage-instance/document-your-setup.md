---
description: Documente la configuración de la nueva instancia de Marketo Engage.
title: 'Prácticas Recomendadas Para Nuevas Instancias: Documentar La Configuración'
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 67b9d79482c16b0b513f81b02fe8f237961ac30f
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 2%

---

# Prácticas Recomendadas Para Nuevas Instancias: Documentar La Configuración {#new-instance-best-practices-document-your-setup}

Ahora que ha aprendido las áreas de producto clave para configurar para una nueva instancia de Marketo Engage, el siguiente paso es crear documentación para la configuración de la instancia y la pila tecnológica. Tanto si la crea mediante una hoja de cálculo como mediante una aplicación de gestión de proyectos, su documentación será un excelente recurso para realizar un seguimiento del progreso y registrar los detalles, así como para mantener su instancia estructurada y sostenible para los futuros especialistas en marketing de su organización.

## Datos {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Lista de importación</td>
    <td><li>Reúna una lista de fuentes de datos de las que se extraerán registros para <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people" target="_blank">importar en Marketo Engage</a>.</li>
    <li>Si está importando desde varios orígenes de datos, considere la posibilidad de utilizar Listas maestras o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">crear un campo personalizado</a> en el registro de persona para indicar la fuente de datos.</li></td>
  </tr>
  <tr>
    <td>Integración de base de datos</td>
    <td><li>Si aprovecha la sincronización nativa entre Marketo Engage y su CRM, tenga en cuenta cuidadosamente qué campos desea sincronizar entre sistemas. No es necesario sincronizar todos los campos, por lo que debe ser estratégico con los flujos de datos.</li></td>
  </tr>
</tbody>
</table>

## Documentación {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Usuarios</td>
    <td><li>Documente el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">usuarios actuales</a> en su caso por razones de seguridad. Los siguientes detalles deben incluirse como mínimo (y todos son visibles en Adobe Admin Console &gt; Usuarios):</li>
    <br>Nombre
    <br>Correo electrónico
    <br>Iniciar sesión
    <br>Rol
    <br>Fecha de caducidad del acceso
    <br>Fecha de creación del usuario
    <br>Fecha de inicio de sesión más reciente

NOTA: Los clientes también pueden ampliar esta información para incluir documentación sobre funciones/permisos.
<p>
<li>Como Administrador de productos de Marketo Engage, desarrolle un proceso interno para auditar y actualizar la lista de usuarios de Marketo Engage a una cadencia regular. Para realizar cambios en la lista de usuarios de Adobe Admin Console, tenga en cuenta lo siguiente <a href="https://helpx.adobe.com/es/enterprise/using/users.html" target="_blank">acciones masivas</a>, como cargar un .CSV, utilizar la API de REST de administración de usuarios, etc.</li></td>
</tr>
  <tr>
    <td>Organización</td>
    <td><li>Documente la estructura de carpetas acordada, las convenciones de nomenclatura estándar para programas, recursos, etc. y el por qué detrás de las decisiones tomadas. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Obtenga más información sobre las prácticas recomendadas aquí.</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Cree un registro de cambios donde pueda documentar qué está cambiando en su instancia y el por qué de las modificaciones. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Obtenga más información sobre las prácticas recomendadas aquí.</a></li></td>
  </tr>
  <tr>
    <td>Manuales</td>
    <td><li>Cree un manual de usuario o un manual de administración para los usuarios internos que se incorporen a la instancia.</li></td>
  </tr>
  <tr>
    <td>Conversaciones con equipos internos</td>
    <td><li>Comience a alinear las expectativas del equipo de marketing interno sobre Marketo Engage con las capacidades de Marketo Engage.</li>
    <li>Identifique los equipos que serán las partes interesadas en la instancia de Marketo Engage y documente sus objetivos para lograr utilizando Marketo Engage como tecnología.</li></td>
  </tr>
</tbody>
</table>
