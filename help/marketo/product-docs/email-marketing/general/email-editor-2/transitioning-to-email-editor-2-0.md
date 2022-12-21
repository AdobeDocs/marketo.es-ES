---
unique-page-id: 11373011
description: 'Transición al Editor de correo electrónico 2.0: Marketo Docs: documentación del producto'
title: Transición al Editor de correo electrónico 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
source-git-commit: 64ff6900a761b9df796a9a7f417cca1ddc628cce
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Transición al Editor de correo electrónico 2.0 {#transitioning-to-email-editor}

Desde la versión del 19 de junio, todas las suscripciones a Marketo se han transferido a Email Editor 2.0. [Más información](https://nation.marketo.com/docs/DOC-7038) acerca de la desaprobación del Editor de correo electrónico 1.0.

Los correos electrónicos y las plantillas de correo electrónico de la suscripción deben tener un número de versión. La versión se puede encontrar en la página de resumen del recurso.

![](assets/five-5.png)

De forma predeterminada, todos los correos electrónicos y plantillas de correo electrónico existentes se marcarán como v1.0 si se crearon antes de la versión de primavera del 16 o después de la versión cuando el Editor de correo electrónico 2.0 está desactivado. Con el Editor de correo electrónico 2.0 ahora habilitado automáticamente, verá el siguiente comportamiento:

* Cuando crea un nuevo correo electrónico, la variable [Selector de plantilla de correo electrónico](email-template-picker-overview.md) se mostrará y podrá elegir una plantilla de correo electrónico v2.0.
* Siempre que cree o edite un correo electrónico con el Editor de correo electrónico 2.0, el correo electrónico resultante **always** se marque como v2.0 (aunque haya utilizado una plantilla de correo electrónico v1.0).

Si la suscripción tiene correos electrónicos v1.0 antes de pasar al Editor de correo electrónico 2.0, experimentará el siguiente comportamiento en función del estado actual del recurso:

**Aprobado** - Al hacer clic en Editar borrador se creará un borrador v2.0 del correo electrónico aprobado. Si a continuación aprueba el borrador v2.0, el estado aprobado del correo electrónico pasa a ser v2.0 y no hay forma de volver a v1.0.\
**Borrador** - Al hacer clic en &quot;Editar borrador&quot; se marcará automáticamente ese borrador como v2.0. En este punto, no será posible descartar y revertir a v1.0 porque no hay una versión aprobada del recurso.
**Aprobado con borrador** - Al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente ese borrador como v2.0. Debido a esto, tampoco hay forma de revertir el borrador a v1.0.

Si la suscripción tiene plantillas de correo electrónico v1.0 antes de pasar al Editor de correo electrónico 2.0, experimentará el siguiente comportamiento:

**Aprobado** - Al hacer clic en Editar borrador se creará un borrador v2.0 de la plantilla de correo electrónico existente.
**Borrador** - Al hacer clic en &quot;Editar borrador&quot; se marcará automáticamente ese borrador como v2.0. En este punto, no sería posible descartar y volver a v1.0 porque no hay una versión aprobada del recurso.
**Aprobado con borrador** - Al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente ese borrador como v2.0. Debido a esto, tampoco hay forma de revertir el borrador a v1.0.

Si aprueba una plantilla de correo electrónico que anteriormente era v1.0 (en cualquiera de los estados anteriores), verá el siguiente comportamiento:

Para correos electrónicos v1.0 existentes que utilizaban la plantilla (anteriormente v1.0):\
**Correo electrónico v1.0 aprobado** - Se creará un borrador v2.0 para este correo electrónico, que seguirá usando la plantilla v2.0 recién aprobada. También recibirá cualquier cambio en la plantilla.\
**Borrador de correo electrónico v1.0** - El borrador permanecerá v1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá cualquier cambio en la plantilla.\
**Aprobado con el correo electrónico de Borrador v1.0** - El borrador permanecerá v1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá cualquier cambio en la plantilla.

Para correos electrónicos v2.0 existentes que utilizaban la plantilla (anteriormente v1.0):\
**Correo electrónico aprobado v2.0** - Se creará un borrador v2.0 para este correo electrónico, que seguirá &quot;usando&quot; la plantilla recién aprobada, y recibirá cualquier cambio en la plantilla.\
**Borrador de correo electrónico v2.0** - El borrador permanecerá tal cual (v2.0) y recibirá cualquier cambio en la plantilla.\
**Aprobado con el correo electrónico de Borrador v2.0** - El borrador permanecerá tal cual (v2.0) y recibirá cualquier cambio en la plantilla.

>[!CAUTION]
>
>Si alguna vez aprueba el borrador v2.0 de una plantilla de correo electrónico v1.0, la plantilla pasará a ser v2.0. Hay **no hay manera** para volver a la versión 1.0.

Aspectos a tener en cuenta

* Los correos electrónicos aprobados son **never** se ha modificado.

* Las plantillas de correo electrónico aprobadas son **never** se ha modificado.

* En **raros** En los casos, no se puede abrir un correo electrónico v1.0 en el Editor de correo electrónico 2.0. Si esto ocurre, descarte el borrador y póngase en contacto con el soporte técnico de Marketo.

>[!MORELIKETHIS]
>
>* [Información general del Editor de correo electrónico 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintaxis de la plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)

