---
description: 'Explicación del seguimiento de objetivos y los registros proyectados: Documentos de Marketo: Documentación del producto'
title: Información sobre el seguimiento de objetivos y los registros proyectados
hide: true
hidefromtoc: true
exl-id: 22d7ef98-2988-4188-99dd-5558a78492e3
source-git-commit: b609a268f08a7eef47d32c77a054a7d120339186
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Información sobre el seguimiento de objetivos y los registros proyectados {#understanding-goal-tracking-and-projected-registrations}

Después [definición de objetivos de evento](/help/marketo/product-docs/marketo-sky/setting-event-goals.md) y enviar invitaciones a través de un [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md), aquí se explica cómo rastrear el progreso de su objetivo y comprender las predicciones de Marketo.

>[!NOTE]
>
>Cuando se crea un programa de eventos en la experiencia de Marketo Classic, la fecha de inicio del evento toma como valor predeterminado actualmente la fecha de creación del evento. Dado que los registros proyectados tienen en cuenta la cantidad de tiempo antes de la fecha de inicio de un evento, estos números pueden no ser precisos si la fecha de inicio y la fecha de creación son iguales (a menos que se establezcan intencionadamente).

## Seguimiento de objetivos y registros proyectados {#goal-tracking-and-projected-registrations}

1. Puede encontrar los detalles de seguimiento de objetivos en la **[!UICONTROL Informes]** del programa de eventos. En este ejemplo en particular, hasta ahora hay 150 miembros inscritos, frente a un objetivo de 200 (75%).

   ![Imagen uno](assets/understanding-goal-tracking-and-projected-registrations-1.png)

También verá su **[!UICONTROL Proyectado]** registros. Pase el ratón sobre el icono de información para ver un desglose de este número por segmento Probabilidad.

![Imagen dos](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>El gráfico Asistido y Superior permanecerá vacío hasta el día del evento.

1. Haga clic en la opción Chart para cambiar a un desglose de sus miembros según la probabilidad de registro. Verá los porcentajes de registro actuales para cada segmento, comparados con el porcentaje promedio para ese segmento en sus programas anteriores.

   ![Imagen tres](assets/understanding-goal-tracking-and-projected-registrations-3.png)

Todos los miembros (registrados y aún no registrados) se clasifican según su probabilidad de inscripción. Pase el ratón sobre el icono de información para ver cómo se definen estas categorías de probabilidad.

![Imagen Cuatro](assets/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Los números de predicción se actualizan cada 24 horas hasta el día del evento. Cualquier miembro que aparezca como _Procesamiento_ se incluye en el siguiente ciclo de cálculo.

## Programas similares {#similar-programs}

Puede obtener información sobre su evento actual mirando cómo se desempeñaron programas similares en el pasado. Esta sección muestra hasta 5 programas similares de los últimos 6 meses, con el número/porcentaje de miembros que fueron _Registrados_ o superior.

Al calcular programas similares, incluimos los siguientes factores, entre otros:

* Tipo de programa
* Canal de programa
* Tamaño de audiencia
* Etiquetas del programa
* Duración desde la creación del evento hasta el inicio del evento
* Duración del evento

   ![Imagen cinco](assets/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations {#recommendations}

En la parte superior de la página Informes , puede encontrar recomendaciones dirigidas por AI/ML basadas en su progreso. Vuelva periódicamente para obtener consejos e información útiles.

![Imagen seis](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## Predicciones de nivel personal {#person-level-predictions}

Haga clic en el **[!UICONTROL Miembros]** para ver todos los miembros del programa. Pase el ratón sobre la **[!UICONTROL Probabilidad de registro]** o **[!UICONTROL Probabilidad de asistencia]** para ver los porcentajes y las clasificaciones exactos. A continuación, puede tomar medidas sobre los miembros de una categoría en particular (por ejemplo, todos los miembros de la categoría &quot;Menos probable&quot; de registrarse) y dirigirlos específicamente para que puedan aumentar sus números de registro.

![Image Seven](assets/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>La probabilidad individual tiene en cuenta más de 40 factores de persona, incluidos los atributos de perfil, la actividad de la persona y las actividades invitadas/registradas/atendidas en el pasado.

## Preguntas frecuentes {#faq}

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

![Imagen ocho](assets/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Puede crear una nueva campaña inteligente con ese umbral para invitar a más personas.

v. En cualquier momento, si desea comprender por qué se muestra un número proyectado, puede alternar para ver la distribución de audiencias entre segmentos, sus tasas de conversión del pasado y aplicar esas tasas de conversión a la audiencia actual (consulte la captura de pantalla a continuación).

**P: ¿Qué es el gráfico Segmentos por registro?**

A: Tres barras, cada una de las cuales representa un segmento (muy probable, probable, menos probable).

**Línea punteada morada:** Tasa media de conversión al registro en ese segmento, según programas similares anteriores.

**Barra azul:** Porcentaje de registro de todas las personas de ese segmento.

![Imagen nueve](assets/understanding-goal-tracking-and-projected-registrations-9.png)

Por ejemplo, digamos que 100 personas tienen probabilidades de registrarse > 50% y 60 de esas 100 personas registradas. Es muy probable que tenga una conversión del 60 %. Por lo tanto, todos los miembros agregados al programa tienen probabilidad de registrar valores, luego se incluyen en segmentos y se calcula el número de personas registradas en cada tasa de conversión de segmento.

**P: ¿Qué significa &quot;Registrado y superior&quot;?**

A: Cualquier persona que aparezca como registrada o cualquier otro estado con un número de paso igual o superior.

Puede crear nuevos estados de progresión para un programa de eventos, pero asignamos esos estados con estados estándar. Considere un caso en el que una persona es trasladada de invitada a recordada, lo que es un paso más alto que el registro. Esta persona también se considerará registrada y se mostrará en el seguimiento de objetivos.

![Imagen Diez](assets/understanding-goal-tracking-and-projected-registrations-10.png)

**P: ¿Cómo se calculan los registros proyectados?**

A: Consulte a continuación.

![Eleven de imagen](assets/understanding-goal-tracking-and-projected-registrations-11.png)
