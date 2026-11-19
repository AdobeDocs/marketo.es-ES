---
description: Descripción
title: Seguimiento de aperturas de correo electrónico a nivel de persona
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 387abcce00de365f2b4abda9565b0eada2598cfd
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 3%
---
# Seguimiento de aperturas de correo electrónico a nivel de persona {#email-open-tracking-at-person-level}

Controle si Adobe Marketo Engage rastrea las aperturas y los clics de correos electrónicos de cada persona. Las anulaciones de seguimiento de correo electrónico de nivel de persona le permiten aplicar un valor predeterminado en el nivel de instancia y, a continuación, cambiar ese valor predeterminado para personas individuales. El rastreo de aperturas y el rastreo de clics se controlan de forma independiente.

Utilice esta función cuando sus requisitos de privacidad o políticas organizativas requieran consentimiento antes de rastrear la participación por correo electrónico.

>[!IMPORTANT]
> 
>Esta función proporciona controles que pueden ayudarle a cumplir con sus obligaciones de cumplimiento; no determina qué leyes se aplican ni qué personas necesitan dar su consentimiento. Trabaje con sus equipos legales y de privacidad para decidir cómo configurar el seguimiento y cómo recopilar y conservar el consentimiento.

## Funcionamiento de las decisiones de seguimiento

Tres configuraciones funcionan juntas:

| Configuración | Nivel | Qué hace |
|---|---|---|
| **Invalidaciones de seguimiento de correo electrónico de nivel de persona** | Instancia | Activa o desactiva la función. Cuando está desactivado, Marketo Engage ignora los campos de instancia predeterminada y de anulación de persona, y utiliza un comportamiento de seguimiento normal. |
| **Seguimiento de correo electrónico desactivado de forma predeterminada** | Instancia | Establece el valor predeterminado para el rastreo de clics y las aperturas. Cuando está desactivado, el seguimiento está activado de forma predeterminada. Cuando está habilitado, el seguimiento está desactivado de forma predeterminada. |
| **Anular el valor predeterminado del seguimiento de aperturas** y **Anular el valor predeterminado del seguimiento de clics** | Persona | Campos booleanos de persona. Un valor de `true` aplica lo contrario de la instancia predeterminada para ese tipo de seguimiento. Un valor de `false` o un valor vacío sigue al valor predeterminado de la instancia. |

Los campos de anulación no significan &quot;adhesión&quot; u &quot;exclusión&quot; por sí mismos. **`true`siempre significa &quot;lo contrario de la instancia predeterminada&quot;.**

### Tabla de decisión de seguimiento

Marketo Engage aplica esta decisión por separado a las aperturas de correo electrónico y a los clics en correos electrónicos.

| Función | Instancia predeterminada | La invalidación de persona es `false` o está vacía | La invalidación de persona es `true` |
|---|---|---|---|
| Activado | Seguimiento activado de forma predeterminada | Rastreado | Sin seguimiento |
| Activado | Seguimiento desactivado de forma predeterminada | Sin seguimiento | Rastreado |
| Desactivado | No aplicable | Seguimiento normal; se omiten la anulación y el valor predeterminado | Seguimiento normal; se omiten la anulación y el valor predeterminado |

### Ejemplo

Supongamos que la función está activada y que el valor predeterminado de la instancia es Tracking activado. Una persona tiene **Anular valor predeterminado de seguimiento de apertura** establecido en `true`, mientras que **Anular valor predeterminado de seguimiento de clics** está vacío. Marketo Engage no realiza el seguimiento de las aperturas del correo electrónico de esa persona, pero sigue realizando el seguimiento de sus clics en el correo electrónico.

## Elija un modelo de seguimiento.

Elija el modelo que coincida con los requisitos de consentimiento y privacidad antes de habilitar la función o rellenar los campos de persona.

| Modelo | Instancia predeterminada | Establezca la anulación en `true` cuando | Uso habitual |
|---|---|---|---|
| Exclusión | Seguimiento activado de forma predeterminada | Una persona se opone al seguimiento | Rastrear a la mayoría de las personas, pero detener el seguimiento de las personas que se oponen. |
| Inclusión (consentimiento) | Seguimiento desactivado de forma predeterminada | Una persona da su consentimiento para el seguimiento | Requerir consentimiento antes del seguimiento, incluso para los destinatarios cubiertos por la CNIL o la guía de Garante aplicables. |

>[!CAUTION]
> 
>Elija el modelo antes de rellenar los campos de anulación y evite cambiar la instancia predeterminada posteriormente. Dado que `true` significa &quot;lo contrario del valor predeterminado&quot;, al cambiar el valor predeterminado se invierte el efecto de todos los valores de invalidación existentes. Por ejemplo, si se pasa de activar el seguimiento de forma predeterminada a desactivarlo, se puede hacer que se realice el seguimiento de las personas que anteriormente se opusieron al seguimiento. Si debe cambiar el valor predeterminado, actualice los valores de anulación de todas las personas afectadas antes de que el cambio surta efecto.

## Activar la función

Las anulaciones de seguimiento de correo electrónico de nivel de persona están desactivadas de forma predeterminada. Para habilitarlo, póngase en contacto con Asistencia al cliente de Adobe y especifique:

1. Que desea habilitar **Anulaciones de seguimiento de correo electrónico de nivel de persona**.
2. Si el valor predeterminado de la instancia debe ser **tracking activado de forma predeterminada** o **tracking desactivado de forma predeterminada**.

>[!TIP]
> 
>Rellene los campos de anulación para las personas existentes antes de solicitar a Adobe que habilite la función. Esto ayuda a garantizar que el comportamiento de seguimiento deseado se aplique desde el primer correo electrónico preparado después de la activación.

## Establecer valores de anulación para personas

Los campos de anulación son campos de persona booleanos. Configúrelos con el método que mejor se adapte a su flujo de trabajo:

| Método | Notas |
|---|---|
| Paso de flujo Cambiar valor de datos | Utilice una campaña inteligente para establecer un campo cuando una persona cumpla sus criterios, como enviar una casilla de verificación de consentimiento en un formulario. |
| Formularios | Asigne una casilla de verificación o un campo oculto de un formulario Marketo Engage al campo de la persona. |
| Importación de lista | Incluya el campo como una columna en el archivo de importación. |
| API de REST | Use los nombres de campo de API `overrideOpenTrackingDefault` y `overrideClickTrackingDefault`. |

Establezca cada campo según el consentimiento de la persona. Si el idioma de consentimiento trata las aperturas y los clics por separado, configure cada campo de forma independiente.

## Cambios en el correo electrónico

Cuando Marketo Engage decide no rastrear a una persona, cambia el contenido del correo electrónico que envía a esa persona.

| Seguimiento desactivado para | Qué cambios | Lo que aún funciona |
|---|---|---|
| Aperturas | El correo electrónico no incluye el píxel de seguimiento abierto. No se ha registrado ninguna actividad **Abrir correo electrónico**. | Otra funcionalidad de correo electrónico, incluido el rastreo de clics si permanece habilitado. |
| Clics | Los vínculos van directamente a sus destinos en lugar de a través del dominio de seguimiento de Marketo Engage. No se agrega el vínculo de seguimiento oculto. No se ha registrado ninguna actividad de **Click Email**. | Los vínculos de cancelación de suscripción, el vínculo de no participación de pie de página de correo electrónico, `list-unsubscribe` y **Ver como página web** siguen funcionando. El uso de estos vínculos no registra una actividad **Click Email**. |

## Qué correos electrónicos se ven afectados

| Tipo de correo electrónico | ¿Invalidaciones aplicadas? |
|---|---|
| Correos electrónicos por lotes, como correos electrónicos enviados desde una campaña inteligente por lotes o un programa de correo electrónico | Sí |
| correos electrónicos de déclencheur, como correos electrónicos enviados desde una campaña inteligente de déclencheur | Sí |
| Correos electrónicos con pruebas A/B o variantes de campeón/aspirante | Sí. El seguimiento se decide por separado para cada persona, independientemente de la variante que reciba. |
| Ver como página web | Sí. La versión web sigue la configuración actual de la persona. Un cambio puede tardar hasta una hora en aparecer. |
| Correos electrónicos operativos | No. Siguen un comportamiento de seguimiento normal. |
| Correos electrónicos de muestra (prueba) | No. Siguen un comportamiento de seguimiento normal. |
| Previsualizaciones de correo electrónico | Sin cambios. No se realiza un seguimiento de las vistas previas. |
| Correos electrónicos de alerta | Sin cambios. No se realiza un seguimiento de las alertas. |
| Mensajes SMS | No. Esta función solo se aplica al correo electrónico. |

## Cuando Marketo Engage toma la decisión de seguimiento

Marketo Engage lee los valores de anulación de una persona cuando prepara el correo electrónico para su envío.

- **Entrega programada o retrasada:** Si un correo electrónico se prepara ahora y se entrega más tarde (por ejemplo, con Head Start o Zona horaria del destinatario), se aplican los valores en el momento de la preparación. Un cambio realizado después de la preparación no cambia ese correo electrónico.
- **Correos electrónicos ya entregados:** Al cambiar la invalidación de una persona, no se cambian los mensajes de correo electrónico que ya ha recibido. Los clics en vínculos en correos electrónicos enviados anteriormente se pueden seguir rastreando si esos vínculos se prepararon con el seguimiento habilitado.
- **Correos electrónicos futuros:** Se aplica un cambio a los mensajes de correo electrónico que Marketo Engage prepara después del cambio.

Si una persona retira el consentimiento, actualice su valor de anulación lo antes posible para que el cambio se aplique al siguiente correo electrónico preparado para ella.

## Impacto en la creación de informes, listas inteligentes y puntuación

Cuando Marketo Engage no rastrea a una persona, no registra las actividades de **Abrir correo electrónico** o **Hacer clic en Enviar correo electrónico** para ellos. Como resultado:

- **Campañas inteligentes:** Los filtros y déclencheur como **Correo electrónico abierto** y **Vínculo en el que se hizo clic en el correo electrónico** no coinciden con esa persona o se activan cuando no se realiza un seguimiento de la actividad correspondiente.
- **Informes y paneles:** Las tasas de apertura de correo electrónico, las tasas de clics y el rendimiento de los vínculos solo reflejan las personas rastreadas. Las métricas de participación pueden disminuir a medida que no se realiza el seguimiento de más personas.
- **Puntuación y éxito del programa:** Las reglas y los pasos de éxito del programa basados en aperturas o clics no se aplican a las personas cuyas actividades no se rastrean. Revise estas reglas para que las personas no reciban puntuaciones ni avances injustos.
- **Asociación de actividad web:** Cuando el rastreo de clics está desactivado, los vínculos de correo electrónico no llevan el token de seguimiento de Marketo Engage. Si la persona aún no es conocida por Munchkin, una visita al sitio web desde ese correo electrónico no se asocia con la persona a través del vínculo.

**Las actividades enviadas, enviadas, devueltas y canceladas no se ven afectadas.**

## Cómo funciona esto con otras configuraciones de seguimiento

Las anulaciones de seguimiento de correo electrónico en el nivel de persona pueden desactivar el seguimiento de una persona. No activa el seguimiento cuando otra configuración ya lo ha deshabilitado. Por ejemplo, los vínculos marcados con la clase `mktNoTrack` permanecen sin seguimiento aunque la configuración de la persona permita el rastreo de clics.

## Desactivar la función

Si Adobe deshabilita la función para su instancia, los correos electrónicos preparados después del cambio vuelven al comportamiento de seguimiento normal. Los valores de anulación permanecen en los registros de las personas, pero se ignoran. Si la función vuelve a activarse más adelante, los valores almacenados se aplican de nuevo.

## Preguntas frecuentes

### ¿Puedo rastrear aperturas pero no clics de una persona o al revés?

Sí. La apertura y el rastreo de clics se deciden de forma independiente. Establezca únicamente el campo de anulación para el tipo de seguimiento que desea cambiar.

### ¿Esta función evita que envíe correos electrónicos a una persona?

No. Solo controla el seguimiento. Para dejar de enviar correos electrónicos de marketing a una persona, utilice las funciones de cancelación de suscripción y consentimiento existentes.

### ¿Siguen viendo los vínculos de cancelación de suscripción los usuarios sin seguimiento?

Sí. Los vínculos de cancelación de suscripción y **Ver como página web** siguen funcionando para todas las personas.

### ¿Por qué una persona que se excluyó sigue teniendo una actividad de correo electrónico de clic?

Es posible que hayan hecho clic en un vínculo de un correo electrónico preparado antes de que cambiara su valor de anulación. Los cambios se aplican a los correos electrónicos preparados después del cambio.

### ¿Debo cambiar mis plantillas de correo electrónico?

No. Marketo Engage aplica la decisión de seguimiento cuando crea cada correo electrónico. No es necesario que cambie las plantillas o los correos electrónicos.

## Artículos relacionados

- Explicación de los correos electrónicos operativos
- Paso de flujo para cambiar valor de datos
- Deshabilitar el seguimiento de un vínculo en un correo electrónico
- Head Start
- Zona horaria del destinatario
- Informe de rendimiento de correo electrónico
