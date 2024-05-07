---
unique-page-id: 11387674
description: Actualizaciones en la terminología de Marketo - Documentos de Marketo - Documentación del producto
hide: true
hidefromtoc: true
title: Actualizaciones en la terminología de Marketo
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 2%

---

# Actualizaciones en la terminología de Marketo {#updates-to-marketo-terminology}

Estamos haciendo algunos cambios en nuestra plataforma, que afectarán cómo se llaman algunas cosas. Si tiene una nueva instancia de Marketo a partir de marzo de 2016 o si su empresa renovó después de julio de 2016, es posible que esté viendo la nueva terminología ahora.

Aunque puede ver una terminología diferente en la documentación de Marketo, puede estar seguro de que todos los artículos se actualizarán pronto para reflejar estos cambios. Todas las instrucciones son las mismas.

Entonces, ¿qué ha cambiado?

## El posible cliente ahora es una persona {#lead-is-now-person}

El cambio más grande es el cambio de nombre de Posible cliente/Posible cliente a Persona/Personas.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antiguo</strong></td> 
   <td><strong>Nuevo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

En algunos casos, simplemente se elimina la palabra &quot;posible cliente&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antiguo</strong></td> 
   <td><strong>Nuevo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Posible cliente y persona **son lo mismo**.

## Tokens {#tokens}

Tokens con la palabra lead en ellos **no están cambiando**. Lamentamos cualquier confusión; sin embargo, cambiar todos los tokens para que coincidan con la nueva terminología rompería muchos de los tokens que se utilizan actualmente. Por lo tanto, seguirá viendo tokens como &quot;`{{lead.First Name}}`.&quot; No hay tokens específicos de persona.

>[!NOTE]
>
>Ahí *es* un token denominado &quot;Notas de persona&quot;; sin embargo, ese token siempre estaba allí. Normalmente se utiliza para un campo de descripción en su CRM, si es que lo hay.

## Administración de campos {#field-management}

Los campos que contenían el término Posible cliente se han sustituido por Persona o se ha eliminado la palabra Posible cliente. Sin embargo, una excepción notable es el campo &quot;Propietario principal&quot;. Ahora se conoce como &quot;Propietario de ventas&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antiguo</strong></td> 
   <td><strong>Nuevo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Para obtener una lista completa de los nombres de campo afectados, visite esta [Artículo de soporte](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## La personalización en tiempo real (RTP) ahora es personalización web {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antiguo</strong></td> 
   <td><strong>Nuevo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Además del cambio de nombre, ahora consta de cuatro aplicaciones independientes:

| **[Personalización web](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Tiene su propio mosaico en la pantalla principal |
|---|---|
| **[Marketing web basado en cuentas](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Accesible mediante el mosaico Personalización web |
| **[Redireccionamiento personalizado](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Accesible mediante el mosaico Personalización web |
| **[Contenido predictivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Tiene su propio mosaico en la pantalla principal |

>[!NOTE]
>
>Los mosaicos visibles en la pantalla de inicio reflejarán los módulos comprados.

Gracias por su paciencia durante esta actualización.
