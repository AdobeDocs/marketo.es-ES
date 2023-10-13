---
description: 'Explicación del seguimiento de objetivos y los registros proyectados: documentos de Marketo, documentación del producto'
title: Explicación del seguimiento de objetivos y los registros proyectados
exl-id: 110768f4-46ed-4951-96b2-a97813d7b257
feature: Predictive Audiences
source-git-commit: 86f9e9f13b24a82deb50ec4c398035d7d7479d20
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Explicación del seguimiento de objetivos y los registros proyectados {#understanding-goal-tracking-and-projected-registrations}

A continuación, le indicamos cómo realizar un seguimiento del progreso de sus objetivos y comprender las predicciones de Marketo.

>[!PREREQUISITES]
>
>Para acceder a la mayoría de estas funciones, asegúrese de habilitar la variable [alternancia de próxima generación](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"} para programas de eventos.

>[!NOTE]
>
>Cuando se crea un programa de eventos en la experiencia de Marketo Classic, la fecha de inicio del evento se establece de forma predeterminada en la fecha de creación del evento. Dado que los registros proyectados tienen en cuenta la cantidad de tiempo antes de la fecha de inicio de un evento, estos números pueden no ser exactos si la fecha de inicio y la fecha de creación son la misma (a menos que se establezcan intencionadamente).

## Seguimiento de objetivos y registros proyectados

1. Puede encontrar los detalles de seguimiento de objetivos en la **[!UICONTROL Informes]** de su programa de eventos. En este ejemplo en particular, hay 150 miembros registrados hasta ahora contra una meta de 200 (75%).

   ![](assets/understanding-goal-tracking-and-projected-registrations-1.png)

También verá su.. **[!UICONTROL Proyectado]** registros. Pase el ratón sobre el icono de información para ver un desglose de este número por segmento de probabilidad.

![](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>El gráfico Asistencia y Superior permanecerá vacío hasta el día del evento.

Si no ha habilitado el conmutador, así es como aparecerá en la interfaz de usuario de Marketo Class:

![](assets/understanding-goal-tracking-and-projected-registrations-3.png)

1. Haga clic en el botón de alternancia Gráfico para cambiar a un desglose de los miembros por probabilidad de registro. Verá los porcentajes de registro actuales de cada segmento, comparados con el porcentaje promedio de ese segmento en sus programas anteriores.

   ![](assets/understanding-goal-tracking-and-projected-registrations-4.png)

Todos los miembros (registrados y aún no registrados) se clasifican según su probabilidad de registro. Pase el ratón sobre el icono de información para ver cómo se definen estas categorías de probabilidad.

![](assets/understanding-goal-tracking-and-projected-registrations-5.png)

>[!NOTE]
>
>Los números de predicción se actualizan cada 24 horas hasta el día del evento. Cualquier miembro que aparezca como _Procesando_ se incluirá en el siguiente ciclo de cálculo.

## Programas similares

Puede obtener información sobre el evento actual si observa el rendimiento de programas similares en el pasado. Esta sección muestra hasta 5 programas similares de los últimos 6 meses, con el número/porcentaje de miembros que fueron _Registrados_ o superior.

En el cálculo de programas similares se incluyen, entre otros, los siguientes factores:

* Tipo de programa
* Canal de programa
* Tamaño de audiencia
* Etiquetas del programa
* Duración de tiempo desde la creación del evento hasta su inicio
* Duración del evento

  ![](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## Recommendations

En la parte superior del [!UICONTROL Informes] , puede encontrar recomendaciones impulsadas por IA/ML basadas en su progreso. Vuelva periódicamente para obtener consejos y perspectivas útiles.

![](assets/understanding-goal-tracking-and-projected-registrations-7.png)

## Predicciones a nivel de persona

Haga clic en **[!UICONTROL Miembros]** para ver todos los miembros del programa. Pase el ratón sobre **[!UICONTROL Probabilidad de registro]** o **[!UICONTROL Probabilidad de asistencia]** para ver los porcentajes y las categorizaciones exactos. Luego puede tomar medidas con los miembros de una categoría en particular (por ejemplo, todos en la categoría &quot;Menos probable&quot; de registrarse), y específicamente dirigirlos para aumentar potencialmente sus números de registro.

![](assets/understanding-goal-tracking-and-projected-registrations-8.png)

>[!NOTE]
>
>La probabilidad individual tiene en cuenta más de 40 factores de persona, incluidos los atributos de perfil, la actividad de la persona y las actividades pasadas invitadas/registradas/asistidas.

## Preguntas frecuentes

**P: ¿Qué es el segmento?**

R: Es probable que el registro tenga un valor entre 0 y 100. Todas las personas que sean miembros del programa de eventos obtendrán un valor de probabilidad entre 0 y 100.

Colocamos los valores de probabilidad en tres segmentos:

* Probabilidad de registro > 50 % = Segmento con alta probabilidad
* Probabilidad de registro de >25% a &lt;50% = Segmento probable
* Probabilidad de registro &lt;25% = Segmento con menos probabilidades

Cuando una persona tiene probabilidades de registrarse, la predicción caerá en uno de estos segmentos (cada persona que sea miembro de un programa caerá en uno de ellos). Por ejemplo, si un programa de eventos tiene 1000 miembros según las predicciones de probabilidad, esos 1000 se distribuirían en _Muy probable_, _Probable_, o _Menos probable_ segmentos.

Por lo tanto, las personas que entran en el segmento Altamente probable tendrán una mayor probabilidad de registrarse en el evento.

Conversión a registro = número de personas en el segmento registrado dividido por el número de personas que pertenecen al segmento (por ejemplo, si 100 personas pertenecen al segmento Altamente probable y 60 de ellas se registran, la tasa de conversión es del 60 %).

El % de conversión para registrarse seguirá este patrón: Muy probable > Probable > Menos probable.

**P: ¿Cómo utilizo las perspectivas?**

R: La práctica recomendada implica lo siguiente:

i. Crea un programa y luego una campaña inteligente utiliza filtros predictivos con &quot;mayor que X&quot;, lo que resultaría en una cierta cantidad de personas (digamos 1000) y ejecuta la campaña.

ii. Después de 24 horas, en el [!UICONTROL Informes] pestaña puede ver los registros proyectados que se calculan en función de la probabilidad de registrar valores de todas las personas invitadas actualmente.

iii. Si las inscripciones proyectadas son menores que el objetivo, tendría que invitar a más personas. En este punto, puede ver las perspectivas que le indican cuál era el umbral que funcionaba en programas anteriores.

![](assets/understanding-goal-tracking-and-projected-registrations-9.png)

iv. Puede crear una nueva campaña inteligente con ese umbral para invitar a más personas.

v. En cualquier momento, si desea comprender por qué se muestra un número proyectado, puede alternar para ver la distribución de audiencias entre segmentos, sus tasas de conversión del pasado y aplicar esas tasas de conversión a la audiencia actual (véase la captura de pantalla siguiente).

**P: ¿Qué es el gráfico Segmentos por registro?**

R: Tres barras, cada una de las cuales representa un segmento (Muy probable, Probable, Menos probable).

**Línea de puntos púrpura:** Tasa promedio de conversaciones hasta el registro en ese segmento, según programas similares anteriores.

**Barra azul:** Porcentaje de registro de todas las personas de ese segmento.

![](assets/understanding-goal-tracking-and-projected-registrations-10.png)

Por ejemplo, supongamos que 100 personas tienen probabilidad de registrarse > 50 % y 60 de esas 100 personas registradas. Es muy probable que tenga una conversión del 60 %. Por lo tanto, todos los miembros añadidos al programa tienen probabilidad de registrar valores, luego se colocan en segmentos y según el número de personas registradas en cada tasa de conversión del segmento se calcula.

**P: ¿Qué significa &quot;Registrado y Superior&quot;?**

R: Cualquier persona que aparezca como registrada o cualquier otro estado con un número de paso igual o superior.

Puede crear nuevos estados de progresión para un programa de evento, pero asignamos esos estados con estados estándar. Considere un caso en el que una persona pasa de invitada a recordada, lo que supone un paso más alto que el registro. Esta persona también se considerará registrada y se mostrará en el seguimiento de objetivos.

![](assets/understanding-goal-tracking-and-projected-registrations-11.png)

**P: ¿Cómo se calculan los registros proyectados?**

R: Consulte lo siguiente.

![](assets/understanding-goal-tracking-and-projected-registrations-12.png)
