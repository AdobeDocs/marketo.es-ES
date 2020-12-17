---
unique-page-id: 11373011
description: Transición al Editor de correo electrónico 2.0 - Documentos de marketing - Documentación del producto
title: Transición al Editor de correo electrónico 2.0
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Transición al Editor de correo electrónico 2.0 {#transitioning-to-email-editor}

A partir de la [versión del 19 de junio](../../../../release-notes/2016/release-notes-spring-16.md), todas las suscripciones de Marketing se han transferido al Editor de correo electrónico 2.0. [Más información](https://nation.marketo.com/docs/DOC-7038) sobre la obsolescencia del Editor de correo electrónico 1.0.

Los correos electrónicos y las plantillas de correo electrónico de la suscripción deben tener un número de versión. La versión se encuentra en la página de resumen del recurso.

![](assets/five-5.png)

De forma predeterminada, todos los correos electrónicos y las plantillas de correo electrónico existentes se marcarán como v1.0 si se crearon antes de la versión de primavera del 16 o después de la versión cuando el Editor de correo electrónico 2.0 esté deshabilitado. Con el Editor de correo electrónico 2.0 ahora habilitado automáticamente, verá el siguiente comportamiento:

* Cuando cree un nuevo mensaje de correo electrónico, se mostrará el [Selector de plantilla de correo electrónico](email-template-picker-overview.md) y podrá elegir una plantilla de correo electrónico v2.0.
* Siempre que cree o edite un correo electrónico con el Editor de correo electrónico 2.0, el correo electrónico resultante **siempre** se marcará como v2.0 (incluso si utilizó una plantilla de correo electrónico v1.0).

Si la suscripción tiene correos electrónicos v1.0 antes de pasar al Editor de correo electrónico 2.0, experimentará el siguiente comportamiento en función del estado actual del recurso:

**Aprobado** : al hacer clic en &quot;Editar borrador&quot; se creará un borrador v2.0 del correo electrónico aprobado. Si luego aprueba el borrador v2.0, el estado aprobado del correo electrónico pasará a ser v2.0 y no hay forma de volver a la versión 1.0.\
**Borrador** : al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente ese borrador como v2.0. En este punto, no será posible descartar y revertir a v1.0 porque no hay ninguna versión aprobada del recurso.\
**Aprobado con borrador** : al hacer clic en &quot;Editar borrador&quot; se marcará automáticamente ese borrador como v2.0. Debido a esto, tampoco hay forma de volver a la versión 1.0 del borrador.

Si su suscripción tiene plantillas de correo electrónico v1.0 antes de pasar al Editor de correo electrónico 2.0, experimentará el siguiente comportamiento:

**Aprobado** : al hacer clic en &quot;Editar borrador&quot; se creará un borrador v2.0 de la plantilla de correo electrónico existente.\
**Borrador** : al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente ese borrador como v2.0. En este punto, no sería posible descartar y revertir a v1.0 porque no hay ninguna versión aprobada del recurso.\
**Aprobado con borrador** : al hacer clic en &quot;Editar borrador&quot; se marcará automáticamente ese borrador como v2.0. Debido a esto, tampoco hay forma de volver a la versión 1.0 del borrador.

Si aprueba una plantilla de correo electrónico que antes era v1.0 (en cualquiera de los estados anteriores), verá el siguiente comportamiento:

Para los correos electrónicos v1.0 existentes que utilizaban la plantilla (anteriormente v1.0):\
**Correo electrónico**  v1.0 aprobado: se creará un borrador v2.0 para este mensaje de correo electrónico, que seguirá usando la plantilla v2.0 recién aprobada. También recibirá cualquier cambio de plantilla.\
**Correo electrónico**  de borrador v1.0: el borrador permanecerá v1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá los cambios de plantilla.\
**Aprobado con borrador v1.0 email** : el borrador permanecerá v1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá los cambios de plantilla.

Para los correos electrónicos v2.0 existentes que utilizaban la plantilla (anteriormente v1.0):\
**Correo electrónico**  v2.0 aprobado: se creará un borrador v2.0 para este mensaje de correo electrónico, que seguirá &quot;usando&quot; la plantilla recién aprobada y recibirá los cambios de plantilla.\
**Correo electrónico**  de borrador v2.0: el borrador permanecerá tal cual (v2.0) y recibirá los cambios de plantilla.\
**Aprobado con borrador v2.0 email** : el borrador permanecerá tal cual (v2.0) y recibirá los cambios de plantilla.

>[!CAUTION]
>
>Si alguna vez aprueba el borrador v2.0 de una plantilla de correo electrónico v1.0, la plantilla pasará a ser v2.0. No hay **forma** de revertirlo a v1.0.

Aspectos a tener en cuenta

* Los correos electrónicos aprobados **nunca** se modifican.

* Las plantillas de correo electrónico aprobadas **nunca** cambian.

* En algunos **casos poco comunes**, no se puede abrir un correo electrónico v1.0 en el Editor de correo electrónico 2.0. Si esto sucede, descarte el borrador y póngase en contacto con la asistencia técnica de marketing.

>[!MORELIKETHIS]
>
>* [Información general del editor de correo electrónico 2.0](email-editor-v2-0-overview.md)
>* [Sintaxis de la plantilla de correo electrónico](email-template-syntax.md)

>



