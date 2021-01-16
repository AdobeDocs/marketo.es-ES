---
unique-page-id: 9437991
description: Déclencheur y Filtros para Campañas inteligentes móviles - Documentos de marketing - Documentación del producto
title: Déclencheur y Filtros para Campañas inteligentes móviles
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


# Déclencheur y Filtros para Campañas inteligentes móviles {#triggers-and-filters-for-mobile-smart-campaigns}

Puede configurar déclencheur y filtros para una campaña inteligente de aplicación móvil.

Para la mayoría de las actividades, hay un déclencheur, un filtro y un filtro de inactividad. Use filtros de inactividad para rastrear una acción, como tocar una notificación push, que *no se produjo*.

* Se instaló o se instaló la aplicación móvil
* Se abrió o se abrió la aplicación móvil
* Tiene o tiene Actividad de aplicación móvil
* Tiene o ha tenido una sesión de aplicación móvil
* Toque/toque notificación push móvil

Solo hay filtros para esta actividad:

* Notificación push de envío: filtro y filtro de inactividad

Busque **aplicación móvil** en el panel derecho para realizar la lista de todos los filtros y déclencheur de aplicaciones móviles.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Restricciones {#constraints}

Utilice restricciones con déclencheur y filtros para ordenar los datos con mayor profundidad.

![](assets/image2015-8-17-12-3a6-3a33.png)

Todos los déclencheur y filtros, excepto la notificación push de envío, contienen estas dos restricciones estándar:

* Tipo de dispositivo: iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, smartphone Android, tablet Android, Desconocido (se trata de una lista preestablecida)

* Plataforma: iPhone o Android

Algunos déclencheur y filtros oferta restricciones adicionales, como:

* Versión de la aplicación: una forma de destinatario para personas que no están en la versión más reciente. Por ejemplo, si la última versión de la aplicación es 2.0, puede utilizarla para buscar personas que NO estén en la versión 2.0 de la aplicación

* Instalar origen: actualmente, la única opción es API

* Configuración regional: la configuración del dispositivo

* Aplicación móvil: el nombre de una aplicación específica. Útil para especificar si tiene más de uno

* Versión de la plataforma: la versión del sistema operativo

* Duración de la sesión (segundos): tiempo de sesión cuando la aplicación está en primer plano

* Es push habilitado: **True** significa que se pueden enviar notificaciones push. **** Falsemans que no pueden; por ejemplo, es posible que la persona haya exclusión de recibir notificaciones push

## Déclencheur y Filtros {#triggers-and-filters}

**Tiene una aplicación móvil**

Utilice este filtro para averiguar qué personas han tenido la aplicación instalada alguna vez. Esto solo está disponible como filtro.

>[!NOTE]
>
>El filtro buscará tanto las instalaciones actuales como las anteriores, ya que Marketing no realiza el seguimiento de las desinstalaciones de la aplicación.

**Restricciones**: Tipo de dispositivo, Plataforma, Aplicación móvil, Versión de la aplicación móvil, Tipo de dispositivo, Origen de instalación, Está habilitado para inserción y Configuración regional

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>Se recomienda especificar Has Mobile App = true y Is Push Enabled = true, así como el nombre de la aplicación móvil al definir la lista inteligente de quién debe recibir una notificación push.

Se instaló o se instaló la aplicación móvil

* Aplicación móvil instalada: déclencheur

* Aplicación móvil instalada: filtro

* NO se instaló la aplicación móvil: filtro de inactividad

**Restricciones**: Tipo de dispositivo, Plataforma, Versión de la aplicación, Configuración regional e Instalar origen

![](assets/image2015-8-17-13-3a11-3a3.png)

Se abrió o se abrió la aplicación móvil

* Aplicación móvil abierta: déclencheur

* Aplicación móvil abierta: filtro

* NO se abrió la aplicación móvil: filtro de inactividad

**Restricciones**: Tipo y plataforma de dispositivo

![](assets/image2015-8-17-13-3a13-3a55.png)

Tiene o tiene Actividad de aplicación móvil

Esto proporciona una manera eficaz de rastrear la actividad móvil personalizada. Tendrá que trabajar con su desarrollador para configurar el seguimiento [para Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android) y [para iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Tiene Actividad de aplicación móvil: déclencheur

* Con Actividad de aplicación móvil: filtro

* NO tenía Actividad de aplicación móvil: filtro de inactividad

**Restricciones**: Tipo y plataforma de dispositivo, más cinco adicionales:

* Acción: actividad móvil personalizada

* Tipo de acción: campo de texto (opcional) utilizado para categorizar varias acciones

* Detalles de la acción: campo de texto (opcional) que proporciona información adicional sobre una acción

* Métrica de acción: campo numérico (opcional) que proporciona información adicional sobre una acción (por ejemplo, precio)

* Duración de la acción (segundos): campo numérico (opcional) que se puede utilizar para capturar cuánto tiempo tardó un usuario en completar una acción

Las restricciones de acción le permiten utilizar el déclencheur y los filtros para realizar un seguimiento muy atento de la actividad móvil.

>[!NOTE]
>
>**Ejemplo**
>
>En el tipo de acción *Shopping*, se muestra una acción muy específica, con las otras restricciones que la definen:
>
>* Compró una camisa
   >   * Era rojo
   >   * Costó 30 dólares
   >   * Se tardaron 20 segundos en comprar


Este es el aspecto del filtro en MarketingTo:

![](assets/image2015-8-17-13-3a16-3a12.png)

>[!NOTE]
>
>**Ejemplo**
>
>Puede tener varias acciones en el mismo tipo de acción. De hecho, su experiencia de compra normal puede involucrar varias columnas en Compras! ¿Qué tal unos calcetines para ir con eso?
>
>| Tipo de acción | Compras | Compras |
>|---|---|---|
>| Acción | Camisa comprada | Pantalones comprados |
>| Detalles de la acción | Color | Color |
>| Métrica de acción | Precio | Precio |


**Tiene o ha tenido una sesión de aplicación móvil**

* Tiene sesión de aplicación móvil: déclencheur

* Tenía sesión de aplicación móvil: filtro

* NO tuvo sesión de aplicación móvil: filtro de inactividad

**Restricciones**: Tipo de dispositivo, Plataforma y Duración de la sesión (segundos)

![](assets/image2015-8-17-13-3a18-3a34.png)

Tapas/notificaciones push de toque

* Notificaciones push de toques: déclencheur

* Notificación push de toque: filtro

* Notificación push NO capturada: filtro de inactividad

**Restricciones**: Tipo de dispositivo, Plataforma, Versión de aplicación móvil, Notificación push y Versión de plataforma

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Utilice el filtro de inactividad Notificación push no capturada para buscar personas que no tocaron una notificación push recientemente enviada a ellas, de modo que pueda realizar un seguimiento por correo electrónico.

**Notificación push** de envíoEsta actividad solo está disponible como filtro.

* Se envió notificación push - filtro

* NO se envió la notificación push - filtro de inactividad

**Restricciones**: Notificación push y aplicación móvil

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!MORELIKETHIS]
>
>* [Añadir una restricción a un filtro de Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Usar Filtros de inactividad en una Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

