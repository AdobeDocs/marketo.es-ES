---
description: CT-AAAA-MM-Página de aterrizaje de contenido que no es de Marketo - Documentos de Marketo - Documentación del producto
title: CT-AAAA-MM-Contenido de la página de destino que no es de Marketo
feature: Programs
exl-id: b7cf8e52-4f3f-44d7-ab4c-ad10fa0badc9
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 15%

---

# CT-AAAA-MM-Contenido de la página de destino que no es de Marketo {#ct-yyyy-mm-content-non-marketo-landing-page}

Este es un ejemplo de programa de contenido con un formulario de Marketo Engage para descargar contenido en una página de aterrizaje que no sea de Marketo Engage mediante un programa predeterminado de Marketo Engage. Este programa está diseñado para trabajar con un formulario de Marketo Engage incrustado en el sitio web. El vínculo a la oferta/contenido se puede enviar en un correo electrónico de agradecimiento.

Para obtener más ayuda sobre la estrategia o para personalizar un programa, comuníquese con el equipo de cuenta de Adobe o visite la página de [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Contenido web</td>
   <td>Miembro 01
<br/>02-Participación-Éxito</td>
   <td>Incluido</td>
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
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>01-Correo electrónico-Gracias</td>
  </tr>
  <tr>
   <td>Formulario</td>
   <td> </td>
   <td>Formulario de registro de contenido FM (recurso global en Design Studio)</td>
  </tr>
  <tr>
   <td>Informe local</td>
   <td> </td>
   <td>Desempeño de email</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>00-Programa de adquisición de capturas</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Formulario rellenado en 01</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>Participación en el programa 02 (éxito del programa)</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Assets: aloja todos los recursos creativos
<br/>(subcarpetas para correos electrónicos y páginas de aterrizaje)  </td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Campañas: aloja todas las campañas inteligentes</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Informes</td>
  </tr>
 </tbody>
</table>

![](assets/ct-yyyy-mm-content-non-marketo-landing-page-1.png)

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo de token</th>
   <th>Nombre del token</th>
   <th>Valor</th>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
 </tbody>
</table>

## Reglas de conflicto {#conflict-rules}

* **Etiquetas de programas**
   * Crear etiquetas en esta suscripción: _Recomendado_
   * Ignorar

* **Plantilla de página de aterrizaje con el mismo nombre**
   * Copiar plantilla original
   * Usar plantilla de destino: _Recomendado_

* **Imágenes con el mismo nombre**
   * Conservar ambos archivos
   * Reemplazar elemento en esta suscripción: _Recomendado_

* **Plantillas de correo electrónico con el mismo nombre**
   * Conservar ambas plantillas
   * Reemplazar plantilla existente: _Recomendado_

## Mejores prácticas {#best-practices}

* Después de importar el programa de contenido, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad para actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;02-Engaged&quot; para realizar un seguimiento del éxito. Haga esto _antes_ de que su formulario esté activo y se envíen correos electrónicos.
