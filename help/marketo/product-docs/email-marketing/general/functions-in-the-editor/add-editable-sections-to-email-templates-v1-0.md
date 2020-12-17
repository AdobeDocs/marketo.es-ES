---
unique-page-id: 1900585
description: Añadir secciones editables a plantillas de correo electrónico v1.0 - Documentos de marketing - Documentación del producto
title: Añadir secciones editables a plantillas de correo electrónico v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Añadir secciones editables a plantillas de correo electrónico v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si va a crear una plantilla en el Editor de plantillas de correo electrónico v1.0, puede hacer que cualquier sección se pueda editar colocando una `<div>` especial alrededor de ella.

>[!NOTE]
>
>**Ejemplo**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Reglas:

1. El HTML siempre debe ser válido.
1. Se debe incluir la clase **mktEditable**.
1. El ID debe ser único en ese HTML.
1. No hay espacios en el ID.

>[!CAUTION]
>
>Las instrucciones mktEditable no se pueden anidar.

Si desea obtener información sobre cómo hacerlo en el Editor de plantillas de correo electrónico v2.0, consulte [sintaxis de plantillas de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
