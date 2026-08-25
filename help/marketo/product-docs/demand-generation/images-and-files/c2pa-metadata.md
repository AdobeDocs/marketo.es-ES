---
description: Descubra cómo los metadatos de C2PA se adjuntan automáticamente a imágenes generadas por IA en Marketo Engage, se conservan mediante ediciones y se utilizan para la procedencia del contenido.
title: Metadatos de C2PA en Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 77c4c0b6438f8a5070fd33412b7037b79f7fded1
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 2%

---

# Metadatos de C2PA en Marketo Engage

Están surgiendo nuevas leyes en torno a la transparencia generativa de la IA, y Adobe está trabajando para cumplir con los requisitos aplicables en todas las jurisdicciones. Los metadatos de C2PA son la herramienta de procedencia que utiliza Adobe para cumplir con los requisitos de estas leyes.

Los metadatos de C2PA son metadatos duraderos e invisibles que registran cómo se creó o editó un fragmento de contenido. Cuando se genera o edita una imagen con herramientas de IA generativa en Marketo Engage, los metadatos de C2PA se adjuntan automáticamente a esa imagen (no se requiere ninguna acción por su parte). Se trata de información cifrada y a prueba de manipulaciones que puede ayudar a los espectadores a comprender el linaje del contenido y garantizar la integridad de los activos de la marca. Esta información incluye:

* **Emisor o firmante**: información sobre la entidad o compañía que emitió la firma digital para certificar o firmar el recurso.
* **Fecha del problema**: Fecha en la que se aplicaron los metadatos de C2PA al recurso.
* **Crédito y uso**: Información sobre el productor del recurso, incluidos el nombre, los identificadores de medios sociales u otra información relacionada con la identidad.
* **Proceso**: Registra las ediciones o modificaciones realizadas en el recurso.
* **Detalles del dispositivo**: información sobre la aplicación o el dispositivo utilizado para crear o editar el recurso.
* **Herramienta de IA utilizada**: Si se utilizó IA generativa para crear el recurso, se puede incluir el nombre del modelo utilizado.
* **Otra información relevante**: también se incluyen datos adicionales para ayudar a ofrecer más contexto sobre el historial de un recurso.

## Acciones que adjuntan metadatos de C2PA

La siguiente tabla resume cuándo se adjuntan los metadatos de C2PA, en función de la acción de imagen realizada en la generación de imágenes en Marketo Engage.

| Acción | Descripción | ¿Metadatos de C2PA adjuntos? | Ejemplo de caso de uso |
|---|---|---|---|
| **Usar la herramienta &#39;Generar imagen&#39;** | Cree una nueva imagen a partir de un mensaje de texto, de una imagen de referencia o genere una imagen similar. | Siempre. La imagen se genera mediante IA generativa, por lo que siempre lleva metadatos frescos de C2PA. | Se genera una imagen de titular para una campaña de correo electrónico a partir de un mensaje de texto que describe el elemento visual deseado. |
| **Recortar una imagen** | Ajuste una imagen a las dimensiones solicitadas. | Solo si la imagen de origen ya tenía metadatos de C2PA. Al recortar se vuelven a crear los píxeles de la imagen, lo que normalmente borraría los metadatos de C2PA, por lo que Marketo Engage los lee de la imagen de origen antes de recortarlos y, a continuación, los vuelve a crear y a adjuntar al resultado recortado. El recorte en sí no agrega una nueva acción de IA generativa; conserva la existente. | Se recorta una imagen de titular generada para que se ajuste a una página web: los metadatos de C2PA se conservan a través del recorte. Se recorta una foto de archivo cargada que se utiliza como fondo de notificación push para ajustarse a la pantalla: como la foto de archivo no lleva ninguna acción de IA generativa, no se crean metadatos de C2PA. |
| **Agregar una superposición de texto** | Procesar texto generado sobre una imagen de fondo. | Solo si la imagen de fondo ya tenía metadatos de C2PA. Al procesar la superposición, se genera una nueva imagen del fondo más el texto, que normalmente borraría esos metadatos de C2PA, por lo que Marketo Engage los lee de antemano de la imagen de fondo y luego los reconstruye y vuelve a adjuntar al resultado. El paso de superposición no agrega una nueva acción de IA generativa. | Un titular promocional se procesa como una superposición de texto en una imagen de fondo generada para una página de aterrizaje: se conservan los metadatos de C2PA de la imagen de fondo. |

## Tipos de contenido y su ámbito

**Imágenes**: Cubiertas. Los metadatos de C2PA se adjuntan cuando las imágenes se generan con IA generativa y se conservan mediante operaciones de recorte y superposición de texto realizadas por la generación de imágenes en Marketo Engage.

**Texto**: No aplicable. Las salidas de solo texto de la generación de imágenes en Marketo Engage, como la generación de copias, la traducción y las sugerencias de alineación de marca, no requieren metadatos de C2PA.

## Qué sucede a medida que se mueve el contenido

Marketo Engage conserva los metadatos de C2PA asociados a los recursos de imagen admitidos. Si una imagen contiene metadatos de C2PA cuando se importa en Marketo Engage, los metadatos se conservan cuando el recurso se utiliza en el contenido de campaña generado y en las experiencias de correo electrónico saliente.

## Recursos adicionales

* [Directrices de usuario de IA generativa de Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* [Mecanismos de protección y limitaciones](https://experienceleague.adobe.com/es/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails)
