---
unique-page-id: 1900585
description: 'Agregar secciones editables a las plantillas de correo electrónico v1.0: Documentos de Marketo: Documentación del producto'
title: Agregar secciones editables a las plantillas de correo electrónico v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# Agregar secciones editables a las plantillas de correo electrónico v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si está creando una plantilla en el Editor de plantillas de correo electrónico v1.0, puede hacer que cualquier sección sea editable colocando un `<div>` a su alrededor.

>[!NOTE]
>
>**Ejemplo**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Reglas:

1. El HTML siempre debe ser válido.
1. La clase de **mktEditable** debe incluirse.
1. El ID debe ser único en ese HTML.
1. No hay espacios en el ID.

>[!CAUTION]
>
>Las instrucciones mktEditable no se pueden anidar.

Si desea obtener información sobre cómo hacerlo en el Editor de plantillas de correo electrónico v2.0, consulte [sintaxis de plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
