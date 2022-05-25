---
description: 'Explicación del seguimiento de objetivos y los registros proyectados: Documentos de Marketo: Documentación del producto'
title: Información sobre el seguimiento de objetivos y los registros proyectados
hide: true
hidefromtoc: true
exl-id: 110768f4-46ed-4951-96b2-a97813d7b257
source-git-commit: e6b6fc5e3414936390a15dfb2034cfa4980169fb
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# Información sobre el seguimiento de objetivos y los registros proyectados {#understanding-goal-tracking-and-projected-registrations}

A continuación se muestra cómo realizar un seguimiento del progreso de sus objetivos y comprender las predicciones de Marketo.

>[!PREREQUISITES]
>
>Para acceder a la mayoría de estas funciones, asegúrese de habilitar la variable [alternancia de siguiente generación](/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md){target=&quot;_blank&quot;} para programas de eventos.

>[!NOTE]
>
>Cuando se crea un programa de eventos en la experiencia de Marketo Classic, la fecha de inicio del evento toma como valor predeterminado actualmente la fecha de creación del evento. Dado que los registros proyectados tienen en cuenta la cantidad de tiempo antes de la fecha de inicio de un evento, estos números pueden no ser precisos si la fecha de inicio y la fecha de creación son iguales (a menos que se establezcan intencionadamente).

## Seguimiento de objetivos y registros proyectados

1. Puede encontrar los detalles de seguimiento de objetivos en la **[!UICONTROL Informes]** del programa de eventos. En este ejemplo en particular, hasta ahora hay 150 miembros inscritos, frente a un objetivo de 200 (75%).

PICC

También verá su **[!UICONTROL Proyectado]** registros. Pase el ratón sobre el icono de información para ver un desglose de este número por segmento Probabilidad.

PICC

>[!NOTE]
>
>El gráfico Asistido y Superior permanecerá vacío hasta el día del evento.

1. Haga clic en la opción Chart para cambiar a un desglose de sus miembros según la probabilidad de registro. Verá los porcentajes de registro actuales para cada segmento, comparados con el porcentaje promedio para ese segmento en sus programas anteriores.

PICC

Todos los miembros (registrados y aún no registrados) se clasifican según su probabilidad de inscripción. Pase el ratón sobre el icono de información para ver cómo se definen estas categorías de probabilidad.

PICC

>[!NOTE]
>
>Los números de predicción se actualizan cada 24 horas hasta el día del evento. Cualquier miembro que aparezca como _Procesamiento_ se incluye en el siguiente ciclo de cálculo.

## Programas similares

Puede obtener información sobre su evento actual mirando cómo se desempeñaron programas similares en el pasado. Esta sección muestra hasta 5 programas similares de los últimos 6 meses, con el número/porcentaje de miembros que fueron _Registrados_ o superior.

Al calcular programas similares, incluimos los siguientes factores, entre otros:

* Tipo de programa
* Canal de programa
* Tamaño de la audiencia
* Etiquetas del programa
* Duración desde la creación del evento hasta el inicio del evento
* Duración del evento

PICC

## Recommendations

En la parte superior de la página Informes , puede encontrar recomendaciones dirigidas por AI/ML basadas en su progreso. Vuelva periódicamente para obtener consejos e información útiles.

PICC

## Predicciones de nivel personal

Haga clic en el **[!UICONTROL Miembros]** para ver todos los miembros del programa. Pase el ratón sobre la **[!UICONTROL Probabilidad de registro]** o **[!UICONTROL Probabilidad de asistencia]** para ver los porcentajes y las clasificaciones exactos. A continuación, puede tomar medidas sobre los miembros de una categoría en particular (por ejemplo, todos los miembros de la categoría &quot;Menos probable&quot; de registrarse) y dirigirlos específicamente para que puedan aumentar sus números de registro.

PICC

>[!NOTE]
>
>La probabilidad individual tiene en cuenta más de 40 factores de persona, incluidos los atributos de perfil, la actividad de la persona y las actividades invitadas/registradas/atendidas en el pasado.

## Preguntas frecuentes

**P: ¿Qué es el segmento?**

A: Es probable que se registre un valor entre 0 y 100. Toda persona que sea miembro del programa de eventos obtendrá un valor de probabilidad entre 0 y 100.

Hemos incluido los valores de probabilidad en tres segmentos:

* Probabilidad de registrarse >50% = Segmento muy probable
* Probabilidad de registrarse >25% a &lt;50% = Segmento probable
* Probabilidad de registrar &lt;25% = Segmento menos probable

Cuando una persona tiene probabilidad de registrarse, la predicción se incluirá en uno de estos segmentos (todas las personas que sean miembros de un programa caerán en uno de ellos). Por ejemplo, si un programa de eventos tiene 1000 miembros en función de las predicciones de probabilidad, esos 1000 se distribuirían en _Muy probable_, _Probable_ o _Menos probable_ segmentos.

Por lo tanto, las personas que entren en el segmento Muy probable tendrán más posibilidades de registrarse en el evento.

Conversión para registrarse = N.º de personas en el segmento registradas dividido por N.º de personas que entran en el segmento (por ejemplo, si 100 personas caen en el segmento Muy probable y 60 de ellas se registran, la tasa de conversión es del 60 %).

El porcentaje de conversión que se registrará seguirá este patrón: Muy probable > Probable > Menos probable.

**P: ¿Cómo utilizo las perspectivas?**

A: Las prácticas recomendadas implican lo siguiente:

i. Usted crea un programa y luego una campaña inteligente usa filtros predictivos con &quot;bueno que X&quot;, que resultarían en una cierta cantidad de personas (digamos, 1000) y usted ejecuta la campaña.

ii. Después de 24 horas, en la variable [!UICONTROL Informes] puede ver los registros proyectados que se calculan en función de la probabilidad de registrar valores de todas las personas que están actualmente invitadas.

iii. Si los registros proyectados son menores que el objetivo, tendría que invitar a más personas. En este punto, puede ver las perspectivas que indican cuál fue el umbral que funcionó en programas anteriores.

PICC

iv. Puede crear una nueva campaña inteligente con ese umbral para invitar a más personas.

v. En cualquier momento, si desea comprender por qué se muestra un número proyectado, puede alternar para ver la distribución de audiencias entre segmentos, sus tasas de conversión del pasado y aplicar esas tasas de conversión a la audiencia actual (consulte la captura de pantalla a continuación).

**P: ¿Qué es el gráfico Segmentos por registro?**

A: Tres barras, cada una de las cuales representa un segmento (muy probable, probable, menos probable).

**Línea punteada morada:** Tasa media de conversión al registro en ese segmento, según programas similares anteriores.

**Barra azul:** Porcentaje de registro de todas las personas de ese segmento.

PICC

Por ejemplo, digamos que 100 personas tienen probabilidades de registrarse > 50% y 60 de esas 100 personas registradas. Es muy probable que tenga una conversión del 60 %. Por lo tanto, todos los miembros agregados al programa tienen probabilidad de registrar valores, luego se incluyen en segmentos y se calcula el número de personas registradas en cada tasa de conversión de segmento.

**P: ¿Qué significa &quot;Registrado y superior&quot;?**

A: Cualquier persona que aparezca como registrada o cualquier otro estado con un número de paso igual o superior.

Puede crear nuevos estados de progresión para un programa de eventos, pero asignamos esos estados con estados estándar. Considere un caso en el que una persona es trasladada de invitada a recordada, lo que es un paso más alto que el registro. Esta persona también se considerará registrada y se mostrará en el seguimiento de objetivos.

PICC

**P: ¿Cómo se calculan los registros proyectados?**

A: Consulte a continuación.

PICC
