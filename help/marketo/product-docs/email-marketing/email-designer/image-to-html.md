---
title: Integración de GenStudio para Marketo Engage
description: Aprenda a utilizar GenStudio en Marketo Engage.
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 6f1b4b6478e95d6d8aa332622daf2f29dd794bfe
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---

# Conversión de imágenes en plantillas de HTML {#image-to-html}

## Información general {#overview}

El conversor de imagen a HTML acelera de forma significativa la creación de correos electrónicos al convertir imágenes estáticas en plantillas de contenido de correo electrónico de HTML modulares y totalmente personalizables. Esta herramienta sin código le permite transformar diseños visuales de diseñadores gráficos o herramientas de diseño en plantillas de correo electrónico adaptables y editables que se pueden reutilizar una y otra vez.

Al aprovechar la tecnología de IA generativa, el conversor de imagen a HTML analiza el diseño, la tipografía, los colores y los elementos visuales de la imagen y genera un código HTML modular y limpio que mantiene la fidelidad del diseño, a la vez que garantiza la editabilidad y compatibilidad completas con el Designer de correo electrónico.

>[!PREREQUISITES]
>
>* Primero debe aceptar los [términos básicos de la generación de IA y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} para usar la funcionalidad de generación de IA en el Designer de correo electrónico. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
>* Debe tener _nombre de acceso_, así como _permisos de plantillas de correo electrónico de acceso_ habilitados [en su rol de Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#edit-a-role).

## Convertir una imagen {#convert-an-image}

Para convertir una imagen en una plantilla de correo electrónico de HTML totalmente personalizable, siga los pasos a continuación.

>[!NOTE]
>
>Para obtener los mejores resultados, utilice imágenes de alta calidad con elementos visuales claros y texto legible. Lo ideal es que las imágenes tengan entre 600 y 800 píxeles de ancho para coincidir con las dimensiones de correo electrónico estándar.

1. En _Design Studio_, haga clic en **Plantillas de correo electrónico** y luego en **Plantillas de correo electrónico (nuevas)**.

   ![](assets/image-to-html-1.png)

1. Haga clic en **[!UICONTROL Convertir imagen en plantilla]**.

   ![](assets/image-to-html-2.png)

1. Escriba un _nombre de plantilla_ y una descripción opcional. Además, también puede elegir el estilo de su marca. Cargue o arrastre y suelte la imagen deseada.

   ![](assets/image-to-html-3.png)

   EN PROFUNDIDAD, ¿PUEDO USAR DELETE PARA ESTA ETIQUETA DE PRECAUCIÓN?

   >[!CAUTION]
   >
   >Al cargar una imagen para su conversión, **todo el contenido que se agrega actualmente al correo electrónico se eliminará y se reemplazará** con la plantilla generada. Si tiene contenido existente en el correo electrónico, asegúrese de guardarlo antes de continuar con la conversión de la imagen.

   ¿EN QUÉ PROFUNDIDAD PUEDO UTILIZAR DELETE PARA ESTA ETIQUETA DE PRECAUCIÓN^^^

1. Desplácese hacia abajo y seleccione la casilla de verificación _El archivo de carga no contiene..._. Haga clic en **Convertir**.

   ![](assets/image-to-html-4.png)

   >[!NOTE]
   >
   >El proceso de generación puede tardar hasta cinco minutos en función de la complejidad y el tamaño del diseño de la imagen. El procesamiento de IA se produce en segundo plano, por lo que puede salir de esta pantalla y trabajar en otras tareas mientras la conversión está en curso. Es posible que tenga que actualizar la pantalla de la biblioteca _Plantilla de correo electrónico_ para ver el cambio de estado.

1. Una vez completada la conversión, la plantilla se guardará automáticamente como borrador. Selecciónelo..

   ![](assets/image-to-html-5.png)

1. La plantilla convertida se abre en el Designer de correo electrónico con funciones de edición completas. Ahora puede:

   * Editar contenido de texto y aplicar personalización
   * Modificación de imágenes y adición de vínculos
   * Ajuste de colores, fuentes y estilo
   * Agregar, quitar o reorganizar componentes de contenido
   * Aproveche todas las funciones de Email Designer como con cualquier otra plantilla

   ![](assets/image-to-html-6.png){width="800" zoomable="yes"}

1. Puede realizar los ajustes necesarios para perfeccionar la plantilla y adaptarla a las directrices de marca.

1. Una vez que esté satisfecho con la plantilla, haga clic en **[!UICONTROL Guardar y cerrar]** y luego en **Publicar**.

La plantilla ya está disponible en la biblioteca _Plantillas de correo electrónico_ y se puede usar al crear correos electrónicos.

## Casos de uso comunes {#use-cases}

El convertidor de imagen a HTML es ideal para:

* **Migración de la plataforma**: ¿Está migrando desde otra plataforma de marketing por correo electrónico? Convierta sus diseños de correo electrónico existentes en plantillas de HTML compatibles con Marketo Engage sin tener que volver a crear desde cero
* **Conversión de maqueta de diseño**: transforme maquetas de diseño de herramientas como Photoshop, Figma u otro software de diseño en plantillas de correo electrónico funcionales
* **Creación rápida de plantillas**: genere plantillas de correo electrónico rápidamente para campañas en las que el tiempo sea importante sin esperar los recursos para desarrolladores
* **Creación de bibliotecas de plantillas**: cree una biblioteca completa de plantillas compatibles con la marca que los integrantes del equipo no técnicos puedan personalizar e implementar

## Prácticas recomendadas {#best-practices}

**Antes de comenzar**

* **Guardar contenido existente**: al convertir una imagen a HTML, se reemplazará todo el contenido existente en el correo electrónico. Guarde siempre el trabajo actual antes de utilizar esta función.
* **Planifique el flujo de trabajo**: use el convertidor de imagen a HTML al principio del proceso de creación del correo electrónico o asegúrese de que está listo para reemplazar todo el contenido actual.

**Preparación de imágenes**

* **Resolución**: utilice imágenes de alta resolución para un mejor reconocimiento de texto y detección de elementos.
* **Claridad**: Asegúrese de que el texto sea claramente legible y de que los elementos visuales estén bien definidos.
* **Anchura**: Diseñe imágenes con anchuras de correo electrónico estándar (600-800 px) para que coincidan con los requisitos habituales de los clientes de correo electrónico.
* **Formato de archivo**: use el formato JPEG o PNG para evitar imágenes comprimidas o de baja calidad.
* **Diseño completo**: incluya el diseño de correo electrónico completo en una sola imagen, desde el encabezado hasta el pie de página.

**Consideraciones de diseño**

* **Diseños simples**: los diseños simples y bien estructurados se convierten con mayor precisión que los diseños muy complejos.
* **Elementos estándar**: utilice patrones de diseño de correo electrónico comunes (encabezado, secciones de cuerpo, CTA, pie de página).
* **Legibilidad del texto**: Asegúrese de que haya suficiente contraste entre el texto y los fondos.
* **Fuentes seguras para la Web**: Los diseños que usan fuentes seguras para la Web comunes tendrán una mejor fidelidad.
* **Evite elementos superpuestos**: Mantenga los elementos de diseño claramente separados para un mejor reconocimiento de la estructura.

**Después de la conversión**

* **Revise el borrador**: una vez completada la conversión, la plantilla se guardará automáticamente como borrador. Tómese tiempo para revisar cuidadosamente la HTML generada para comprobar su precisión.
* **Realizar pruebas exhaustivas**: probar el correo electrónico en distintos clientes y dispositivos de correo electrónico. Para obtener resultados más rápidos, aproveche la [integración Litmus](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).
* **Refinar manualmente**: realice los ajustes necesarios mediante las funciones de edición completas de Designer de correo electrónico.
* **Alineación de marca**: compruebe que los colores, las fuentes y el estilo coinciden con las directrices de marca.
* **Personalization**: agregue contenido dinámico y tokens de personalización según desee.
* **Accesibilidad**: revise y mejore las características de accesibilidad si es necesario.

## Limitaciones y consideraciones {#limitations}

Tenga en cuenta las siguientes limitaciones al utilizar el convertidor de imagen a HTML.

* **Interpretación de IA**: La IA genera HTML basándose en una interpretación visual de su imagen. Los diseños complejos o inusuales pueden requerir ajustes manuales después de la conversión.

* **Precisión del texto**: Mientras la IA intenta reconocer y reproducir el texto con precisión, compruebe siempre el contenido del texto y realice las correcciones necesarias.

* **Contenido dinámico**: el proceso de conversión crea HTML estático basado en la imagen. Después de la conversión, debe agregar manualmente la personalización, el contenido dinámico y el seguimiento.

* **Diseños complejos**: Es posible que los diseños muy complejos con capas complejas, formas inusuales o elementos no estándar no se conviertan a la perfección. Los diseños más simples generalmente arrojan mejores resultados.

* **Tiempo de procesamiento**: El proceso de conversión puede tardar hasta cinco minutos según la complejidad y el tamaño de la imagen. El procesamiento de IA se produce en segundo plano, lo que le permite trabajar en otras tareas sin mantener la pantalla abierta. La plantilla se guarda automáticamente como borrador una vez completada la conversión.

>[!NOTE]
>
>El conversor de imagen a HTML está diseñado para proporcionar un punto de partida sólido para la creación de correos electrónicos. La HTML generada debe revisarse y refinarse usando la Designer de correo electrónico para asegurarse de que cumple con sus requisitos.

## Preguntas frecuentes {#faq}

+++¿Qué sucede con el contenido del correo electrónico existente cuando utilizo el convertidor de imagen a HTML?

Todo el contenido existente en su correo electrónico se eliminará y se reemplazará por la plantilla recién generada al cargar una imagen para su conversión. Asegúrese de guardar cualquier contenido importante antes de utilizar esta función. Es mejor utilizar el conversor de imagen a HTML al principio del proceso de creación del correo electrónico.

+++

+++¿Qué formatos de archivo se admiten?

El convertidor de imagen a HTML es compatible con los formatos de imagen JPEG (.jpg, .jpeg) y PNG (.png).

+++

+++¿Cuánto tiempo tarda el proceso de conversión?

La conversión puede tardar hasta cinco minutos, según la complejidad y el tamaño del diseño de la imagen. El procesamiento de IA se produce en segundo plano, por lo que puede desplazarse y trabajar en otras tareas; no es necesario mantener la pantalla abierta. Una vez completada la conversión, el archivo se guardará automáticamente como borrador para que lo revise y edite.

+++

+++¿Puedo editar la plantilla generada?

¡Sí! La plantilla de HTML generada se abre en el Designer de correo electrónico con funciones de edición completas. Puede modificar todos los aspectos de la plantilla, incluidos el texto, las imágenes, el estilo, el diseño y la estructura.

+++

+++¿Qué sucede si la conversión no coincide exactamente con mi diseño?

La IA hace todo lo posible para interpretar con precisión su diseño, pero puede ser necesario un poco de refinamiento manual. Utilice la Designer de correo electrónico para ajustar cualquier elemento que necesite ajustes.

+++

+++¿Puedo utilizar esta función para páginas de aterrizaje u otros tipos de contenido?

El convertidor de imagen a HTML está diseñado actualmente específicamente para plantillas de correo electrónico. Para otros tipos de contenido, utilice las opciones de diseño e importación estándar disponibles en el Designer de correo electrónico.

+++

+++¿Puedo reutilizar plantillas convertidas en varias campañas de correo electrónico?

¡Sí! Las plantillas creadas con el convertidor de imagen a HTML se guardan automáticamente en la biblioteca _Plantillas de correo electrónico_. Puede acceder a ellas y reutilizarlas en cualquier mensaje de correo electrónico que reciba a partir de ahora.

+++
