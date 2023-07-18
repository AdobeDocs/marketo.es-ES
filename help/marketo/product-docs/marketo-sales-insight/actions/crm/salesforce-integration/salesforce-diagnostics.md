---
description: 'Diagnóstico de Salesforce: Documentos de Marketo: documentación del producto'
title: Diagnóstico de Salesforce
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: 15c3124a53ce55810b598c43e29e21321534c81f
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Diagnóstico de Salesforce {#salesforce-diagnostics}

Parte de nuestra integración con Salesforce incluye una página de diagnóstico de Salesforce dentro de la aplicación web. Esta página captura los errores del registro de datos fallido en Salesforce. Los errores pueden ser útiles, pero no siempre son legibles. Como tal, creamos una hoja de trucos que ayuda a explicar los mensajes de error.

## Diagnóstico de acceso {#access-diagnostics}

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/salesforce-diagnostics-1.png)

1. En Integraciones, haga clic en **Diagnóstico**.

   ![](assets/salesforce-diagnostics-2.png)

## Hoja de características de error {#error-cheat-sheet}

**Error:** API_CURRENTLY_DISABLED\
**Categoría:** Acceso/Validación\
**Mensaje:** La API está deshabilitada para este usuario\
**Qué está ocurriendo:** El usuario no tiene acceso a API\
**Pasos para solucionar problemas:** El administrador de Salesforce debe conceder al usuario acceso a la API.

**Error:** AUTHENTICATION_FAILURE\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: error de autenticación\
**Qué está ocurriendo:** Error de autenticación\
**Pasos para solucionar problemas:** Desconéctese de Salesforce y vuelva a conectarse.

**Error:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoría:** Acceso/Validación\
**Mensaje:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expire or invalid&quot;}\
**Qué está ocurriendo:**

1 - El código de Déclencheur está causando un error en la actualización.\
2 - El usuario no tiene permisos de escritura a nivel de objeto en el objeto dado.

**Pasos para solucionar problemas:**

1 - Revisar el déclencheur que está fallando.\
2 - Conceda acceso de escritura al usuario para el objeto O deshabilite la función que está intentando escribir en el objeto.

**Error:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoría:** Otros\
**Mensaje:** no puede hacer referencia al posible cliente convertido\
**Qué está ocurriendo:** Estamos intentando registrar en un posible cliente convertido durante el registro de actividades más recientes para contactos y posibles clientes. También he visto un par de estos para lanzamientos.\
**Pasos para solucionar problemas:** Informe de cualquier caso a nuestro [equipo de apoyo](https://nation.marketo.com/t5/Support/ct-p/Support).

**Error:** ENTITY_IS_LOCKED\
**Categoría:** Acceso/Validación\
**Mensaje:** la entidad está bloqueada para edición\
**Qué está ocurriendo:** El registro se encuentra en un proceso de aprobación en el que está bloqueado desde cualquier edición adicional hasta que lo aprueba o lo rechaza una persona propietaria de la aprobación.\
**Pasos para solucionar problemas:** Consulte lo anterior.

**Error:** EXPIRED_ACCESS
**Categoría:** Autenticación
**Mensaje:** invalid_grant: token de acceso/actualización caducado
**Qué está ocurriendo:** El token de acceso o actualización ha caducado. Los tokens caducan según el [configuración de sesión en Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Pasos para solucionar problemas:** Tendrá que volver a autenticarse. Desconecte la conexión de Salesforce y vuelva a conectarse.

**Error:** FAILED_WRITE\
**Categoría:** Intermitente\
**Mensaje:** fin de archivo alcanzado\
**Qué está ocurriendo:** Problema de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos del lado del cliente.\
**Pasos para solucionar problemas:** La lógica de reintento debe gestionar esto. Si sigue sin funcionar, colabore con su administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoría:** Acceso/Validación
**Mensaje:** Varía de un cliente a otro.
**Qué está ocurriendo:** Error en una regla de validación personalizada para el objeto.
**Pasos para solucionar problemas:** Compruebe la regla de validación personalizada que causa este error. Dado que se trata de una norma personalizada, el error debe tratarse de forma puntual.

**Error:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El valor no existe o no coincide con los criterios de filtro\
**Qué está ocurriendo:** Los datos incorrectos existentes en Salesforce se aplican tras la actualización.\
**Pasos para solucionar problemas:** Consulte lo anterior.

**Error:** FIELD_INTEGRITY_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El país o territorio existente no reconoce el valor de estado para el campo: Código de estado o provincia\
**Qué está ocurriendo:** Los datos incorrectos existentes en Salesforce se aplican tras la actualización.\
**Pasos para solucionar problemas:** Consulte lo anterior.

**Error:** INACTIVE_ORGANIZATION\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: organización inactiva\
**Qué está ocurriendo:** Su organización de Salesforce ya no está activa.
**Pasos para solucionar problemas:** Desconecte y vuelva a conectarse desde Salesforce.

**Error:** INACTIVE_USER
**Categoría:** Autenticación
**Mensaje:** invalid_grant: usuario inactivo
**Qué está ocurriendo:** El usuario de Salesforce ya no está activo
**Pasos para solucionar problemas:** Desconecte y vuelva a conectarse desde Salesforce.

**Error:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoría:** Intermitente\
**Mensaje:** (sin mensaje adicional)\
**Qué está ocurriendo:** La instancia de Salesforce está en modo de mantenimiento.\
**Pasos para solucionar problemas:** Espere hasta que se complete el mantenimiento del sistema y vuelva a intentar el registro.

**Error:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoría:** Acceso/Validación
**Mensaje:** derechos de acceso insuficientes en id de objeto
**Qué está ocurriendo:** No hay acceso al registro principal de una tarea.
**Pasos para solucionar problemas:** Consulte lo anterior.

**Error:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoría:** Acceso/Validación
**Mensaje:** derechos de acceso insuficientes en id de objeto
**Qué está ocurriendo:** El registro de actividades más recientes no puede editar el registro específico porque el usuario no tiene acceso de escritura.\
**Pasos para solucionar problemas:** Conceda al usuario acceso en Salesforce O deshabilite el registro de actividades más recientes para ese objeto para ese usuario.

**Error:** INVALID_FIELD\
**Categoría:** Intermitente\
**Mensaje:** Net::ReadTimeout\
**Qué está ocurriendo:** La solicitud está agotando el tiempo de espera. Esto es probablemente el resultado de demasiadas transacciones lentas.\
**Pasos para solucionar problemas:** Revise las personalizaciones existentes para detectar posibles culpables de los problemas de latencia o deshabilite el registro de actividades más recientes para uno o todos los objetos a fin de reducir la carga.

**Error:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoría:** Acceso/Validación\
**Mensaje:** No se pueden crear/actualizar los campos: MSE_Replied__c. Compruebe la configuración de seguridad de este campo.
**Qué está ocurriendo:** Los usuarios no tienen acceso de escritura a los campos personalizados de acciones de perspectiva de ventas necesarios para realizar la transacción de registro de actividad más reciente. Es posible que el equipo haya instalado el paquete, pero no ha habilitado los campos correctos para los usuarios.\
**Pasos para solucionar problemas:** El administrador de Salesforce debe conceder acceso a los campos personalizados O desactivar el registro de actividades más recientes.

**Error:** INVALID_GRANT\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: ip restringida\
**Qué está ocurriendo:** Estamos intentando acceder a su Salesforce, pero existen restricciones de IP que nos impiden hacerlo.\
**Pasos para solucionar problemas:** El administrador de Salesforce deberá realizar la lista de permitidos de sus IP. Los usuarios deben ponerse en contacto con Asistencia técnica para obtener las direcciones IP.

**Error:** INVALID_TYPE\
**Categoría:** Acceso/Validación\
**Mensaje:** CreatedDate, (SELECT Id FROM Tasks) FROM Posible cliente WHERE Email=&#39;emailid&#39;^ERROR at Row:1:No se admite el tipo de objeto Column:53s &#39;Posible cliente&#39;. Si intenta utilizar un objeto personalizado, asegúrese de anexar &quot;__c&quot; después del nombre de la entidad. Consulte su WSDL o la llamada de descripción para obtener los nombres adecuados
**Qué está ocurriendo:** Estamos intentando consultar un tipo de objeto de Salesforce al que el usuario no tiene acceso. Es muy probable que esto esté relacionado con que el usuario no tenga el acceso correcto al objeto de posible cliente.\
**Pasos para solucionar problemas:** Conceda acceso de lectura y actualización al objeto de posible cliente en Salesforce o desactive el registro de correo electrónico y el registro de actividades más recientes en los registros de posibles clientes.

**Error:** QUERY_TIMEOUT\
**Categoría:** Intermitente\
**Mensaje:** La solicitud de consulta se estaba ejecutando demasiado tiempo\
**Qué está ocurriendo:** Consulte lo anterior.\
**Pasos para solucionar problemas:** La lógica de reintento debe gestionar esto. Si sigue sin funcionar, colabore con su administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** REQUEST_LIMIT_EXCEEDED\
**Categoría:** Intermitente\
**Mensaje:**
1 - Límite de ConcurrentPerOrgLongTxn excedido\
2 - Límite total de solicitudes excedido\
3 - ConcurrentRequest\
**Qué está ocurriendo:**
1 - Se ha superado el límite de solicitudes simultáneas, probablemente debido a un código de déclencheur ineficiente.\
2 - Demasiadas integraciones colocan a la organización más allá de la ventana móvil de 24 horas.\
**Pasos para solucionar problemas:**
1 - Revise los déclencheur existentes en los objetos afectados. Se puede deshabilitar el registro de resumen de uno o más objetos.\
2 - Comprar más llamadas de API desde Salesforce. Se puede deshabilitar el registro de resumen de uno o más objetos.

**Error:** REQUIRED_FIELD_MISSING\
**Categoría:** Acceso/Validación\
**Mensaje:** Faltan campos obligatorios: `[Amount_Committed_Private_Capital__c]`
**Qué está ocurriendo:** Esto suele ocurrir en el registro de actividades más recientes. Los campos personalizados se han configurado para ser obligatorios, pero contienen valores vacíos. Esto puede suceder si el registro se creó con un valor vacío del campo personalizado y, a continuación, se hizo obligatorio. El requisito se aplica cuando intentamos actualizar el registro, aunque no estemos tocando el campo personalizado.\
**Pasos para solucionar problemas:** Actualice manualmente los valores de los campos que faltan. A continuación, puede volver a intentar enviar el mensaje desde Acciones de perspectiva de ventas.

**Error:** SERVER_UNAVAILABLE\
**Categoría:** Intermitente\
**Mensaje:** servidor demasiado ocupado\
**Qué está ocurriendo:** Problema de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos por parte del cliente\
**Pasos para solucionar problemas:** La lógica de reintento debe gestionar esto. Si sigue sin funcionar, colabore con su administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** TXN_SECURITY_NO_ACCESS\
**Categoría:** Acceso/Validación\
**Mensaje:** La operación solicitada no está permitida debido a una directiva de seguridad de su organización. Póngase en contacto con su administrador o administradora.
**Qué está ocurriendo:** Se ha configurado algún tipo de restricción de seguridad; consulte https://developer.salesforce.com/forums/?id=&quot;id. de registro&quot;\
**Pasos para solucionar problemas:** Hable con el administrador de Salesforce y vea cuál puede ser la restricción específica.

**Error:** UNABLE_TO_LOCK_ROW\
**Categoría:** Intermitente\
**Mensaje:** no se puede obtener acceso exclusivo a este registro o a 1 registros: &quot;id. de registro&quot;\
**Qué está ocurriendo:** Es probable que haya un déclencheur que esté causando varios intentos de acceso al mismo registro, posiblemente en el caso de un correo electrónico de grupo.\
**Pasos para solucionar problemas:** La lógica de reintento debe gestionar esto. Si sigue sin funcionar, colabore con su administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** UNKNOWN_EXCEPTION
**Categoría:** Otros\
**Mensaje:** Excepción desconocida\
**Qué está ocurriendo:** Excepción no controlada en Salesforce.\
**Pasos para solucionar problemas:** Registre un caso con Salesforce y copie los valores numéricos en el mensaje de error. Este es un código de Salesforce que no gestiona un error correctamente.
