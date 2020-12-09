---
title: comprensión-objetivo-seguimiento-y-registros-proyectados
description: Explicación del seguimiento de objetivos y los registros proyectados
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---


# Explicación del seguimiento de objetivos y los registros proyectados

<br> 

Después de [establecer objetivos](/help/sky/setting-event-goals.md)de evento y enviar invitaciones a través de una campaña [](/help/sky/create-a-smart-campaign.md)inteligente, aquí se muestra cómo rastrear el progreso de su objetivo y comprender las predicciones de Marketing.

>[!NOTE]
>
>Cuando se crea un programa de evento en la experiencia de marketing clásico, la fecha de inicio de evento toma como valor predeterminado la fecha de creación del evento. Dado que los registros proyectados tienen en cuenta la cantidad de tiempo antes de la fecha de inicio de un evento, es posible que estos números no sean precisos si la fecha de inicio y la fecha de creación son iguales (a menos que se establezcan intencionalmente).

## Seguimiento de objetivos y registros proyectados

1. Puede encontrar los detalles del seguimiento de objetivos en la ficha **[!UICONTROL Informes]** del programa de evento. En este ejemplo particular, hasta ahora hay 150 miembros registrados contra un objetivo de 200 (75%).

   ![Imagen uno](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

También verá los registros **[!UICONTROL proyectados]** . Pase el ratón sobre el icono de información para ver un desglose de este número por segmento de probabilidad.

![Imagen dos](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>El gráfico de asistentes y superiores permanecerá vacío hasta el día del evento.

1. Haga clic en la opción Gráfico para cambiar a un desglose de los miembros según la probabilidad de registro. Verá los porcentajes de registro actuales para cada segmento, en comparación con el porcentaje promedio para ese segmento en los programas anteriores.

   ![Imagen tres](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Todos los miembros (registrados y aún no registrados) se clasifican según la probabilidad de registro. Pase el ratón sobre el icono de información para ver cómo se definen estas categorías de probabilidad.

![Imagen Cuatro](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Los números de predicción se actualizan cada 24 horas hasta el día del evento. Los miembros que se incluyan como _Procesamiento_ se incluirán en el siguiente ciclo de cálculo.

## Programas similares

Puede obtener información sobre su evento actual observando el rendimiento de programas similares en el pasado. Esta sección muestra hasta 5 programas similares de los últimos 6 meses, con el número/porcentaje de miembros _registrados_ o superiores.

Al calcular programas similares, se incluyen los siguientes factores, entre otros:

* Tipo de programa
* Canal programa
* Tamaño de audiencia
* Etiquetas de programa
* Duración desde la creación de eventos hasta el inicio de eventos
* Duración del evento

   ![Imagen cinco](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

En la parte superior de la página Informes, puede encontrar recomendaciones dirigidas por AI/ML en función de su progreso. Vuelva periódicamente para obtener consejos y perspectivas útiles.

![Imagen seis](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## predicciones de nivel de persona

Haga clic en la ficha **[!UICONTROL Miembros]** para vista de todos los miembros del programa. Pase el ratón sobre las barras de probabilidad **[!UICONTROL de]** registro o probabilidad de **[!UICONTROL asistencia]** para ver los porcentajes y las categorías exactos. A continuación, puede realizar acciones en los miembros de una categoría en particular (por ejemplo, todos los miembros de la categoría &quot;Menos probable&quot; para registrar) y, específicamente, destinatarios para aumentar potencialmente sus números de registro.

![Imagen siete](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>La probabilidad individual tiene en cuenta más de 40 factores de persona, incluidos los atributos de perfil, la actividad de las personas y las actividades invitadas, registradas o atendidas en el pasado.

## Preguntas más frecuentes

**P: ¿Cuál es el segmento?**

A: Es probable que se registre un valor entre 0 y 100. Cada persona que sea miembro del programa de evento obtendrá un valor de probabilidad entre 0 y 100.

Ponemos los valores de probabilidad en tres segmentos:

* Probabilidad de registrar >50% = segmento muy probable
* Probabilidad de registrar >25% a &lt;50% = Segmento probable
* Probabilidad de registrar &lt;25% = segmento menos probable

Cuando una persona tiene la probabilidad de registrarse, la predicción caerá en uno de estos segmentos (toda persona que sea miembro de un programa caerá en uno de ellos). Por ejemplo, si un programa de evento tiene 1000 miembros en función de las predicciones de probabilidad, esos 1000 se distribuirían en segmentos _con alta probabilidad_, _probabilidad_ o _menos probabilidad_ .

Por lo tanto, las personas que se incluyen en el segmento Muy probable tendrán una mayor posibilidad de registrarse para el evento.

Conversión para registrarse = cantidad de personas en el segmento registradas divididas por cantidad de personas que caen en el segmento (por ejemplo: si 100 personas caen en el segmento con más probabilidades y 60 de ellas se registran, la tasa de conversión es del 60%).

El porcentaje de conversión que se registrará seguirá este patrón: Muy probable > Probable > Menos probable.

**P: ¿Cómo se utilizan las perspectivas?**

A: La práctica recomendada implica lo siguiente:

i. Se crea un programa y, a continuación, una Campaña inteligente utiliza filtros predictivos con &quot;buenos que X&quot;, que resultarían en una cierta cantidad de personas (digamos, 1000) y se ejecuta la campaña.

ii. Después de 24 horas, en la ficha [!UICONTROL Informes] puede ver los registros proyectados que se calculan en función de la probabilidad de registrar los valores de todas las personas invitadas actualmente.

iii. Si los registros proyectados son inferiores al objetivo, deberá invitar a más personas. En este punto, puede ver las perspectivas que indican cuál fue el umbral que funcionó en programas pasados.

![Imagen ocho](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Puede crear una nueva Campaña inteligente con ese umbral para invitar a más personas.

v. En cualquier momento, si desea comprender por qué se muestra un número proyectado, puede alternar para ver la distribución de audiencias entre segmentos, sus tasas de conversión del pasado y aplicar esas tasas de conversión a la audiencia actual (consulte la captura de pantalla a continuación).

**P: ¿Qué es el gráfico Segmentos por registro?**

A: Tres barras, cada una que representa un segmento (Muy probable, Probable, Menos probable).

**Línea de puntos púrpura:** Tasa media de conversión al registro en ese segmento, según programas similares anteriores.

**Barra azul:** Porcentaje de registro de todas las personas de ese segmento.

![Imagen nueve](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Por ejemplo: supongamos que 100 personas tienen probabilidades de registrarse > 50% y 60 de esas 100 personas registradas. Es muy probable que tenga una conversión del 60 %. Por lo tanto, todos los miembros agregados al programa tienen probabilidad de registrar valores, luego se colocan en segmentos y se calcula el número de personas registradas en cada tasa de conversión de segmento.

**P: ¿Qué significa &quot;Registrado y Superior&quot;?**

A: Cualquier persona que figure como registrada o cualquier otro estado con un número de paso igual o superior.

Puede crear nuevos estados de progresión para un programa de evento, pero asignamos esos estados con estados estándar. Considere un caso en el que una persona es trasladada de invitada a recordada, lo cual es un paso más alto que el registro. Esta persona también se considerará registrada y se mostrará en el seguimiento de objetivos.

![Imagen Diez](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**P: ¿Cómo se calculan los registros proyectados?**

A: Véase más abajo.

![Imagen once](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
