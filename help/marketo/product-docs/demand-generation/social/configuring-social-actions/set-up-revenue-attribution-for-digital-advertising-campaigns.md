---
unique-page-id: 10098812
description: Configuración de la atribución de ingresos para campañas de Digital Advertising - Documentos de Marketo - Documentación del producto
title: Configuración de la atribución de ingresos para campañas de Digital Advertising
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Configuración de la atribución de ingresos para campañas de Digital Advertising {#set-up-revenue-attribution-for-digital-advertising-campaigns}

A continuación se indica cómo configurar la atribución de ingresos para canales y campañas de publicidad digital. Una vez configurada, puede realizar la atribución de ingresos de primer toque y multitoque para anuncios digitales del mismo modo que en otros programas de Marketo.

>[!IMPORTANT]
>
>El 31 de julio de 2024, empezamos el proceso de dejar de utilizar esta función. Ya no se pueden crear nuevos recursos. Los recursos existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Después de configurar el primer programa de publicidad en Marketo, puede clonarlo y actualizarlo para otros canales. Por ejemplo, clone un programa de LinkedIn en uno de Facebook.

Con programas separados, puede rastrear el número de conversiones de cada uno y ver sus programas en Analizador de programas, Analizador de influencia de oportunidades y otras funciones de Marketo Analytics.

>[!PREREQUISITES]
>
>* Configure una etiqueta de canal con valores de estado y éxito de programa (por ejemplo, Digital Advertising o PPC y pago social)
>* Cree o edite un formulario para pasar una cadena de consulta con la persona
>* Asegúrese de tener acceso a algunas funciones de análisis del ciclo de ingresos para informar sobre sus canales y campañas de publicidad

## Crear un programa predeterminado {#create-a-default-program}

A diferencia de algunos programas (como el correo electrónico) que pueden ejecutarse periódicamente durante un período de tiempo específico, los programas predeterminados siempre están activados.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Haga clic en **Nuevo** y seleccione **Nuevo programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Si ya tienes un programa, puedes [clonarlo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Siempre que clone un programa, asegúrese de reemplazar los nombres en los campos de cadena de consulta de las listas inteligentes.

1. Coloque el nuevo programa en una carpeta de campaña específica, después de configurar el programa inicial.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una cadena de consulta pasada a través de la dirección URL ayuda a Marketo a saber en qué campaña de publicidad hizo clic alguien cuando se convirtió en una persona en Marketo.
   >
   >Puede crear una metodología de cadena de consulta que incluya todas las variables que desee medir. Marketo utiliza estas variables para agregar personas a los distintos programas.
   >
   >Por ejemplo, puede utilizar el canal type_Channel__Asset__Region. Podría tener el siguiente aspecto: SP_FB_NewGuide_US. **Nota**: las abreviaciones ahorran espacio.
   >
   >O bien, configúrelo como Channel_Adsource_AssetName_Region_UniqueIdNumber. Este podría ser: Social-Paid_Facebook_NewGuide_NA_123.

## Creación de una campaña inteligente para nuevos nombres {#create-a-smart-campaign-for-new-names}

1. En la campaña inteligente, cree una lista inteligente que contenga dos déclencheur y dos filtros, como se muestra a continuación.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La cadena de consulta utilizada en los dos déclencheur y el filtro **Programa que capturó el nombre** son exclusivos de usted. Las cadenas de consulta que se muestran aquí solo son ejemplos. Si ha clonado el campo, simplemente reemplace estos campos.

1. Cree un paso de flujo para cambiar el atributo a **Programa de adquisición** y establezca el Nuevo valor en el valor que ha definido para las campañas sociales de pago.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Programe y active la campaña.

## Creación de una campaña inteligente para el éxito del estado/programa {#create-a-smart-campaign-for-status-program-success}

Se necesita una segunda campaña inteligente para cambiar el estado de las personas, de modo que puedan lograr el éxito del programa y se les incluya en los cálculos de atribución de ingresos.

1. En el déclencheur **Rellena formulario**, escriba el nombre del programa en la cadena de consulta. Si va a clonar el programa, reemplace el nombre de la cadena de consulta anterior por el nuevo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Cree pasos de flujo para cambiar el estado a uno asociado al éxito del programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >El ejemplo anterior muestra **Convertido**, pero esto depende de sus valores de estado/éxito.

1. Programe y active la campaña.

## Crear su anuncio {#create-your-ad}

Una vez configurados el programa y las campañas, cree el nuevo anuncio.

1. Vaya al canal; por ejemplo, LinkedIn o Facebook.
1. Cree un anuncio nuevo.
1. Seleccione una página de aterrizaje de Marketo como destino para la llamada a la acción en la campaña.
1. Añada la cadena de consulta a la dirección URL.

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >A continuación, se muestra cómo agregar toda la información configurada en una dirección URL real. Los elementos se separan con un signo &amp;:
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** es el Source de persona usado como identificador de canal
   >* **comment** es el identificador único creado para cada programa
   >* **camp** es la campaña en Facebook, LinkedIn o Google
   >* **kk** es la palabra clave o el nombre de recurso que desea capturar
   >
   >**Estos cuatro términos deben estar en minúscula y no puede haber espacios en la dirección URL para capturar esta información.**

## Mejores prácticas {#best-practices}

Utilice una sola etiqueta de canal para representar todos los canales de Digital Advertising o utilice varias etiquetas de canal si desea realizar comparaciones más granulares con otros canales de marketing (por ejemplo, pago social, búsqueda pagada, visualización y redireccionamiento).

A continuación, configure diferentes programas para cada vista de informes que necesite. Utilice un ID común como parámetro en la URL (BC, por ejemplo) en la cadena de consulta si tiene 10 regiones que inician una &quot;gran campaña&quot; juntas y desea poder ver los resultados entre regiones.

Si desea informar sobre cada región y los resultados colectivos de la Gran Campaña, cree 11 programas, uno para cada región y otro para la Gran Campaña. Cada programa hace referencia únicamente a los caracteres relevantes de la cadena de consulta (como BC).

Existe una superposición intencional en el recuento de personas entre la Gran Campaña y los programas de la región, por lo que no le gustaría informar sobre el recuento total de personas en los 11 programas, ya que algunas personas están tanto en la Gran Campaña como en uno de los programas de la región.
