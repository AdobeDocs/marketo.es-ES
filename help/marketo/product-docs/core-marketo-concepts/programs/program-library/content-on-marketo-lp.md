---
description: Contenido en Marketo LP - Documentos de Marketo - Documentación del producto
title: Contenido en Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 9%

---

# Contenido en Marketo LP {#content-on-marketo-lp}

Nombre del programa: CT-AAAA-MM-Contenido en Marketo LP

Esta referencia de ejemplo está diseñada para ser un programa de contenido que aprovecha una página de aterrizaje de Marketo con un formulario de Marketo que utiliza un programa predeterminado de Marketo. El formulario es para acceder al contenido/oferta. El vínculo a la oferta se puede mostrar en la página de agradecimiento, en un correo electrónico de agradecimiento o en ambos. Para obtener más ayuda sobre la estrategia o para personalizar un programa, póngase en contacto con el equipo de cuenta de Adobe o visite el [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) página.

**Resumen del canal**

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
   <td>Inclusivo</td>
   <td>Predeterminado</td>
  </tr>
 </tbody> 
</table>

**El programa contiene los siguientes recursos:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nombre de plantilla</th>
   <th>Nombre del recurso</th>
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
   <td>Formulario</td> 
   <td> </td>
   <td>Formulario de registro de contenido</td>
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
<br/>(subcarpetas para correo electrónico y páginas de aterrizaje)  </td>
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

CAPTURA DE PANTALLA - Imagen del programa

**Mis tokens incluían:**

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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.thankYouPageURL?sin el http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Consulte Instrucciones de importación de programas para reglas de conflicto predeterminadas.

**Reglas de conflicto predeterminadas recomendadas para la importación:**

* Etiquetas de programa
   * Crear etiquetas en esta suscripción (predeterminado): recomendado
   * Ignorar

* Plantilla de página de aterrizaje con el mismo nombre
   * Copiar plantilla original (predeterminado)
   * Usar plantilla de destino: recomendado

* Imágenes con el mismo nombre
   * Mantener ambos archivos (predeterminado)
   * Reemplazar elemento de esta suscripción: recomendado

* Plantillas de email con el mismo nombre
   * Mantener ambas plantillas (predeterminado)
   * Reemplazar plantilla existente: recomendado

CAPTURA DE PANTALLA: imagen de las reglas de conflicto predeterminadas

**Prácticas recomendadas recomendadas:**

* Las prácticas recomendadas de consultoría de Marketo recomiendan que, después de importar el programa de contenido, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio de Marketo Engage.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad en las actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información adecuada del logotipo y pie de página.

* Considere la posibilidad de actualizar la convención de nombres de esta plantilla de programa para alinearla con la convención de nombres, si es necesario.

* No olvide actualizar los Valores de My Token en la plantilla del programa y cada vez que utilice el programa, según sea necesario.

* Para obtener más ayuda sobre la estrategia o para personalizar un programa, póngase en contacto con el equipo de cuenta de Adobe o visite el [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) página.

>[!TIP]
>
>No olvide activar la campaña &quot;02-Engaged&quot; para realizar un seguimiento del éxito. Haga esto ANTES de que su formulario esté activo y se envíen correos electrónicos.

>[!NOTE]
>
>Mis tokens que hacen referencia a una dirección URL no pueden contener los http:// u https://; de lo contrario, el vínculo no funcionará correctamente dentro del recurso.
