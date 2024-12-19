---
description: 'Paso 1 de 3: Adición de campos de Marketo a Salesforce (Enterprise/Unlimited), documentación de Marketo: documentación del producto'
title: 'Paso 1 de 3: Adición de campos de Marketo a Salesforce (empresarial/ilimitado)'
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Debe tener acceso a las API de Salesforce para sincronizar entre Marketo Engage y Salesforce.

Marketo utiliza un conjunto de campos para capturar determinados tipos de información relacionada con el marketing. Si desea ver estos datos en Salesforce, siga las instrucciones que se indican a continuación.

1. Cree tres campos personalizados en Salesforce en los objetos de contacto y posible cliente: Puntuación, Programa de adquisición y Fecha de adquisición.
1. Asigne estos campos personalizados entre posibles clientes y contactos para que, al realizar la conversión en Salesforce, los valores se transfieran.
1. Si es necesario, puede crear otros campos adicionales (consulte la tabla siguiente).

Todos estos campos personalizados son opcionales y no son necesarios para sincronizar Marketo y Salesforce. Como práctica recomendada, le recomendamos que cree campos para Puntuación, Programa de adquisición y Fecha de adquisición.

## Añadir campos de Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Agregue tres campos personalizados a los objetos de contacto y posible cliente de Salesforce que se han indicado anteriormente. Si desea agregar más, consulte la tabla de campos disponibles al final de esta sección.

Siga estos pasos para cada uno de los tres campos personalizados para agregarlos. Comience con Puntuación.

1. Inicie sesión en Salesforce y haga clic en Configuración.

   CAPTURA DE PANTALLA

1. En la Búsqueda rápida, busque la palabra &quot;Objeto&quot;

   CAPTURA DE PANTALLA

1. Haga clic en Object Managers y busque &quot;Leads&quot;

   CAPTURA DE PANTALLA

1. Haga clic en Posible cliente en ETIQUETA y, a continuación, haga clic en Campos y relaciones a la izquierda.

   CAPTURA DE PANTALLA

1. Haga clic en el botón llamado Nuevo en la página &quot;Campos y relaciones&quot;

   CAPTURA DE PANTALLA

1. Elija el tipo de campo adecuado (para Puntuación - número; Programa de adquisición - texto; Fecha/hora de adquisición).

   CAPTURA DE PANTALLA

1. Haga clic en Siguiente.

   CAPTURA DE PANTALLA

1. Introduzca la Etiqueta de campo, Longitud y Nombre de campo para el campo, como se muestra en la tabla siguiente.

   TABLA

   >[!NOTE]
   >
   >Salesforce anexa __c a los nombres de campo cuando los utiliza para crear nombres de API.

   CAPTURA DE PANTALLA

   >[!NOTE]
   >
   >Los campos de texto y número requieren una longitud, pero los campos de fecha y hora no. Una descripción es opcional.

1. Haga clic en Siguiente.

   CAPTURA DE PANTALLA

1. Especifique la configuración de acceso y haga clic en Siguiente:

   Definir todas las funciones como Visible y Solo lectura

   Desactive la casilla de verificación Solo lectura para el perfil del usuario de sincronización:

   Si tiene un usuario con el perfil de un administrador del sistema como usuario de sincronización, desactive la casilla Solo lectura del perfil del administrador del sistema (como se muestra a continuación)
Si ha creado un perfil personalizado para el usuario de sincronización, desactive la casilla de verificación Solo lectura para ese perfil personalizado

   CAPTURA DE PANTALLA

1. Elija los diseños de página que deben mostrar el campo.

   CAPTURA DE PANTALLA

1. Haga clic en Guardar y nuevo para volver y crear cada uno de los otros dos campos personalizados. Haga clic en Guardar con si ha terminado con las tres.

   CAPTURA DE PANTALLA

* En el Administrador de objetos, busque &quot;Contactos&quot;. Haga clic en Campos y relaciones.
* Realice los pasos del 5 al 12 para los campos Puntuación, Fecha de adquisición y Programa de adquisición del objeto de contacto, tal como lo hizo para el objeto de posible cliente.
* De forma opcional, utilice el procedimiento anterior para cualquier campo personalizado adicional de esta tabla.

  TABLA

  >[!NOTE]
  >
  >Los valores de los campos asignados automáticamente por Marketo no estarán disponibles inmediatamente en Salesforce cuando se haya creado el nuevo campo. Marketo sincronizará los datos con Salesforce la próxima actualización del registro en cualquiera de los sistemas (es decir, una actualización de cualquiera de los campos sincronizados entre Marketo y Salesforce).

## Asignación de campos personalizados para conversiones {#map-custom-fields-for-conversions}

Un campo personalizado en el objeto de posible cliente de Salesforce debe asignarse a un campo de contacto en el objeto de contacto para que los datos se transfieran cuando se produzca una conversión.

1. En la esquina superior derecha, haga clic en Configuración.

   CAPTURA DE PANTALLA

1. En la Búsqueda rápida, busque la palabra &quot;Objeto&quot;

   CAPTURA DE PANTALLA

1. Vaya a la sección Campos personalizados y relaciones de posibles clientes y haga clic en Asignar campos de posibles clientes

   CAPTURA DE PANTALLA

1. Haga clic en la lista desplegable junto al campo que desee asignar, en la pestaña correspondiente: cuenta, contacto u oportunidad

   CAPTURA DE PANTALLA

1. Seleccione el campo personalizado de contacto correspondiente.

   CAPTURA DE PANTALLA

1. Repita los pasos anteriores para cualquier otro campo que haya creado.

1. Haga clic en Guardar cuando termine.
