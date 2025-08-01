---
unique-page-id: 11373011
description: 'Transición al Editor de correo electrónico 2.0: documentos de Marketo, documentación del producto'
title: Transición al Editor de correo electrónico 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Pasando a [!DNL Email Editor 2.0] {#transitioning-to-email-editor}

En la versión de junio de 2019, todas las suscripciones de Marketo se habían transferido a [!DNL Email Editor 2.0]. [Más información](https://nation.marketo.com/docs/DOC-7038) sobre la desaprobación de [!DNL Email Editor 1.0].

Los correos electrónicos y las plantillas de correo electrónico de su suscripción deben tener un número de versión. La versión se encuentra en la página de resumen del recurso.

![](assets/five-5.png)

De forma predeterminada, todos los correos electrónicos y plantillas de correo electrónico existentes se marcarán como v1.0 si se crearon antes de la versión de primavera de 16 o después de la versión cuando el Editor de correo electrónico 2.0 esté deshabilitado. Con el Editor de correo electrónico 2.0 ahora habilitado automáticamente, verá el siguiente comportamiento:

* Al crear un correo electrónico nuevo, se mostrará [Selector de plantilla de correo electrónico](email-template-picker-overview.md) y podrá elegir una plantilla de correo electrónico v2.0.
* Cada vez que cree o edite un correo electrónico con [!DNL Email Editor 2.0], el correo electrónico resultante **siempre** se marcará como v2.0 (incluso si ha utilizado una plantilla de correo electrónico v1.0).

Si su suscripción tiene correos electrónicos de la versión 1.0 antes del paso a [!DNL Email Editor 2.0], experimentará el siguiente comportamiento según el estado actual del recurso:

**Aprobado**: al hacer clic en &quot;Editar borrador&quot;, se creará un borrador v2.0 del correo electrónico aprobado. Si aprueba el borrador de la versión 2.0, el estado aprobado del correo electrónico pasa a ser la versión 2.0 y no hay forma de volver a la versión 1.0.
**Borrador**: al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente como v2.0. En este punto, no será posible descartar y volver a la versión 1.0 porque no hay una versión aprobada del recurso.
**Aprobado con borrador**: al hacer clic en &quot;Editar borrador&quot;, ese borrador se marcará automáticamente como v2.0. Debido a esto, tampoco hay forma de revertir el borrador a v1.0.

Si su suscripción tiene plantillas de correo electrónico v1.0 antes de pasar a [!DNL Email Editor 2.0], experimentará el siguiente comportamiento:

**Aprobado**: al hacer clic en &quot;Editar borrador&quot;, se creará un borrador v2.0 de la plantilla de correo electrónico existente.
**Borrador**: al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente como v2.0. En este punto, no sería posible descartar y volver a la versión 1.0 porque no hay una versión aprobada del recurso.
**Aprobado con borrador**: al hacer clic en &quot;Editar borrador&quot;, se marcará automáticamente ese borrador como v2.0. Debido a esto, tampoco hay forma de revertir el borrador a v1.0.

Si aprueba una plantilla de correo electrónico anterior a la versión 1.0 (en cualquiera de los estados anteriores), verá el siguiente comportamiento:

Para los correos electrónicos de la versión 1.0 existentes que utilizaban la plantilla (anteriormente la versión 1.0):
**Correo electrónico v1.0 aprobado**: se creará un borrador v2.0 para este correo electrónico, aún con la plantilla v2.0 recién aprobada. También recibirá cualquier cambio en la plantilla.
**Correo electrónico de borrador v1.0**: el borrador permanecerá en la versión 1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá cualquier cambio en la plantilla.
**Aprobado con el borrador v1.0 por correo electrónico**: el borrador permanecerá en la versión 1.0 hasta que haga clic en &quot;Editar borrador&quot;. Después, se marcará automáticamente como v2.0 y recibirá cualquier cambio en la plantilla.

Para los correos electrónicos de la versión 2.0 existentes que utilizaban la plantilla (anteriormente la versión 1.0):
**Correo electrónico de la versión 2.0 aprobado**: se creará un borrador de la versión 2.0 para este correo electrónico, que seguirá &quot;utilizando&quot; la plantilla recién aprobada y recibirá cualquier cambio en la plantilla.
**Correo electrónico de borrador v2.0**: el borrador permanecerá tal cual (v2.0) y recibirá cualquier cambio de plantilla.
**Aprobado con el borrador v2.0 por correo electrónico**: el borrador permanecerá tal cual (v2.0) y recibirá cualquier cambio de plantilla.

>[!CAUTION]
>
>Si alguna vez aprueba el borrador v2.0 de una plantilla de correo electrónico v1.0, la plantilla pasará a ser v2.0. **no hay forma** de revertirlo a la versión 1.0.

Cosas que hay que tener en cuenta

* Los correos electrónicos aprobados **nunca** se han modificado.

* Las plantillas de correo electrónico aprobadas **nunca** han cambiado.

* En algunos **casos excepcionales**, no se puede abrir un mensaje de correo electrónico v1.0 en [!DNL Email Editor 2.0]. Si esto sucede, descarte el borrador y póngase en contacto con el Soporte técnico de Marketo.

>[!MORELIKETHIS]
>
>* [[!DNL Email Editor 2.0] Información general](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintaxis de plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
