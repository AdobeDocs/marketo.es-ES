---
description: Programa de solicitud WR-AAAA-MM-Web - Documentos de Marketo - Documentación del producto
title: Programa de solicitud web WR-AAAA-MM
feature: Programs
exl-id: 539dfd08-eed8-4fac-b976-7fe43f5d24b3
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 14%

---

# Programa de solicitud web WR-AAAA-MM {#wr-yyyy-mm-web-request-program}

Este es un programa de ejemplo ideal para formularios de solicitud de contacto, solicitud de presupuesto, solicitud de demostración o solicitud de prueba que utilizan un programa predeterminado de Marketo Engage. Se puede utilizar con páginas de destino de Marketo o como formulario incrustado en páginas de destino que no sean de Marketo. Se envía un correo electrónico de alerta a una persona especificada tras el envío del formulario.

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
   <td>Web Solicitud</td> 
   <td>01 - Participación - Éxito</td>
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
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>Alert-WebRequest</td>
  </tr>
  <tr> 
   <td>Página de aterrizaje</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Plantilla de LP de inicio rápido</a></td>
   <td>01 - LP - Solicitud</td>
  </tr>
  <tr> 
   <td>Página de aterrizaje</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Plantilla de LP de inicio rápido</a></td>
   <td>02 - LP - Gracias</td>
  </tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de página de aterrizaje</td>
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
   <td>Assets: aloja todos los recursos creativos 
<br/>(subcarpetas para Alertas y páginas de aterrizaje)</td>
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

![](assets/wr-yyyy-mm-web-request-program-1.png)

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Nombre de token</th>
   <th>Valor</th>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Request-Type}}</code></td>
   <td>Comuníquese con nosotros</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
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

## Prácticas recomendadas {#best-practices}

* Después de importar el programa de seminario web, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad para actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!IMPORTANT]
>
>Mis tokens que hacen referencia a una dirección URL no pueden contener los http:// u https://; de lo contrario, el vínculo no funcionará correctamente dentro del recurso.
