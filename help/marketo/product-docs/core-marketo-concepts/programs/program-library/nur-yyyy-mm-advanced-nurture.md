---
description: NUR-AAAA-MM-Advanced Nurture - Documentos de Marketo - Documentación del producto
title: NUR-AAAA-MM-Nutrición avanzada
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 15%

---

# NUR-AAAA-MM-Nutrición avanzada {#nur-yyyy-mm-advanced-nurture}

Este es un ejemplo de programas de nutrición avanzados que utilizan el Programa de participación de Marketo Engage. Los programas de correo electrónico anidados impiden que las personas reciban contenido que ya han consumido o controlan el tipo de contenido que deben consumir en cada flujo. Los informes de atribución se pueden ejecutar para cada programa de correo electrónico anidado individual. Canales: &quot;Nutrir&quot; y un canal &quot;Nutrir correo electrónico&quot; dedicado para los programas de correo electrónico anidados envía un correo electrónico de newsletter mediante un programa de correo electrónico de Marketo Engage. El correo electrónico puede incluir o no una prueba A/B.

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
   <td>Acompañamiento</td>
   <td>01 - Miembro
<br/>02 - Participado - Correcto</td>
   <td>Incluido</td>
   <td>Participación</td>
  </tr>
  <tr>
   <td>Nutrir correo electrónico</td>
   <td>01 - Omitir
<br/>02 - Enviado
<br/>03 - Comprometido - Correcto</td>
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
   <td>Desempeño de email</td>
  </tr>
  <tr>
   <td>Informe local</td>
   <td> </td>
   <td>Desempeño de vínculo de email</td>
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
   <td>Assets (contener programas anidados y las carpetas de recursos también se encuentran en programas anidados para contener correos electrónicos)</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Programas anidados (se encuentra en la carpeta Assets)</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Campañas: aloja todas las campañas inteligentes en el programa principal Nutrir y las carpetas de campaña también se encuentran en cada programa anidado</td>
  </tr>
  <tr>
   <td>Carpeta</td>
   <td> </td>
   <td>Informes</td>
  </tr>
 </tbody>
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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

* Considere la posibilidad de actualizar las plantillas del programa importado para utilizar plantillas con marca actual o actualizar la plantilla recién importada para reflejar su marca añadiendo un fragmento o la información del logotipo/pie de página correspondiente.

* Considere la posibilidad de actualizar la convención de nombres de este ejemplo de programa para que se ajuste a la convención de nombres.

* Asegúrese de que dispone de reglas para pausar y reanudar la cadencia de nutrición. Estas campañas inteligentes deben activarse o programarse antes de activar el programa de participación.

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;04 - Participación (éxito del programa)&quot; para realizar el seguimiento del éxito. Haz esto _antes_ de que se envíen tus correos electrónicos.
