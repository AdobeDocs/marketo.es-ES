---
description: Página de aterrizaje de Marketo de publicidad en línea de OA-YYYY-MM - Documentos de Marketo - Documentación del producto
title: OA-YYYY-MM-Página de aterrizaje de Marketo de publicidad en línea
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: afdf59729f16d27a548fa60a8156c941be54a8a7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# OA-YYYY-MM-Página de aterrizaje de Marketo de publicidad en línea {#oa-yyyy-mm-online-advertising-marketo-landing-page}

Este es un ejemplo de programa de seguimiento de publicidad en línea que incluye una página de aterrizaje de Marketo con formulario de registro y un programa predeterminado de Marketo. El vínculo a la oferta se puede mostrar en la página de agradecimiento, en un correo electrónico de agradecimiento o en ambos.

Para obtener más ayuda sobre la estrategia o para personalizar un programa, póngase en contacto con el equipo de cuenta de Adobe o visite el [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} página.

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
   <td>Publicidad en línea</td> 
   <td>Miembro 01 
<br/>02-Participación-Éxito</td>
   <td>Inclusivo</td>
   <td>Predeterminado</td>
  </tr>
 </tbody> 
</table>

## El programa contiene los siguientes recursos {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nombre de plantilla</th>
   <th>Nombre del recurso</th>
  </tr> 
  <tr> 
   <td>Formulario</td> 
   <td> </td>
   <td>Registro de contenido FM</td>
  </tr>
  <tr> 
   <td>Correo electrónico</td> 
   <td>Plantilla de correo electrónico de inicio rápido</td>
   <td>01-Correo electrónico-Gracias</td>
  </tr>
  <tr> 
   <td>Página de aterrizaje</td> 
   <td>Plantilla de LP de inicio rápido</td>
   <td>01 - LP - Registro</td>
  </tr>
   <tr> 
   <td>Página de aterrizaje</td> 
   <td>Plantilla de LP de inicio rápido</td>
   <td>02 - LP - Gracias</td>
  </tr>
   <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de correo electrónico</td>
  </tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de página de aterrizaje</td>
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
   <td>Informes de  </td>
  </tr>
 </tbody> 
</table>

CAPTURA DE PANTALLA DEL PROGRAMA

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Nombre de token</th>
   <th>Valor</th>
  </tr> 
  <tr> 
   <td>Texto enriquecido</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Haga doble clic para obtener detalles  
<br/><code><--My Content Description Here--></code> 
<br/>Edite esta descripción de contenido en el nivel de programa, en la pestaña Mis tokens. 
<br/>Aprenderá a hacer lo siguiente: 
<li>Viñeta 1</li>
<li>Viñeta 2</li>
<li>Viñeta 3</li></td>
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
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.thankYouPageURL?sin el http://</td>
  </tr>
 </tbody> 
</table>

## Reglas de conflicto {#conflict-rules}

* **Etiquetas del programa**
   * Crear etiquetas en esta suscripción: _Recomendado_
   * Ignorar

* **Plantilla de página de aterrizaje con el mismo nombre**
   * Copiar plantilla original
   * Usar plantilla de destino - _Recomendado_

* **Imágenes con el mismo nombre**
   * Conservar ambos archivos
   * Reemplazar elemento en esta suscripción - _Recomendado_

* **Plantillas de email con el mismo nombre**
   * Conservar ambas plantillas
   * Reemplazar plantilla existente: _Recomendado_

CAPTURA DE PANTALLA DE REGLAS DE CONFLICTO

## Prácticas recomendadas {#best-practices}

* Después de importar el programa de contenido, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad en las actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Use Etiquetas de programas para filtrar informes según las distintas fuentes de publicidad en línea.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;02-Engaged&quot; para realizar un seguimiento del éxito. Haga esto _antes_ el formulario está activo y se envían correos electrónicos.

>[!IMPORTANT]
>
>Mis tokens que hacen referencia a una dirección URL no pueden contener los http:// u https://; de lo contrario, el vínculo no funcionará correctamente dentro del recurso.
