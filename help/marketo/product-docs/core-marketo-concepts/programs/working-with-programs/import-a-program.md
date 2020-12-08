---
unique-page-id: 1147108
description: Importar un Programa - Documentos de marketing - Documentación del producto
title: Importación de un Programa
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---


# Importación de un Programa {#import-a-program}

Un programa se puede importar de una suscripción de marketing a otra. Por ejemplo, puede crear un programa en un simulador para pruebas y luego importarlo en la suscripción activa. Además, puede importar un programa precompilado desde la Biblioteca de Programas de Marketing to.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Importación de un Programa {#import-a-program-1}

1. Vaya a Actividades **de marketing.**

   ![](assets/ma.png)

1. Haga clic en **Nuevo **desplegable. Seleccione **Importar Programa**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >Importación de programa solo está disponible para usuarios que tienen roles con permiso de importación de Programa habilitado. Obtenga más información sobre la [administración de funciones y permisos](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)de usuario.
   >
   >
   >Para conectar una cuenta de simulación de pruebas a la suscripción activa, póngase en contacto con la asistencia técnica [de marketing](http://www.marketo.com/services/support/).

1. Seleccione una **Suscripción** de marketing y un programa para importar. Haga clic en **Siguiente**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Especifique una carpeta **de** Campaña para el programa importado. Haga clic en **Siguiente.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Asegúrese de que** ****Usar reglas de conflicto** predeterminadas está seleccionado. Las reglas de conflicto son necesarias cuando se importan programas en una instancia que tiene recursos del mismo nombre.

1. Detalles de previsualización e **Importar** el programa.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Un cuadro de diálogo muestra el progreso de importación de programas.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Recibirá una confirmación por correo electrónico una vez finalizada la importación.

>[!NOTE]
>
>Tendrá que volver a programar campañas de lote importadas y activar campañas de desencadenador. El sistema desactiva automáticamente los programas de campañas y activa campañas en el programa importado.

## Identifique los Programas pregenerados en la biblioteca de Programas de marketing {#identify-pre-built-programs-in-the-marketo-program-library}

La biblioteca de Programas de Marketing Cloud contiene programas creados previamente y probados que se pueden importar en la suscripción. Los programas disponibles incluyen:

1. **Nurtura básica de goteo.** Envía una serie de correos electrónicos separados por pasos de espera.
1. **gestión de datos.** Mantiene la integridad de los datos mediante campañas inteligentes.
1. **Correo electrónico con Página de aterrizaje.** Envía un correo electrónico inicial con una oferta, como &quot;descargar este documento técnico&quot;. A continuación se muestra un correo electrónico de confirmación o recordatorio. Incluye una página de aterrizaje con un formulario.
1. **Correo electrónico con estados de progresión.** Envía una explosión de correo con un vínculo rastreable para que la persona haga clic. Actualiza el estado de progresión de cada persona: Enviado, Abierto, Clic, etc.
1. **Momentos interesantes.** Crea momentos interesantes para que el equipo de ventas los mantenga en el circuito.
1. **página de aterrizaje con Autorresponder.** Use contenido descargable para conseguir nuevas personas y nutrirlas. Incluye páginas de aterrizaje y formularios.
1. **Ciclo de vida 2.** Utiliza la puntuación para mover a una persona de la lista nueva a la cualificada para marketing.
1. **Plantilla de correo electrónico móvil.** Una plantilla de correo electrónico adaptable probada con iPhone y Android. Determinadas versiones de aplicaciones de Android, MS Outlook, Exchange y de terceros como Gmail y Yahoo! Las aplicaciones móviles de correo no admiten la CSS necesaria para las plantillas interactivas. Le recomendamos que realice la prueba antes de enviar correos electrónicos.
1. **Apuestas de importación de programa.** Programa de apuestas para los que están probando la Biblioteca de Programas! Simplemente apruebe los correos electrónicos y la página de aterrizaje y active la campaña inteligente. A continuación, vista la página de aterrizaje aprobada, rellene el formulario, ¡y se le ingresa!
1. **Campañas disponibles de ventas.** Ofrece a sus representantes de ventas una forma de ejecutar campañas inteligentes de marketing desde un Panel en su CRM.
1. **Puntuación - Spark Edition.** Puntuación demográfica y de comportamiento capturada en un solo campo de puntuación. Incluye más de dos docenas de campañas relacionadas con la puntuación.
1. **Puntuación - Ediciones estándar y seleccionadas.** Puntuación demográfica y de comportamiento capturada en campos de puntuación separados. Incluye más de dos docenas de campañas relacionadas con la puntuación.
1. **Sincronizar nuevas personas con CRM.** La campaña que sincroniza nuevos usuarios con el sistema CRM. Asigna un estado de persona de tal manera que se reconoce que no está listo para las ventas.
1. **Seminario web con adaptador de Evento.** Un conjunto completo de correos electrónicos, como invitaciones y recordatorios, además de páginas de aterrizaje con formularios y campañas para mover personas a través del programa. Este programa recibe actualizaciones sobre registro, asistencia, etc. de proveedores de eventos en línea como WebEx.
1. **Seminario web sin adaptador de Evento.** Igual que antes, pero con procesos manuales para registrar el registro, la asistencia, etc.
1. **Programa** de Puntuación de Sirius Decisions. Este programa está diseñado para apoyar el modelo de puntuación estándar Sirius Decisions, incluyendo las reglas de puntuación implícitas y explícitas y la asignación de persona matrixed. Vista [este](http://docs.marketo.com/display/docs/assets/sirius-decisions-scoring-program-overview.pdf)PDF para obtener más información.

>[!CAUTION]
>
>Debe crear dos campos personalizados (&quot;Puntuación demográfica&quot; y &quot;Puntuación de comportamiento&quot;) antes de importar el programa Puntuación - Ediciones estándar y Seleccionar.

## Impacto en los activos externos durante las importaciones de Programas {#impact-on-external-assets-during-program-imports}

Los programas utilizan recursos externos como plantillas de correo electrónico, plantillas de página de aterrizaje, imágenes, formularios, tokens y etiquetas de programa. Tiene la capacidad de configurar la forma en que se administran las plantillas de página de aterrizaje y las etiquetas de programa, y Marketing administra automáticamente el resto.

**Plantillas de correo electrónico: **Las plantillas de correo electrónico se importan y crean automáticamente a menos que exista una con el mismo nombre.

**Plantillas de Página de aterrizaje: **Las plantillas de Página de aterrizaje se importan al estudio de diseño. Puede utilizar reglas de conflicto para configurar el comportamiento cuando exista una plantilla con el mismo nombre. Con la regla predeterminada, se agregará un número a una plantilla de página de aterrizaje si existe una con el mismo nombre. Por ejemplo, se creará una plantilla de página de aterrizaje denominada Plantilla estándar 1 si existe una plantilla estándar con el nombre Plantilla estándar.

**Imágenes: **Las imágenes utilizadas por las páginas de aterrizaje se importan al estudio de diseño a menos que exista una con el mismo nombre.

**Tokens: **Los tokens que viven fuera de un programa se convertirán en tokens locales durante el proceso de importación.

>[!CAUTION]
>
>El tipo de imagen de mis tokens no es compatible con las importaciones de programa. Si se importa un programa con un tipo de imagen, se importarán mis tokens, **no **se introducirán tokens.

**Etiquetas de Programa: **Puede utilizar reglas de conflicto para controlar cómo se tratarán las etiquetas de programa que no existan en la cuenta de destino. Si utiliza la regla predeterminada, se crearán las etiquetas de programa o puede omitir las etiquetas.  **Forms: **Los formularios externos se importarán automáticamente al estudio de diseño a menos que exista uno con el mismo nombre.

>[!CAUTION]
>
>Al importar un programa, se omitirán las páginas de aterrizaje o correos electrónicos que contengan contenido [](http://docs.marketo.com/x/yRAt) dinámico.

## Ver un video {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/KgvZssZ9WRkZgDsY1yZfms.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`