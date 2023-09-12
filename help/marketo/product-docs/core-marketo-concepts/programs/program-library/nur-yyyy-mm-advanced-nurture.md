---
description: NUR-AAAA-MM-Advanced Nurture - Documentos de Marketo - Documentación del producto
title: NUR-AAAA-MM-Nutrición avanzada
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 13%

---

# NUR-AAAA-MM-Nutrición avanzada {#nur-yyyy-mm-advanced-nurture}

Este es un ejemplo de programas avanzados de nutrición que utilizan el programa de participación del Marketo Engage. Los programas de correo electrónico anidados impiden que las personas reciban contenido que ya han consumido o controlan el tipo de contenido que deben consumir en cada flujo. Los informes de atribución se pueden ejecutar para cada programa de correo electrónico anidado individual. Canales: &quot;Nutrir&quot; y un canal &quot;Nutrir correo electrónico&quot; dedicado para los programas de correo electrónico anidados envía un correo electrónico de newsletter mediante un programa de correo electrónico de Marketo Engage. El correo electrónico puede incluir o no una prueba A/B.

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
   <td>Cultivar</td> 
   <td>01 - Miembro 
<br/>02 - Participación - Éxito</td>
   <td>Inclusivo</td>
   <td>Compromiso</td>
  </tr>
  <tr> 
   <td>Nutrir correo electrónico</td> 
   <td>01 - Omitir 
<br/>02 - Enviado
<br/>03 - Participación - Éxito</td>
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
   <td>Programa anidado</td> 
   <td> </td>
   <td>01 - Tema X</td>
  </tr>
  <tr> 
   <td>Programa anidado</td> 
   <td> </td>
   <td>02 - Tema Y</td>
  </tr>
  <tr> 
   <td>Programa anidado</td> 
   <td> </td>
   <td>03 - Tema Z</td>
  </tr>
  <tr> 
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>01 - Correo electrónico (activo en programas anidados)</td>
  </tr>
   <tr> 
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>02 - Correo electrónico (activo en programas anidados)</td>
  </tr>
   <tr> 
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>03 - Correo electrónico (activo en programas anidados)</td>
  </tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de correo electrónico</td>
  </tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de vínculo de correo electrónico</td>
  </tr>
  <tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>01 - Añadir a Nutrir</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>02 - Pausar Nutrición</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>03 - Reanudar la nutrición</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>04 - Participación (éxito del programa)</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>00 - Omitir correo electrónico (ubicado en cada programa anidado)</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>01 - Enviar correo electrónico (ubicado en cada programa anidado)</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>02 - Participación-éxito (ubicado en cada programa anidado)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Los recursos (contienen programas anidados y las carpetas de recursos también se encuentran en programas anidados para contener correos electrónicos)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Programas anidados (se encuentra en la carpeta Recursos)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Campañas: aloja todas las campañas inteligentes en el programa principal Nutrir y las carpetas de campaña también se encuentran en cada programa anidado</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Informes de  </td>
  </tr>
 </tbody> 
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

* Asegúrese de que dispone de reglas para pausar y reanudar la cadencia de nutrición. Estas campañas inteligentes deben activarse o programarse antes de activar el programa de participación.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;04 - Participación (éxito del programa)&quot; para realizar el seguimiento del éxito. Haga esto _antes_ se envían sus correos electrónicos.
