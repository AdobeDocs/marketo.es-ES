---
unique-page-id: 9437991
description: 'Déclencheur y filtros para campañas móviles inteligentes: Documentos de Marketo, documentación del producto'
title: Déclencheur y filtros para campañas inteligentes móviles
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 1%

---

# Déclencheur y filtros para campañas inteligentes móviles {#triggers-and-filters-for-mobile-smart-campaigns}

Puede configurar déclencheur y filtros para una aplicación móvil o campaña inteligente.

Para la mayoría de las actividades, hay un déclencheur, un filtro y un filtro de inactividad. Utilice filtros de inactividad para rastrear una acción, como pulsar una notificación push, que _no lo hice_ suceda.

* La Aplicación Móvil Está/Estaba Instalada
* Se Ha Abierto/Se Ha Abierto La Aplicación Móvil
* Tiene/Tuvo Actividad De Aplicación Móvil
* Tiene/tuvo sesión de aplicación móvil
* Notificaciones push móviles con toque o toque

Solo hay filtros para esta actividad:

* Se envió la notificación push: filtro y filtro de inactividad

Busque &quot;aplicación móvil&quot; en el panel derecho para ver una lista de todos los déclencheur y filtros de aplicaciones móviles.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Restricciones {#constraints}

Utilice restricciones con déclencheur y filtros para ordenar aún más los datos.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Todos los déclencheur, excepto la notificación push de tipo Se envió, contienen estas dos restricciones estándar:

* Tipo de dispositivo: iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, smartphone Android, tableta Android, desconocido (esta es una lista preestablecida)

* Platform: iPhone o Android

Algunos déclencheur ofrecen restricciones adicionales, como las siguientes:

* Versión de la aplicación: una forma de dirigirse a personas que no están en la versión más reciente. Por ejemplo, si la versión más reciente de la aplicación es 2.0, puede utilizarla para buscar personas que NO estén en la versión 2.0 de la aplicación

* Instalar origen: actualmente, la única opción es API

* Configuración regional: la configuración del dispositivo

* Aplicación móvil: nombre de una aplicación específica. Útil para especificar si tiene más de uno

* Versión de plataforma: la versión del sistema operativo

* Duración de la sesión (segundos): tiempo de la sesión cuando la aplicación está en primer plano

* ¿Está activada la push? **Verdadero** significa que se pueden enviar notificaciones push. **Falso** significa que no pueden; por ejemplo, la persona puede haber optado por no recibir notificaciones push

## Déclencheur y filtros {#triggers-and-filters}

**Tiene aplicación móvil**

Utilice este filtro para averiguar todas las personas que han instalado su aplicación en algún momento. Esto solo está disponible como filtro.

>[!NOTE]
>
>El filtro encontrará instalaciones actuales y anteriores, ya que Marketo no realiza un seguimiento de las desinstalaciones de aplicaciones.

**Restricciones** : Tipo de dispositivo, plataforma, aplicación móvil, versión de aplicación móvil, tipo de dispositivo, origen de instalación, con push habilitado y configuración regional

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>Se recomienda especificar Has Mobile App = true y Is Push Enabled = true, así como el nombre de la aplicación móvil al definir la lista inteligente de destinatarios que deben recibir una notificación push.

La Aplicación Móvil Está/Estaba Instalada

* Aplicación móvil instalada: déclencheur

* Se ha instalado la aplicación móvil: filtro

* No se ha instalado la aplicación móvil: filtro de inactividad

**Restricciones** : Tipo de dispositivo, plataforma, versión de aplicación, configuración regional y origen de instalación

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

Se Ha Abierto/Se Ha Abierto La Aplicación Móvil

* La aplicación móvil está abierta: déclencheur

* Se ha abierto la aplicación móvil: filtro

* No se ha abierto la aplicación móvil: filtro de inactividad

**Restricciones** - Tipo de dispositivo y plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Tiene/Tuvo Actividad De Aplicación Móvil

Proporcionan una forma eficaz de realizar un seguimiento de la actividad móvil personalizada. Deberá trabajar con el desarrollador para configurar el seguimiento [para Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android){target="_blank"} and [for iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios){target="_blank"}.

* Tiene actividad de aplicación móvil: déclencheur

* Actividad de aplicación móvil principal: filtro

* NO tuvo actividad de aplicación móvil: filtro de inactividad

**Restricciones** - Tipo de dispositivo, Plataforma, Versión de aplicación móvil, Configuración regional, Versión de plataforma, además de cinco adicionales:

* Acción: actividad móvil personalizada

* Tipo de acción (opcional) Campo de texto utilizado para categorizar varias acciones

* Detalles de la acción: campo de texto (opcional) que proporciona información adicional sobre una acción

* Métrica de acción: campo numérico (opcional) que proporciona información adicional sobre una acción (por ejemplo, el precio)

* Duración de la acción (segundos): campo numérico (opcional) que se puede utilizar para capturar cuánto tiempo tardó un usuario en completar una acción

Las restricciones de acción permiten utilizar el déclencheur y los filtros para realizar un seguimiento muy atento de la actividad móvil.

>[!NOTE]
>
>**Ejemplo**
>
>En el tipo de acción de *Compras* Sin embargo, esta es una acción muy específica, con las otras restricciones que la definen:
>
>* Compré una camisa
>   * Era rojo
>   * Costó 30 dólares
>   * Tomó 20 segundos para comprar

Este es el aspecto del filtro en Marketo:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Ejemplo**
>
>Puede tener varias acciones bajo el mismo tipo de acción. De hecho, su experiencia de compra normal puede implicar varias columnas bajo Compras! ¿Qué tal unos calcetines para acompañar eso?
>
>| Tipo de acción | Compras | Compras |
>|---|---|---|
>| Acción | Comprado camisa | Pantalones adquiridos |
>| Detalles de la acción | Color | Color |
>| Métrica de la acción | Precio | Precio |

**Tiene/tuvo sesión de aplicación móvil**

* Tiene sesión de aplicación móvil: déclencheur

* Tuvo una sesión de aplicación móvil: filtro

* NO se ha tenido la sesión de la aplicación móvil: filtro de inactividad

**Restricciones** : Tipo de dispositivo, plataforma y duración de la sesión (segundos)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Notificaciones push con toque o toque

* Déclencheur de notificaciones push de toques

* Notificación push pulsada: filtro

* Notificación push sin pulsar: filtro de inactividad

**Restricciones** : Tipo de dispositivo, Plataforma, Versión de aplicación móvil, Notificación push y Versión de plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Utilice el filtro de inactividad de notificaciones push sin pulsar para buscar personas que no hayan pulsado una notificación push que se les haya enviado recientemente, de modo que pueda realizar el seguimiento por correo electrónico.

**Se Envió La Notificación Push** Esta actividad solo está disponible como filtro.

* Se envió la notificación push: filtro

* NO se ha enviado notificación push: filtro de inactividad

**Restricciones** - Notificación push y aplicación móvil

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Agregar una restricción a un filtro de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}
>* [Uso de filtros de inactividad en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
