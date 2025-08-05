---
description: Programa EV-AAAA-MM-DD-Event - Documentos de Marketo - Documentación del producto
title: Programa EV-AAAA-MM-DD-Evento
feature: Programs
exl-id: 999a82ae-6637-40bf-96c0-62183cb0a197
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 16%

---

# Programa EV-AAAA-MM-DD-Evento {#ev-yyyy-mm-dd-event-program}

Este es un ejemplo de programa de eventos con una página de registro, tres correos electrónicos de invitación y correos electrónicos de seguimiento que utilizan un programa de eventos de Marketo Engage. Adecuado para todos los eventos en los que se requieren registros, incluidos espectáculos itinerantes, almuerzos, cenas o presentaciones en eventos de ferias comerciales.

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
   <td>Evento</td>
   <td>01-Invitado
<br/>02 - En lista de espera
<br/>03-Registrados
<br/>04-No mostrar
<br/>05-Attended-Success</td>
   <td>Incluido</td>
   <td>Evento</td>
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
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>02a- Correo electrónico - Invitación</td>
  </tr>
  <tr>
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>02b - Correo electrónico - Recordatorio de invitación</td>
  </tr>
  <tr>
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>02c- Correo electrónico - Recordatorio de invitación Última oportunidad</td>
  </tr>
  <tr>
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>03 - Correo electrónico: recordatorio de asistencia</td>
  </tr>
  <tr>
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>04a - Correo electrónico - Seguimiento - Asistencia</td>
  </tr>
  <tr>
   <td>Correo electrónico</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Plantilla de correo electrónico de inicio rápido</a></td>
   <td>04b - Correo electrónico - Seguimiento - NoShow</td>
  </tr>
  <tr>
   <td>Página de destino</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Plantilla de LP de inicio rápido</a></td>
   <td>01a - LP - Registro</td>
  </tr>
  <tr>
   <td>Página de destino</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Plantilla de LP de inicio rápido</a></td>
   <td>01b - LP - Gracias</td>
  </tr>
  <tr>
   <td>Form</td>
   <td> </td>
   <td>Registro de eventos FM</td>
  </tr>
  <tr>
   <td>Informe local</td>
   <td> </td>
   <td>Desempeño de email</td>
  </tr>
  <tr>
   <td>Informe local</td>
   <td> </td>
   <td>Desempeño de página de destino</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>00 - Programa de adquisición de capturas</td>
  </tr>
  <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>01 - Registro del proceso</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>02a - Enviar invitación</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>02b - Enviar recordatorio de invitación</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>02c - Enviar invitación Última oportunidad</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>03 - Enviar recordatorio de asistencia</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>04 - Asistencia (éxito del programa)</td>
  </tr>
   <tr>
   <td>Campaña inteligente</td>
   <td> </td>
   <td>05 - Envío de correos electrónicos de seguimiento</td>
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
   <td>Informes</td>
  </tr>
 </tbody>
</table>

![](assets/ev-yyyy-mm-dd-event-program-1.png)

## Mis tokens incluidos {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo de token</th>
   <th>Nombre del token</th>
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
   <td><code>{{my.Content-Description}}</code></td>
   <td>Haga doble clic para obtener detalles
<br/><code><--My Content Description Here--></code>
<br/>Edite esta descripción de contenido en el nivel de programa, en la pestaña Mis tokens.
<br/>Aprenderá lo siguiente:
<li>Viñeta 1</li>
<li>Viñeta 2</li>
<li>Viñeta 3</li></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Event-Location-Line1}}</code></td>
   <td><code><--XYZ Hotel--></code></td>
  </tr>
   <tr>
   <td>Texto</td>
   <td><code>{{my.Event-Location-Line2}}</code></td>
   <td><code><--ABC Room--></code></td>
  </tr>
   <tr>
   <td>Texto</td>
   <td><code>{{my.Event-Location-Line3}}</code></td>
   <td><code><--1234 Anystreet--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Event-Location-Line4}}</code></td>
   <td><code><--Anytown, ZZ 99999--></code></td>
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
   <td>Evento en vivo</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.PageURL-Download}}</code></td>
   <td>my.DownloadURL?without=http://</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.PageURL-Registration}}</code></td>
   <td>my.RegistrationPageURL?without=http://</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>my.ThankYouPageURL?without=http://</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker1-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker1-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker2-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker2-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker3-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
 <tr>
   <td>Texto</td>
   <td><code>{{my.Speaker3-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
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

* Después de importar el programa de seminario web, mueva el formulario de un recurso local a un recurso global ubicado en Design Studio.
   * Reducir el número de formularios y utilizar más recursos globales de Design Studio permite una mayor escalabilidad en el diseño del programa y en el control administrativo. También proporciona flexibilidad en las actualizaciones de cumplimiento regulares para campos, idioma de inclusión, etc.

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;06 asistencia (éxito del programa)&quot; para realizar un seguimiento del éxito. Haga esto _antes_ de que su formulario esté activo y se envíen correos electrónicos.

>[!IMPORTANT]
>
>Mis tokens que hacen referencia a una dirección URL no pueden contener los http:// u https://; de lo contrario, el vínculo no funcionará correctamente dentro del recurso.
