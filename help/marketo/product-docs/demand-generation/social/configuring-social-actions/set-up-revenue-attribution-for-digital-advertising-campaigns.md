---
unique-page-id: 10098812
description: Configuración de la atribución de ingresos para campañas de publicidad digital - Marketo Docs - Documentación del producto
title: Configuración de la atribución de ingresos para campañas de publicidad digital
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Configuración de la atribución de ingresos para campañas de publicidad digital {#set-up-revenue-attribution-for-digital-advertising-campaigns}

A continuación se muestra cómo configurar la atribución de ingresos para canales y campañas de publicidad digital. Una vez configurada, puede realizar la atribución de ingresos de primer toque y de varios contactos para anuncios digitales del mismo modo que en otros programas de Marketo.

Después de configurar el primer programa de publicidad en Marketo, puede clonarlo y actualizarlo para otros canales. Por ejemplo, clone un programa de LinkedIn en uno de Facebook.

Con programas independientes, puede realizar un seguimiento del número de conversiones de cada uno y ver los programas en Analizador de programas, Analizador de influencias de oportunidades y otras funciones de Marketo Analytics.

>[!PREREQUISITES]
>
>* Configure una etiqueta de canal con valores de estado y éxito del programa (por ejemplo, publicidad digital o social pagada y PPC)
>* Cree o edite un formulario para pasar una cadena de consulta con la persona
>* Asegúrese de tener acceso a algunas funciones de análisis de ciclo de ingresos para informar sobre los canales y campañas de publicidad


## Crear un programa predeterminado {#create-a-default-program}

A diferencia de algunos programas (como el correo electrónico) que pueden ejecutarse periódicamente durante un período de tiempo específico, los programas predeterminados siempre están activados.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Haga clic en **Nuevo** y seleccione **Nuevo programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Si ya dispone de un programa, puede [clone it](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Siempre que clone un programa, asegúrese de reemplazar los nombres en los campos de cadena de consulta de las listas inteligentes.

1. Coloque el nuevo programa en una carpeta de campaña específica, una vez configurado el programa inicial.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una cadena de consulta pasada a través de la dirección URL ayuda a Marketo a saber en qué campaña de publicidad hizo clic alguien cuando se convirtió en persona en Marketo.
   >
   >Puede crear una metodología de cadena de consulta que incluya todas las variables que desee medir. Marketo usa estas variables para agregar personas a sus diferentes programas.
   >
   >Por ejemplo, puede utilizar Channel type_Channel__Asset_Region. Esto podría tener el siguiente aspecto: SP_FB_NewGuide_US. **Nota**: las abreviaturas ahorran espacio.
   >
   >O bien, configúrelo como Channel_Adsource_AssetName_Region_UniqueIdNumber. Esto podría tener el siguiente aspecto: Social-Paid_Facebook_NewGuide_NA_123.

## Creación de una campaña inteligente para nuevos nombres {#create-a-smart-campaign-for-new-names}

1. En la campaña inteligente, cree una lista inteligente que contenga dos déclencheur y dos filtros, como se muestra a continuación.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La cadena de consulta utilizada en los dos déclencheur y la variable **Programa que capturó el nombre** es exclusivo de usted. Las cadenas de consulta que se muestran aquí son solo por ejemplo. Si clona el campo, simplemente reemplace estos campos.

1. Cree un paso de flujo para cambiar el atributo a **Programa de adquisición** y establezca el valor nuevo en el valor que haya definido para las campañas sociales de pago.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Programe y active la campaña.

## Creación de una campaña inteligente para el estado o el éxito del programa {#create-a-smart-campaign-for-status-program-success}

Necesita una segunda campaña inteligente para cambiar el estado de las personas, de modo que logren el éxito del programa y se puedan incluir en los cálculos de atribución de ingresos.

1. En el **Rellena el formulario** déclencheur, introduzca el nombre del programa en la cadena de consulta. Si va a clonar el programa, reemplace el antiguo nombre de la cadena de consulta por el nuevo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Cree pasos de flujo para cambiar el estado a uno asociado con el éxito del programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >El ejemplo anterior muestra **Convertido**, pero esto depende de los valores de estado/éxito.

1. Programe y active la campaña.

## Crear una publicidad {#create-your-ad}

Después de configurar el programa y las campañas, cree la nueva publicidad.

1. Vaya al canal; Por ejemplo, LinkedIn o Facebook.
1. Cree una publicidad nueva.
1. Seleccione una página de aterrizaje de Marketo como destino para la llamada a la acción en la campaña.
1. Agregue la cadena de consulta a la dirección URL.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Así puede añadir toda la información configurada en una URL real. Los elementos se separan con un signo &amp;:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** es la fuente de persona utilizada como identificador de canal
   >* **comment** es el identificador único creado para cada programa
   >* **camp** es la campaña en Facebook, LinkedIn o Google
   >* **kk** es la palabra clave o el nombre de recurso que desea capturar

   >
   >**Estos cuatro términos deben estar en minúsculas y no puede haber espacios en la dirección URL para que se capture esta información.**

## Prácticas recomendadas {#best-practices}

Utilice una etiqueta de canal único para representar toda la publicidad digital, o utilice varias etiquetas de canal si desea realizar comparaciones más granulares con los demás canales de marketing (por ejemplo, Social-Paid, Search-Paid, Display, Retargeting).

A continuación, configure diferentes programas para cada vista de informes que necesite. Utilice un ID común como parámetro en la URL (BC, por ejemplo) de la cadena de consulta si tiene 10 regiones iniciando una &quot;Campaña Grande&quot; juntas y desea poder ver los resultados entre regiones.

Si desea informar sobre cada región y los resultados colectivos de la Gran Campaña, cree 11 programas, uno para cada región y otro para la Gran Campaña. Cada programa hace referencia únicamente a los caracteres relevantes de la cadena de consulta (como BC).

Hay superposición intencional en el recuento de personas entre la Gran Campaña y los programas de la región, por lo que no querrá informar sobre el recuento total de personas en los 11 programas, ya que algunas personas están tanto en la Gran Campaña como en uno de los programas de la región.
