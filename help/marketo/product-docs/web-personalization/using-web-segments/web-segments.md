---
unique-page-id: 4719093
description: Segmentos web - Documentos de Marketo - Documentación del producto
title: Segmentos web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2031'
ht-degree: 0%

---

# Segmentos web {#web-segments}

## Ver segmento {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

La pestaña Segmentos muestra todos los segmentos definidos personalizados que ha configurado en función de varios atributos.  **Un segmento es un conjunto de visitantes que cumplen los criterios especificados definidos en la página Definir un segmento.**  Un segmento puede ser visitante de un sector específico, una ubicación o en función de la actividad en el sitio del visitante.

En la personalización web, un visitante puede hacer coincidir más de un segmento. Por ejemplo, si hay un segmento para visitantes de EE. UU. y otro para empresas financieras, coincidiría un visitante web de Bank of America **ambos** el segmento para visitantes de EE. UU. y el segmento para empresas financieras.

**GRÁFICO:**  La página Segmentos muestra un gráfico de barras de los segmentos seleccionados según el número de visitantes del segmento (eje y) y el nombre del segmento (eje x).

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nombre</th> 
   <th colspan="1" rowspan="1">Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Nombre</strong></td> 
   <td colspan="1" rowspan="1">El título del segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Coincidencias</strong></p></td> 
   <td colspan="1" rowspan="1">El número de visitantes que cumplen los criterios personalizados y definidos del segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Definir campaña</strong></td> 
   <td colspan="1" rowspan="1">Permite configurar una CTA de campaña asociada al término de búsqueda seleccionado</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visitantes</strong></td> 
   <td colspan="1">Vista previa de la tabla de visitantes asociada al término de búsqueda seleccionado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Flujo de navegación</strong></td> 
   <td colspan="1" rowspan="1">Muestra una tabla de la actividad y la ruta URL del visitante en el sitio, así como la duración de su visita a cada página </td> 
  </tr> 
 </tbody> 
</table>

Consulte [cómo crear y ver etiquetas de segmentos](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmentos: panel derecho**

![](assets/image2014-11-12-10-3a46-3a32.png)

Al seleccionar un segmento en la tabla, se muestran detalles adicionales sobre el segmento en el panel derecho.

Estos detalles incluyen:

* Nombre del segmento
* Fecha de creación del segmento
* Las campañas asociadas que muestran las campañas que operan con el segmento. Al hacer clic en el número de reacciones, accederá a la página de campañas que muestra la CTA de campaña (llamada a la acción) del segmento
* El número de coincidencias (cantidad de visitantes que cumplieron los criterios del segmento) para el segmento y el número de visitantes distintos (únicos) que coincidieron con el segmento. Al hacer clic en el vínculo de visitante único, accederá a la página del visitante donde se muestran los resultados del segmento
* El propietario/creador de usuario del segmento
* Los sitios de dominio asociados con el segmento
* Un breve resumen de los criterios seleccionados del segmento

## Habilitar o deshabilitar un segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Para activar o desactivar un segmento, seleccione la casilla de ese segmento en la tabla y, en el cuadro desplegable &quot;Elegir acción&quot; en la parte inferior de la tabla, seleccione la acción &quot;Activar&quot; o &quot;Desactivar&quot;. Cuando un segmento está deshabilitado, se muestra la palabra &quot;deshabilitar&quot; en la columna Estado.

## Crear segmentos {#create-segments}

El segmento que cree cumple los criterios específicos que defina en la variable **Definir segmento** página. También puede personalizar los segmentos en función de una combinación de criterios y segmentar una audiencia específica en la campaña.

Para crear un nuevo segmento

Desde el **Segmentos** página, haga clic en **Crear nuevo** debajo del gráfico. Aparece la siguiente pantalla.

![](assets/four.png)

Defina parámetros generales para el segmento:

* **Nombre:**  Asigne un nombre al segmento.
* **Descripción:**  Proporcione una explicación más detallada de los criterios del segmento.
* **Dominios:**  Seleccione los dominios que desea incluir en el segmento.
* **Lógica de regla de segmento:**  Seleccione una lógica AND/OR para crear cada atributo de segmentación
* **Horario:** Defina el nivel de participación del visitante que desea en la campaña

   * **En la entrada**: Participación de cuando el visitante llega al sitio web
   * **Después del primer - noveno clic**: Capte al visitante después de una cantidad específica de clics en el sitio web

>[!TIP]
>
>**Lógica de regla de segmento**
>
>Hay tres opciones de filtro:
>
>1. Usar todos los filtros (1 y 2 y 3...)
>1. Utilice cualquier filtro (1, 2 o 3...)
>1. Filtros avanzados (con expresiones y/o )
>
>    Los filtros avanzados permiten controlar la condición del segmento. Introduzca los números de filtro separados por &quot;and&quot; y &quot;or&quot;.
>
>    * 1 y 2 y 3
>    * 1, 2 o 3
>
>    La combinación de &quot;y&quot; y &quot;o&quot; requiere paréntesis para aclarar la intención lógica. Por ejemplo, &quot;1 o 2 y 3&quot; debe escribirse de una de las siguientes maneras:
>
>    * 1 y (2 o 3)
>    * (1 y 2) o 3
>
>    Los paréntesis anidados se aceptan para lógicas más complicadas.
>
>    * (1 y 2) o (3 y 4)
>    * 1 y (2 o (3 y 4))
>
>    Compruebe la lógica después de insertar, eliminar o reordenar.

Arrastre y suelte los atributos de segmento de la columna derecha en el editor de segmentos de la izquierda:

![](assets/five.png)

### Firmografía {#firmographics}

**Ubicación**

Arrastrar y soltar **Ubicación** en el editor de segmentos.

* Seleccione entre los siguientes parámetros:

   * **Incluir** - Seleccione si quiere que la campaña incluya o excluya una ubicación.
   * **Seleccione el país que desea añadir** : En el cuadro desplegable, seleccione el país que desea incluir en el segmento. El nombre del país aparece a la derecha. Puede elegir varios países.

Una vez agregado el país, también puede especificar el estado, la ciudad y el código postal del segmento.

* **Seleccione el estado o la provincia que desea agregar** - En el cuadro desplegable, seleccione el estado de EE. UU. o la provincia canadiense que desee incluir. Puede realizar varias selecciones.
* **Código postal** : Introduzca el código postal que desea incluir en el segmento.
* **Ciudades** - Introduzca la ciudad o ciudades que desea incluir. Utilice un punto y coma entre ciudades.

>[!TIP]
>
>**¿Qué condiciones de segmento elijo? ¿&quot;AND&quot; u &quot;OR&quot;?** OR funciona como una opción adicional dentro de cada campo. Los clientes potenciales solo tienen que cumplir uno de los criterios seleccionados en cada campo para poder acceder al segmento. (Por ejemplo, los clientes potenciales pueden proceder de EE. UU. *o* de la industria de Defensa). Y funciona como un parámetro obligatorio adicional que debe cumplirse para este segmento. (Por ejemplo, las perspectivas deben ser tanto de Estados Unidos como de la industria de Defensa). Dentro de cada perfil de segmentación, cada campo independiente puede funcionar como ambos, ya sea como &quot;Y&quot; u &quot;O&quot; según la Condición del segmento seleccionada.

**Industrias** En el **Segmentación de perfiles** , marque la casilla junto a **Industria**.

* Seleccione entre los siguientes parámetros:

   * **Incluye** - Seleccione si quiere que el segmento incluya o excluya un sector.
   * **Seleccionar industrias que agregar** - Seleccione el sector que desea incluir en el segmento. El sector aparece debajo del cuadro desplegable. Puede elegir varias industrias.

**Grupo de organización**

En el **Segmentación de perfiles** , marque la casilla junto a **Grupo de organización.**

* En el cuadro desplegable, seleccione una de las siguientes opciones:

   * Fortune 500: incluye solo las compañías de Fortune 500 en este segmento
   * Fortune 1000: incluye solo las compañías de Fortune 1000 en este segmento
   * Global 2000: incluye las empresas de Global 2000 en este segmento
   * Empresa: incluye organizaciones con más de 1000 empleados y unos ingresos buenos a los 250 millones de dólares.
   * SMB: sólo incluye pequeñas y medianas empresas en este segmento

**-Cuentas con nombre-**

**Organizaciones**

* **Es de estas empresas (nombres específicos)**

   * Seleccione la empresa de destino en la lista desplegable &quot;Seleccionar empresa para agregar&quot;.
   * Puede escribir el nombre exacto de la organización a la que desea dirigirse. *Es _siempre_ Se recomienda utilizar Listas de cuentas con nombres en lugar de escribir los nombres manualmente para obtener mejores coincidencias (ver a continuación).

**Lista de cuentas con nombre**

Seleccione entre una [Lista de cuentas con nombre](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) para segmentar cuentas de destino clave.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>El número entre corchetes junto al nombre de la lista de cuentas con nombre se utiliza como referencia de índice para la lista de Web Personalization [API de lectura](https://developers.marketo.com/documentation/websites/rtp-js-api/).

**Excluir ISP**

Excluye a los proveedores de servicios de Internet (ISP) del segmento.

### Personas conocidas {#known-people}

**Base de datos**

La personalización web se integra con la base de datos de Marketo, lo que le permite segmentar y personalizar campañas por atributos y datos de personas conocidas.

Seleccione Base de datos y seleccione un campo de datos de persona de la lista desplegable. Seleccione el **+** para añadir campos desde la lista desplegable.

![](assets/seven.png)

Puede agregar o quitar campos de datos de personas desde Configuración de cuenta > Base de datos

>[!TIP]
>
>Cree sus criterios de segmento según todos los campos de datos de personas de Marketo, como puesto de trabajo, puntuación, función, etc.
>
>P. ej. &quot;Puesto igual a CMO&quot; y &quot;Puntuación menor o igual a 50&quot;

**Marketo Email Campaign** Segmente y personalice campañas por referencia de correo electrónico desde un visitante que hace clic en un correo electrónico de Marketo y llega al sitio. Segmente por nombre de programa de Marketo o de campaña y continúe la conversación desde el correo electrónico a la web. Seleccione el signo + para añadir campos de la lista desplegable.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Estado**

Defina su segmento según el estado de un cliente potencial: conocido o anónimo.

* Conocido: seleccione esta opción en el cuadro desplegable para visitantes conocidos. Un visitante es conocido cuando envía un formulario en su sitio web y aparece en la página Personas de personalización web.
* Anónimo: seleccione esta opción en el cuadro desplegable para visitantes anónimos.

![](assets/image2015-5-27-17-3a23-3a2.png)

### De comportamiento {#behavioral}

**Visitas -** Defina su segmento según el comportamiento de los visitantes o identifique.

* Número de visitas: seleccione esta opción en el cuadro desplegable para especificar el número de visitas de los posibles clientes en el sitio web.

   * Seleccione Igual a, Igual a o Bueno que o Igual a o Menor que en el cuadro desplegable.

* Visitas específicas: seleccione esta opción en el cuadro desplegable para especificar un visitante específico.

   * En el cuadro de texto de la derecha, introduzca el número de visitante que desea rastrear. El número de identificación único del visitante de Web Personalization se puede encontrar al hacer clic en un visitante (en la página de visitantes) y en Establecer campaña en el panel lateral derecho. El ID de visitante se encuentra en la sección Configuración avanzada. El ID de visitante también se puede encontrar en la dirección URL (por ejemplo, VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Términos de búsqueda** : Defina un segmento según los términos de búsqueda de un cliente potencial.

* El visitante buscó: en la lista desplegable, seleccione los términos que desee rastrear en la búsqueda de visitantes o agregue sus propios términos de búsqueda. (No es necesario el &#42; comodín en términos de búsqueda (ya que está configurado de forma predeterminada para incluir frases que contienen el término de búsqueda).

**Referencias** : Añada las direcciones URL a las que se refirió el visitante.

* Seleccionar referencias que agregar: en la lista desplegable, seleccione los sitios de referencia que desee rastrear o agregue su propia referencia. Una vez seleccionadas, las referencias aparecerán en el cuadro siguiente. (Utilizando &#42; como comodín (permitido)

**Incluir páginas** - Rastrear páginas específicas de los posibles clientes visitados en el sitio web.

* Coincidencias de URL: añada la URL de las páginas web específicas que desea rastrear. Puede agregar varias direcciones URL separándolas con un punto y coma. (Utilizando &#42; como comodín).

**Excluir páginas** - Excluya las páginas específicas que no quiera que coincidan en el segmento. (Utilizando &#42; como comodín).

* La URL no coincide: añada la URL de las páginas web específicas que desee excluir del seguimiento. Puede agregar varias direcciones URL separándolas con un punto y coma

![](assets/segment-extra.png)

### Dispositivo/navegador {#device-browser}

**Sistema operativo móvil**

Arrastre y suelte el sistema operativo móvil en el editor de segmentos

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo de visitante**<br />
  **Sistema operativo móvil** : En el cuadro desplegable, seleccione uno o varios sistemas operativos móviles de la lista. El sistema operativo móvil seleccionado aparece a continuación.

   * El visitante utiliza cualquier dispositivo móvil
   * El visitante utiliza este dispositivo/SO específico
   * El visitante no utiliza ningún dispositivo móvil

* **Dispositivo**  - En la lista desplegable, seleccione uno o más dispositivos (Apple, Samsung, LG, HTC, Nexus, Blackberry, etc.). Los dispositivos seleccionados aparecen a continuación.

**Navegador**

Visitante de Target que utiliza tipos de explorador o versiones específicos.

* Tipo de explorador: en el cuadro desplegable, seleccione uno o varios exploradores de Internet Los exploradores seleccionados aparecen a continuación.
* Versión del explorador: introduzca la versión del explorador que desea añadir al segmento. Puede seleccionar varias versiones separándolas con una coma. (Utilizando &#42; como comodín).

### API {#api}

**Eventos de datos** : Segmentar a los visitantes que almacenan en déclencheur eventos de datos personalizados específicos.

Añada el valor de Event que desee segmentar. Por ejemplo, de fuentes de datos de terceros.

**API de contexto de usuario**

Llamada de API de personalización web  [puede obtener más información al respecto aquí.](https://developers.marketo.com/documentation/websites/rtp-user-context-api/)

>[!TIP]
>
>**Uso de caracteres comodín:** Cuando desee incluir cualquier término de búsqueda o URL que contenga algo dentro de él, es decir, &quot;[google.com](https://google.com)&quot; o &quot;término de búsqueda producto&quot;, lo llamamos comodín y debe ser introducido con un asterisco - este pequeño chico&#42; - en cada extremo. Así que cualquier cosa que venga de [google.com](https://google.com) debe introducirse como &#42; [google.com](https://google.com)&#42;

## Editar segmentos {#edit-segments}

Puede editar un segmento que se haya creado.

1. Para editar un segmento, vaya a **Segmentos**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. En el **Segmentos** , haga clic en el icono de edición ( ![](assets/segment-edit.png)) del segmento que desea editar. El **Definir segmento** se abre la página con el segmento seleccionado.
1. Aplique las ediciones o cambios que desee realizar en el segmento.
1. Clic **Guardar**.

## Eliminar segmentos {#delete-segments}

Puede eliminar los segmentos que ha creado.

1. Desde el **Segmentos** página anterior, seleccione un segmento.
1. Haga clic en el icono Eliminar ( ![](assets/segment-delete.png) ) del segmento que desea eliminar.
1. Aparecerá un mensaje de confirmación que confirma que está a punto de eliminar el **Segmento**.

>[!NOTE]
>
>No puede eliminar un segmento asociado a una campaña. Primero debe eliminar la campaña y luego el segmento.

Excelente! Ahora que comprende la sección Segmentos, vamos a obtener más información sobre las campañas.

>[!MORELIKETHIS]
>
>* [Creación de un segmento web básico](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
>* [Creación de una nueva campaña web de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Creación de una nueva campaña web en la zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Creación de una nueva campaña web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
