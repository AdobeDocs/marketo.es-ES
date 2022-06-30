---
unique-page-id: 11387674
description: 'Actualizaciones de la terminología de Marketo: Marketo Docs: Documentación del producto'
title: Actualizaciones de la terminología de Marketo
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 1%

---

# Actualizaciones de la terminología de Marketo {#updates-to-marketo-terminology}

Estamos realizando algunos cambios en nuestra plataforma, que afectarán a lo que se llama algunas cosas. Si tiene una nueva instancia de Marketo a partir de marzo de 2016 o si su empresa se ha renovado después de julio de 2016, es posible que ahora esté viendo la nueva terminología.

Aunque puede ver diferentes terminologías en la documentación de Marketo, tenga la seguridad de que todos los artículos se actualizarán pronto para reflejar estos cambios. Todas las instrucciones son las mismas.

Entonces, ¿qué ha cambiado?

## El posible cliente es ahora persona {#lead-is-now-person}

El mayor cambio es cambiar el nombre de Posibles clientes/Posibles clientes por Persona/Personas.

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

En algunos casos, la palabra &quot;posible cliente&quot; se elimina simplemente.

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

Tokens con la palabra &quot;lead&quot; en ellos **no están cambiando**. Pedimos disculpas por cualquier confusión; sin embargo, cambiar todos los tokens para que coincidan con la nueva terminología rompería un montón de tokens actualmente en uso. Por lo tanto, seguirá viendo tokens como &quot;`{{lead.First Name}}`.&quot; No hay tokens específicos de persona.

>[!NOTE]
>
>Ahí *es* un token llamado &quot;Notas de persona&quot;, sin embargo, ese token siempre estaba allí. Normalmente se utiliza para un campo de descripción en su CRM, si es que lo hace.

## Gestión de las actividades sobre el terreno {#field-management}

Los campos que contenían el término Posible cliente se han sustituido por Persona o la palabra Posible cliente se ha eliminado. Sin embargo, una excepción notable es el campo &quot;Propietario del posible cliente&quot;. Ahora se conoce como &quot;Propietario de ventas&quot;.

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
>Para obtener una lista completa de los nombres de campo afectados, visite esta [Artículo de asistencia](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target=&quot;_blank&quot;}.

## La personalización en tiempo real (RTP) ya es personalización web {#real-time-personalization-rtp-is-now-web-personalization}

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

| **[Personalización web](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target=&quot;_blank&quot;}** | Tiene su propio mosaico en la pantalla de inicio |
|---|---|
| **[Marketing web basado en cuentas](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target=&quot;_blank&quot;}** | Accesible a través del mosaico Personalización web |
| **[Redireccionamiento personalizado](https://docs.marketo.com/display/DOCS/Website+Retargeting){target=&quot;_blank&quot;}** | Accesible a través del mosaico Personalización web |
| **[Contenido predictivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target=&quot;_blank&quot;}** | Tiene su propio mosaico en la pantalla de inicio |

>[!NOTE]
>
>Los mosaicos visibles en la pantalla principal reflejarán los módulos comprados.

Gracias por su paciencia durante esta actualización.
