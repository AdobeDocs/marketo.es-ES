---
unique-page-id: 11387674
description: Actualizaciones en la terminología de Marketo - Docs de Marketo - Documentación del producto
hide: true
hidefromtoc: true
title: Actualizaciones en la terminología de Marketo
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '328'
ht-degree: 100%

---

# Actualizaciones en la terminología de Marketo {#updates-to-marketo-terminology}

Estamos realizando algunos cambios en nuestra plataforma, lo que afectará a la denominación de algunos elementos. Si tiene una nueva instancia de Marketo desde marzo de 2016 o si su compañía ha renovado después de julio de 2016, podrá ver la nueva terminología ahora.

Tal vez vea una terminología diferente en la documentación de Marketo, pero le garantizamos que todos los artículos se actualizarán lo antes posible para reflejar estos cambios. Todas las instrucciones son las mismas.

Entonces, ¿qué ha cambiado?

## El posible cliente ahora es una persona {#lead-is-now-person}

El cambio más importante es el cambio de nombre de Posible cliente/Posibles clientes a Persona/Personas.

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

En algunos casos, simplemente se ha eliminado la palabra «Posible cliente».

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

El posible cliente y la persona **son lo mismo**.

## Tókenes {#tokens}

Los tókenes que contienen la palabra Posible cliente **no cambian**. Lamentamos cualquier confusión; sin embargo, cambiar todos los tókenes para que coincidan con la nueva terminología rompería muchos de los que se utilizan actualmente. Por lo tanto, seguirá viendo tókenes como «`{{lead.First Name}}`» No hay tókenes específicos para cada persona.

>[!NOTE]
>
>*Hay* un token llamado «Notas de la persona», sin embargo ese token siempre estuvo ahí. Normalmente se utiliza para un campo de descripción en su CRM, si es que lo hay.

## Administración de campos {#field-management}

Los campos que contenían el término Posible cliente se han sustituido por Persona o se ha eliminado la palabra Posible cliente. Sin embargo, una excepción importante es el campo «Propietario de posibles clientes». Ahora se conoce como «Propietario de ventas».

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
>Para obtener una lista completa de los nombres de campo afectados, visite este [Artículo de asistencia técnica](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## La personalización en tiempo real (RTP) ahora es Personalización web {#real-time-personalization-rtp-is-now-web-personalization}

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
| **[Account-based Web Marketing](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Accesible a través del mosaico de personalización web |
| **[Resegmentación personalizada](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Accesible a través del mosaico de personalización web |
| **[Contenido predictivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Tiene su propio mosaico en la pantalla principal |

>[!NOTE]
>
>Los mosaicos visibles en la pantalla principal reflejarán los módulos comprados.

Gracias por su paciencia durante esta actualización.
