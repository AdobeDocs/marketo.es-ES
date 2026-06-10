---
description: Una guía paso a paso para crear una campaña de correo electrónico en CX Enterprise Coworker, desde escribir mensajes hasta revisar y exportar su campaña.
title: Creación y generación de campañas de correo electrónico
source-git-commit: b58edb707bf68aeed9f1b5eba8328c54a95c5a2f
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Creación y generación de campañas de correo electrónico {#build-and-generate-email-campaigns}

Obtenga información sobre cómo crear y revisar campañas de correo electrónico completas en minutos.

## Antes de comenzar

Asegúrese de que dispone de:

* Cuenta activa de colaborador de CX Enterprise ([regístrese aquí](https://coworker-essentials.experience.adobe.com/) si aún no lo ha hecho).

* Tu marca se configuró en **Tus cosas** > **Marcas**.

* (Opcional, pero recomendada) Se ha cargado una plantilla de correo electrónico de HTML en **Sus cosas** > **Plantillas de correo electrónico**.

* Un CSV de audiencia listo para cargar.

* Una idea clara del objetivo de la campaña (por ejemplo, &quot;recuperar clientes caducados&quot;, &quot;invitar a usuarios de prueba a un seminario web&quot;).

>[!TIP]
>
>Si no tiene experiencia en escribir mensajes para campañas de marketing, dedique dos minutos a _Preguntar al compañero de CX Enterprise: prácticas recomendadas_ antes de comenzar.

## Paso 1: Iniciar un nuevo chat

Desde la página de inicio, tiene tres formas de empezar:

* Escriba un mensaje en la barra de mensajes central.
* Elija una plantilla de campaña lista para usar de la sección templates debajo de la barra de mensajes.
* Utilice una opción &quot;ayuda para preguntar&quot; en el menú desplegable de la barra de mensajes para que CX Enterprise Coworker le guíe a través de la escritura del mensaje.

[CAPTURA DE PANTALLA: página principal con barra de mensajes, fila de plantilla y opción de &quot;ayuda para preguntar&quot; resaltada]

[FOR KEITH: breve descripción de cada opción y cuándo utilizarla. Recomiende plantillas para los principiantes, mensajes de forma libre para los especialistas en marketing que sepan lo que desean y &quot;ayúdeme a preguntar&quot; para cualquier persona que se encuentre entre medias.]

## Paso 2: Escriba el mensaje

Un mensaje de CX Enterprise Coworker sólido incluye:

* El objetivo de la campaña (lo que está intentando lograr).
* La audiencia (para quién es o de dónde provienen los datos de audiencia).
* Formato y estructura (número de correos electrónicos, cadencia, tono).
* Señales de marca o contexto (referencias a su marca, producto o campaña).

Por ejemplo:

```
"Create a win-back email series for customers who bought last year but haven't returned. Use the CSV I uploaded. Include 2–3 emails that feel seasonal and remind them to shop again."
```

[FOR KEITH: puede agregar de 2 a 3 ejemplos más que abarquen B2B y B2C para dar variedad. Extraiga los casos de uso de nuestro documento de recopilación para mantener la coherencia.]

[CAPTURA DE PANTALLA: Barra de mensaje con mensaje de ejemplo escrito en]

## Paso 3: Carga de la audiencia

[PARA KEITH: Introducción a la carga de CSV. Portada: - Donde está el botón de carga en la interfaz de usuario. : columnas requeridas y expectativas de formato. - Campos de personalización que CX Enterprise Coworker puede utilizar (nombre, fecha de último pedido, categoría de producto, etc.). - Vínculo a CSV de ejemplo. - ¿Qué sucede si los datos son confusos o faltan campos.]

[CAPTURA DE PANTALLA: flujo de carga de CSV]

>[!TIP]
>
>Excluya los contactos que no desee enviar por correo electrónico (usuarios sin suscribir, direcciones internas, cuentas de prueba) antes de cargarlos. Aunque habilitaremos progresivamente la funcionalidad para &quot;excluir&quot; usuarios específicos o &quot;añadir atributos&quot; durante el transcurso de la prueba, no está disponible inmediatamente desde la fecha de lanzamiento.

## Paso 4: Añadir un resumen y materiales de referencia

&lbrack;FOR KEITH: Explique cómo adjuntar un informe, documentos de referencia de marca u otro contexto. Portada: - Tipos de archivo compatibles. - Cómo utiliza CX Enterprise Coworker esta información (extraída en el contexto del prompt, aplicada a la generación de contenido, etc.). - Límites de tamaño de archivo, si los hay

He aquí un análisis profundo de mi sesión en Summit donde repaso esto: https://business.adobe.com/es/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limitaciones - Puedo conectarte con el engg - Neha Pullabhotla, que podrá ayudarnos en detalles específicos aquí. &rbrack;

[CAPTURA DE PANTALLA: resumen/referencia de la IU de datos adjuntos]

## Paso 5: Generación de la campaña

Haga clic en **Generar campaña**. CX Enterprise Coworker:

* Genere un plan de campaña estructurado.
* Pregunte por la audiencia de destino, que también se utilizará para la personalización de contenido.
* Borrador de contenido de correo electrónico personalizado para cada paso.
* Construye dinámicamente el recorrido a lo largo del camino.
* Montarlo todo en un solo tablero de campaña.

[PARA KEITH: descripción del aspecto del tablero de campaña y de su contenido. Abarca la vista de plan, la vista de recorrido y la vista de contenido. Tenga en cuenta cuánto tiempo puede tardar la generación, que depende del número de puntos de contacto en su recorrido. Llame a cabo que cuando abren un editor para el flujo de trabajo o para el correo electrónico, su conversación les mostrará esto para que estén en el contexto del componente específico, cómo el editor de correo electrónico es un editor de correo electrónico de apuntar y hacer clic con la limitación de que no está destinado a ser un diseñador de pleno derecho, los usuarios pueden editar imágenes en Adobe Express o incluso conectarse a Google Drive o AEM Assets mediante Adobe Express, Todos sus recursos de imagen se almacenan en Express, que vuelven a generar imágenes dentro de nuestro editor de correo electrónico con Firefly en línea, o sustituirlos por una imagen local de su equipo. Pueden desactivar la plantilla de HTML y volver a generar el contenido, y finalmente enviarse como &quot;Correo electrónico de prueba&quot; para validar lo que recibirá su cliente final]

[CAPTURA DE PANTALLA: tablero de campaña generado con plan, recorrido y contenido visible]

## Paso 6: revisar y perfeccionar

La interfaz conversacional hace que el refinamiento sea sencillo. Para hacer cambios, hable con CX Enterprise Coworker:

* &quot;Haga que la línea de asunto del correo electrónico 2 sea más urgente&quot;.
* &quot;Acorte la copia del cuerpo en todos los correos electrónicos&quot;.
* &quot;Cambie la audiencia solo a clientes de la región oeste&quot;.
* &quot;Añada un cuarto correo electrónico con una CTA más sólida&quot;.
* &quot;Cambie la espera de 3 días a 5 días&quot;.

[FOR KEITH: explica cómo hacer cambios mediante chat y edición directa. Explique cómo se actualizan los artefactos en su lugar. Mencione que no existe la posibilidad de añadir más nodos al flujo de trabajo a través del editor y que no existe actualmente el control de versiones. Para obtener los mejores resultados, también se recomienda solicitar cualquier cambio en el flujo de trabajo general al principio de la creación del plan]

[CAPTURA DE PANTALLA: refinamiento de la conversación en acción — mostrar un antes y un después de un correo electrónico después de una solicitud de chat]

## Paso 7: Enviar un correo electrónico de prueba

Antes de iniciar, envíese la campaña a usted mismo o a un miembro de su equipo para que la revise en una bandeja de entrada real.

[FOR KEITH: pasos para enviar una prueba. Cubierta: donde está el botón de prueba. - Quién puede recibir pruebas (actualmente solo el usuario que ha iniciado sesión): si se envían todos los correos electrónicos del recorrido o solo uno a la vez (actualmente solo uno a la vez, a menos que el usuario diga &quot;probar esta serie&quot; en el chat. - Qué comprobar en la prueba (renderización, vínculos, tokens de personalización, pie de página de cancelación de suscripción).]

[CAPTURA DE PANTALLA: enviar flujo de prueba]

## Paso 8: Inicio o exportación

Cuando esté satisfecho con la campaña, tiene algunas opciones:

>[!NOTE]
>Launch no está disponible actualmente en el momento de la publicación, pero se habilitará en un plazo de dos semanas desde la publicación inicial, pendiente de la aprobación legal.

* Inicie la campaña.
* Exportar correos electrónicos individuales como HTML.
* Exporte la campaña completa como un documento de Word o PDF para que el equipo lo revise.

[FOR KEITH: detalles sobre cada opción y cualquier comprobación previa al lanzamiento que ejecute CX Enterprise Coworker (cumplimiento, vínculos rotos, campos de personalización que faltan, etc.).]

[CAPTURA DE PANTALLA: Opciones de lanzamiento/exportación]

## Preguntas frecuentes

&lbrack;PARA KEITH: 4-6 preguntas frecuentes basadas en los comentarios tempranos de los usuarios. Primeros pasos sugeridos - para discutir con nuestro equipo de Ing:
* &quot;¿Por qué tarda tanto la primera respuesta?
* &quot;¿Qué sucede si la salida de CX Enterprise Coworker no es correcta?&quot;
* &quot;¿Puedo editar correos electrónicos directamente o solo a través de chat?&quot;
* &quot;¿Cómo puedo guardar una campaña sin iniciarla?&quot;
* &quot;¿Qué sucede si el CSV de mi audiencia contiene errores?&quot;
* &quot;¿Puedo duplicar o remezclar una campaña?&quot;
* &quot;¿Cómo comparto un borrador de campaña con un compañero de equipo para su revisión?&quot;&rbrack;
