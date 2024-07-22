---
description: EM-AAAA-MM-DD-Envío de correo electrónico único - Documentos de Marketo - Documentación del producto
title: EM-AAAA-MM-DD-Envío de un solo correo electrónico
feature: Programs
exl-id: 58782d4c-658b-42cd-9ca3-fa53c7476e48
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 16%

---

# EM-AAAA-MM-DD-Envío de un solo correo electrónico {#em-yyyy-mm-dd-single-email-send}

Este ejemplo envía un solo correo electrónico utilizando un programa de correo electrónico de Marketo Engage. El correo electrónico puede incluir o no una prueba A/B.

Para obtener más ayuda sobre la estrategia o para personalizar un programa, ponte en contacto con el equipo de la cuenta de Adobe o visita la página de [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Correo electrónico</td> 
   <td>Miembro 01 
<br/>02-Participación-Éxito</td>
   <td>Incluido</td>
   <td>Correo electrónico</td>
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
   <td>01: Participación (éxito del programa)</td>
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
   <td>Informes</td>
  </tr>
 </tbody> 
</table>

![](assets/em-yyyy-mm-dd-single-email-send-1.png)

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

>[!NOTE]
>
>Recuerde actualizar los valores de Mi token en la plantilla de programa y cada vez que utilice el programa, según sea necesario.

>[!TIP]
>
>No olvide activar la campaña &quot;01-Engaged&quot; para realizar un seguimiento del éxito. Haga esto _antes_ de que su formulario esté activo y se envíen correos electrónicos.
