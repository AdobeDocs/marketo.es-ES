---
unique-page-id: 10098812
description: Configuración de la atribución de ingresos para Campañas de publicidad digital - Documentos de marketing - Documentación del producto
title: Configurar la atribución de ingresos para Campañas de publicidad digital
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Configurar la atribución de ingresos para Campañas de publicidad digital {#set-up-revenue-attribution-for-digital-advertising-campaigns}

A continuación se muestra cómo configurar la atribución de ingresos para canales y campañas de publicidad digital. Una vez configurada, puede realizar la atribución de ingresos de primer toque y de varios toques para anuncios digitales de la misma manera que en otros programas de marketing.

Después de configurar el primer programa de publicidad en Marketing, puede clonar y actualizarlo para otros canales. Por ejemplo, clona un programa de LinkedIn en uno de Facebook.

Con programas independientes, puede realizar un seguimiento del número de conversiones de cada una y ver sus programas en el Analizador de Programas, el Analizador de influencia de oportunidades y otras funciones de Análisis de marketing.

>[!PREREQUISITES]
>
>* Configure una etiqueta de canal con valores de estado y éxito de programa (por ejemplo, publicidad digital o social paga y PPC)
>* Crear o editar un formulario para pasar una cadena de consulta con la persona
>* Asegúrese de tener acceso a algunas funciones de análisis de ciclo de ingresos para informar sobre sus canales y campañas de publicidad


## Crear un Programa predeterminado {#create-a-default-program}

A diferencia de algunos programas (como el correo electrónico) que pueden ejecutarse periódicamente durante un período de tiempo específico, los programas predeterminados siempre están activados.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Haga clic en **Nuevo** y seleccione **Nuevo Programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Si ya tiene un programa en su lugar, puede [clonarlo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Siempre que clona un programa, asegúrese de reemplazar los nombres en los campos de cadena de consulta de las listas inteligentes.

1. Coloque el nuevo programa en una carpeta de campaña específica, después de definir el programa inicial.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una cadena de consulta que se pasa por la dirección URL ayuda a Marketing a saber en qué campaña de publicidad hizo clic alguien cuando se convirtió en una persona en Marketing.
   >
   >Puede crear una metodología de cadena de consulta que incluya todas las variables que desee medir. Marketing utiliza estas variables para agregar personas a sus distintos programas.
   >
   >Por ejemplo, puede utilizar Canal type_Canal__Asset__Region. Esto podría parecer: SP_FB_NewGuide_US. **Nota**: las abreviaturas ahorran espacio.
   >
   >O bien, configúrelo como Canal_Adsource_AssetName_Region_UniqueIdNumber. Esto podría tener el aspecto siguiente: Social-Paid_Facebook_NewGuide_NA_123.

## Crear una Campaña inteligente para nuevos nombres {#create-a-smart-campaign-for-new-names}

1. En la campaña inteligente, cree una lista inteligente que contenga dos déclencheur y dos filtros, como se muestra.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La cadena de consulta utilizada en los dos déclencheur y el filtro **Programa que capturó el nombre** es única para usted. Las cadenas de consulta que se muestran aquí son solo, por ejemplo. Si ha clonado el campo, simplemente reemplace estos campos.

1. Cree un paso de flujo para cambiar el atributo a **Programa de adquisición** y establezca el valor Nuevo en el valor definido para campañas sociales pagas.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Programe y active la campaña.

## Crear una Campaña inteligente para el estado/éxito del Programa {#create-a-smart-campaign-for-status-program-success}

Necesita una segunda campaña inteligente para cambiar el estado de las personas, de modo que puedan lograr el éxito de los Programas y estar incluidas en los cálculos de atribución de ingresos.

1. En el déclencheur **Rellena el formulario**, introduzca el nombre del programa en la cadena de consulta. Si está clonando el programa, simplemente reemplace el nombre de cadena de consulta antiguo por el nuevo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Cree pasos de flujo para cambiar el estado a uno asociado al éxito de programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >El ejemplo anterior muestra **Convertido**, pero esto depende de los valores de estado/éxito.

1. Programe y active la campaña.

## Crear la publicidad {#create-your-ad}

Después de configurar el programa y las campañas, cree la nueva publicidad.

1. Vaya al canal; Por ejemplo, LinkedIn o Facebook.
1. Cree una publicidad nueva.
1. Seleccione una página de aterrizaje de marketing como destino para la llamada a acción en la campaña.
1. Añada la cadena de consulta a la dirección URL.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Así puede agregar toda la información configurada en una dirección URL real. Los elementos están separados por un signo &amp;:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **** source es la fuente de personas que se utiliza como identificador de canal
   >* **** inicia el identificador único creado para cada programa
   >* **** Acampó la campaña en Facebook, LinkedIn o Google
   >* **** kkkis la palabra clave o el nombre del recurso que desea capturar

   >
   >**Estos cuatro términos deben estar en minúsculas y no puede haber espacios en la dirección URL para que se capture esta información.**

## Prácticas recomendadas {#best-practices}

Utilice una sola etiqueta de canal para representar toda la publicidad digital o utilice varias etiquetas de canal si desea realizar comparaciones más granulares con los demás canales de marketing (por ejemplo, Social-Paid, Search-Paid, Display, Retargeting).

A continuación, configure diferentes programas para cada vista de sistema de informes que necesite. Utilice un ID común como parámetro en la URL (por ejemplo, BC) de la cadena de consulta si tiene 10 regiones que inician una &quot;Gran Campaña&quot; juntas y desea poder realizar la vista de resultados en todas las regiones.

Si desea informar sobre cada región y los resultados colectivos de la Gran Campaña, cree 11 programas, uno para cada región y otro para la Gran Campaña. Cada programa hace referencia únicamente a los caracteres relevantes de la cadena de consulta (como BC).

Hay una superposición intencional en el recuento de personas entre la Gran Campaña y los programas de la región, por lo que no querrías informar sobre el recuento total de personas en los 11 programas, ya que algunas personas están tanto en la Gran Campaña como en uno de los programas de la región.
