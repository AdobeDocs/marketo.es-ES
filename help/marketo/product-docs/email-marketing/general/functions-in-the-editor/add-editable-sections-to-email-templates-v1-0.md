---
unique-page-id: 1900585
description: Aprenda a añadir secciones editables a las plantillas de correo electrónico en la versión 1.0. Permite que los usuarios editen áreas específicas mientras mantienen el resto bloqueado.
title: Añadir secciones editables a plantillas de correo electrónico v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 14%

---

# Añadir secciones editables a plantillas de correo electrónico v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si está creando una plantilla en el Editor de plantillas de correo electrónico v1.0, puede hacer que cualquier sección se pueda editar colocando un `<div>` especial alrededor de ella.

>[!NOTE]
>
>**Ejemplo**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Reglas:

1. La HTML siempre debe ser válida.
1. Se debe incluir la clase de **mktEditable**.
1. El ID debe ser único en ese HTML.
1. No hay espacios en el ID.

>[!CAUTION]
>
>Las instrucciones mktEditable no se pueden anidar.

Si desea obtener información sobre cómo hacerlo en el Editor de plantillas de correo electrónico v2.0, consulte [sintaxis de la plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
