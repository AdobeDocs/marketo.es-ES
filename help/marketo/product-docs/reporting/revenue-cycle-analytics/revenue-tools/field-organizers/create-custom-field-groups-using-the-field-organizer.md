---
unique-page-id: 10094404
description: Creación de grupos de campos personalizados con el organizador de campos - Documentos de Marketo - Documentación del producto
title: Creación de grupos de campos personalizados con el organizador de campos
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 3%

---

# Creación de grupos de campos personalizados con el organizador de campos {#create-custom-field-groups-using-the-field-organizer}

Antes de poder habilitar los grupos de campos personalizados para la creación de informes en el área Análisis de rendimiento del modelo (posibles clientes) del Explorador de ciclos de ingresos, debe categorizar los campos estándar o personalizados en grupos para la creación de informes mediante el Organizador de campos en Marketo Lead Management. Esto solo se aplica a los atributos del cliente potencial y de la compañía.
Al seleccionar un campo estándar o personalizado en la lista desplegable Campo del cuadro de diálogo Nuevo organizador de campos, el sistema asigna el tipo de datos de Marketo Lead Management asociado al campo que desea agrupar con uno de los tres editores disponibles en el organizador de campos: cadena, entero o fecha.

| Tipo de datos de Marketo Lead Management | Tipo de datos del editor del organizador de campos |
|---|---|
| Cadena | Cadena |
| Correo electrónico | Cadena |
| Entero | Entero |
| Texto | Cadena |
| URL | Cadena |
| Referencia | No compatible |
| Moneda | Entero |
| Fecha/Hora | Fecha |
| Booleano | No compatible |
| Teléfono | Cadena |
| Fecha | Fecha |
| Flotante | Entero |
| Calculado | No compatible |

Las tres secciones siguientes describen cómo crear un grupo de campos personalizados para una cadena, un número entero o un tipo de fecha.

## Crear grupo de campos personalizados: editor de cadenas {#create-custom-field-group-string-editor}

1. Haga clic en **[!UICONTROL Base de datos de posibles clientes]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo organizador de campos]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Campo]** y seleccione un campo estándar o personalizado con un tipo de datos que se asigne al editor de cadenas (consulte la tabla de la sección anterior). [!UICONTROL País] se usa aquí.

   ![](assets/three.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/four.png)

   El nuevo grupo personalizado se muestra en el árbol de la base de datos de posibles clientes representado como Nombre de campo > Grupo de nombre de campo (ejemplo: País > Grupo de país).

   ![](assets/4.5.png)

1. Haga clic en el icono de lápiz para personalizar el nombre. Por ejemplo, puede cambiar el nombre de &quot;Grupo de países&quot; por &quot;Continente&quot;. Escriba el nuevo nombre deseado y haga clic fuera del cuadro para guardarlo automáticamente.

   ![](assets/five.png)

1. De manera predeterminada, todos los valores de datos se colocan en el subgrupo &quot;[!UICONTROL Otros]&quot;. Para categorizar los valores de los datos, haga clic en **[!UICONTROL Agregar grupo]** para crear un subgrupo y asígnele un nombre.

   >[!NOTE]
   >
   >Puede añadir hasta diez subgrupos para categorizar los valores de datos. A cada subgrupo creado se le asigna un número de ID.

   En este ejemplo, se han creado grupos para la mayoría de los continentes.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Para eliminar un subgrupo, simplemente haga clic en la X roja junto al nombre del subgrupo. Si hay valores de datos en el grupo, estos se moverán al grupo predeterminado de [!UICONTROL Otros].

1. Resalte uno o varios valores de datos en el lienzo y arrastre y suelte los valores de datos en el subgrupo adecuado.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Para quitar un valor de datos de un subgrupo, reasigne el valor de datos al grupo predeterminado de Otros.

1. Utilice la opción de filtro en la esquina superior izquierda directamente encima del lienzo para seleccionar y ver los valores de datos en uno o varios subgrupos. Los valores de datos basados en la selección de filtro se muestran en el lienzo.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Una vez definidos los grupos, puede habilitar el grupo de campos personalizados para la creación de informes en Análisis de rendimiento del modelo (posibles clientes) mediante la pestaña Análisis del ciclo de ingresos en Administración de posibles clientes de Marketo.

## Crear grupo de campos personalizados: editor de enteros {#create-custom-field-group-integer-editor}

1. Haga clic en **[!UICONTROL Base de datos de posibles clientes]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo organizador de campos]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Campo]** y seleccione un campo estándar o personalizado con un tipo de datos que se asigne al editor de cadenas (consulte la tabla de la sección anterior). [!UICONTROL Ingresos anuales] se utilizan aquí.

   ![](assets/nine.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/9.5.png)

   El nuevo grupo personalizado se muestra en el árbol de la base de datos de posibles clientes representado como Nombre de campo > Grupo de nombre de campo (ejemplo: Ingresos anuales > Grupo de ingresos anuales).

   ![](assets/9.6.png)

1. Haga clic en el nombre de grupo personalizado predeterminado sobre el editor de enteros para personalizar el nombre. Por ejemplo, puede cambiar el nombre de &quot;Grupo de ingresos anuales&quot; por &quot;Ingresos anuales por tamaño&quot;. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/eleven.png)

   El editor de enteros permite crear varios subgrupos para definir cada subgrupo por tamaño. En este ejemplo, se crearán tres grupos para pequeñas empresas, Medium y empresas.

1. Para agregar el primer grupo, escriba un nombre en el campo **[!UICONTROL Nombre del grupo]** (ejemplo: Pequeño) e introduzca un valor máximo en el campo **[!UICONTROL Intervalo del grupo]** (ejemplo: 200000). Haga clic en **[!UICONTROL Agregar grupo]**.

   ![](assets/twelve.png)

   Aparece una entrada de grupo vacía debajo del grupo que acaba de ingresar. El ejemplo siguiente muestra una entrada para pequeñas empresas, Medium y empresas.

   >[!NOTE]
   >
   >Puede añadir hasta diez subgrupos para categorizar los valores de datos. Cada entrada de intervalo de grupos se basa en la entrada anterior. Si deja en blanco la última entrada Rango de grupos para el último subgrupo personalizado que cree, no se establece un valor de datos máximo.

1. Haga clic en la pestaña Resumen para guardar y revisar la configuración.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Para eliminar un subgrupo, haga clic en la X roja junto al nombre del subgrupo.

1. En la página Resumen, revise la configuración.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Una vez definidos los grupos, puede habilitar el grupo de campos personalizados para la creación de informes en Análisis de rendimiento del modelo (posibles clientes) mediante la pestaña Análisis del ciclo de ingresos en Administración de posibles clientes de Marketo.

## Crear grupo de campos personalizados: editor de fechas {#create-custom-field-group-date-editor}

1. Haga clic en **[!UICONTROL Base de datos de posibles clientes]**.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo organizador de campos]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Campo]** y seleccione un campo estándar o personalizado con un tipo de datos que se asigne al editor de cadenas (consulte la tabla de la sección anterior). [!UICONTROL Fecha de adquisición] se usa aquí.

   ![](assets/fourteen.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/14.5.png)

   El nuevo grupo personalizado se muestra en el árbol de la base de datos de posibles clientes representado como Nombre de campo > Grupo de nombre de campo (ejemplo: Fecha de adquisición > Grupo de fecha de adquisición).

   ![](assets/14.6.png)

1. Haga clic en el nombre de grupo personalizado predeterminado sobre el editor de fechas para personalizar el nombre. Por ejemplo, puede cambiar el nombre &quot;Grupo de fecha de adquisición&quot; por &quot;Categorías de fecha de adquisición&quot;. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/fifteen.png)

   El editor de fechas permite crear varios subgrupos y definir cada subgrupo por fecha. En este ejemplo, se crean tres grupos: posibles clientes del primer trimestre de 15, posibles clientes del segundo trimestre de 15 y posibles clientes del tercer trimestre de 15.

1. Para agregar su primer grupo, escriba un nombre en el campo **[!UICONTROL Nombre del grupo]** (ejemplo: Posibles clientes del primer al 15 trimestre) e introduzca una fecha en el campo de fecha que represente la fecha en la que se adquirió el posible cliente o antes (ejemplo: 31/3/2015 para el último día del primer al 15 trimestre). Haga clic en **[!UICONTROL Agregar grupo]**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Puede añadir hasta diez subgrupos para categorizar los valores de datos. Cada entrada [!UICONTROL Intervalo de grupos] se genera a partir de la entrada anterior. Si deja en blanco la última entrada [!UICONTROL Intervalo del grupo] para el último subgrupo personalizado que cree, no se establece un valor de fecha de finalización.

   El ejemplo siguiente muestra una entrada para el primer trimestre de 2015 que va hasta el tercer trimestre.

   ![](assets/16.5.png)

   ¡Y eso es todo! Buen trabajo.
