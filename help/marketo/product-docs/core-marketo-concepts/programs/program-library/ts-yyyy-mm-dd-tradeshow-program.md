---
description: Programa de ferias comerciales TS-AAAA-MM-DD - Documentos de Marketo - Documentación del producto
title: Programa de Ferias Comerciales TS-AAAA-MM-DD
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 569f61f15a9bdeb31b3a60b237f0c19aad68800a
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 14%

---

# Programa de Ferias Comerciales TS-AAAA-MM-DD {#ts-yyyy-mm-dd-tradeshow-program}

Este es un ejemplo de programa de feria comercial con invitaciones y correos electrónicos de seguimiento que utilizan un programa de eventos para Marketo Engage.

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
   <td>Evento</td> 
   <td>01-Invitado 
   <br/>02 - En lista de espera
   <br/>03-Registrados
   <br/>Stand visitado por 04 personas
   <br/>05 - Participación en el programa - Éxito
   <br/>06-Participación en el programa posterior - Éxito</td>
   <td>Inclusivo</td>
   <td>Evento</td>
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
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>01-Correo electrónico-Gracias</td>
  </tr>
   <tr> 
   <td>Correo electrónico</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>02a- Correo electrónico - Invitación</td>
  </tr>
  <tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento de correo electrónico</td>
  </tr>
  <tr> 
   <td>Informe local</td> 
   <td> </td>
   <td>Rendimiento del programa</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>00 - Programa de adquisición de capturas</td>
  </tr>
  <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>01 - Enviar invitación</td>
  </tr>
   <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>02 - Envío de correos electrónicos de seguimiento</td>
  </tr>
   <tr> 
   <td>Campaña inteligente</td> 
   <td> </td>
   <td>03 - Participación por correo electrónico de seguimiento (éxito)</td>
  </tr>
  <tr> 
   <td>Carpeta</td> 
   <td> </td>
   <td>Assets: aloja todos los recursos creativos 
<br/>(subcarpetas para correo electrónico y páginas de aterrizaje)</td>
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

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Nombre de token</th>
   <th>Valor</th>
  </tr>
  <tr> 
   <td>Archivo de calendario</td> 
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Haga doble clic para obtener detalles</td>
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
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr> 
   <td>Texto enriquecido</td> 
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Type}}</code></td>
   <td>Exposición comercial</td>
  </tr>
 </tbody> 
</table>

CAPTURA DE PANTALLA DEL PROGRAMA

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

* Después de importar el programa de seminario web, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad en las actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;03 - Participación por correo electrónico de seguimiento (éxito del programa)&quot; para realizar un seguimiento del éxito. Haga esto _antes_ se envían sus correos electrónicos.

>[!IMPORTANT]
>
>Mis tokens que hacen referencia a una dirección URL no pueden contener los http:// u https://; de lo contrario, el vínculo no funcionará correctamente dentro del recurso.
