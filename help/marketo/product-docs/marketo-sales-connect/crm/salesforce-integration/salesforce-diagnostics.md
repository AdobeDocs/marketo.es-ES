---
unique-page-id: 14745730
description: Diagnóstico de Salesforce - Documentos de Marketo - Documentación del producto
title: Diagnóstico de Salesforce
exl-id: a2b5bd10-bc92-4fd4-bc1b-4e02b48c9d83
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---

# Diagnóstico de Salesforce {#salesforce-diagnostics}

Parte de nuestra integración de Salesforce incluye una página de diagnóstico de Salesforce dentro de la aplicación web. Esta página captura los errores del registro de datos fallido en Salesforce. Los errores pueden resultar útiles, pero no siempre son legibles. Como tal, creamos una hoja de referencia que ayuda a explicar los mensajes de error.

**Error:** API_CURRENTLY_DISABLED\
**Categoría:** Acceso y validación\
**Mensaje:** La API está deshabilitada para este usuario\
**Qué está pasando:** El usuario no tiene acceso a API\
**Pasos para la resolución de problemas:** El administrador de Salesforce debe conceder acceso a la API del usuario.

<br> 

**Error:** AUTHENTICATION_FAILURE\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: error de autenticación\
**Qué está pasando:** Error de autenticación\
**Pasos para la resolución de problemas:** Desconéctese de Salesforce y vuelva a conectarse.

<br> 

**Error:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoría:** Acceso y validación\
**Mensaje:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;La sesión ha caducado o no es válida&quot;}\
**Qué está pasando:**

1 - El código de Déclencheur está causando que la actualización falle.\
2 - El usuario no tiene permisos de escritura a nivel de objeto en el objeto dado.

**Pasos para la resolución de problemas:**

1 - Revise el déclencheur que está fallando.\
2 - Otorgue acceso de escritura al usuario para el objeto O deshabilite la función que está intentando escribir en el objeto.

<br> 

**Error:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoría:** Otro\
**Mensaje:** no puede hacer referencia al posible cliente convertido\
**Qué está pasando:** Estamos intentando registrar en un posible cliente convertido durante el registro de actividad más reciente para contactos y posibles clientes. También he visto un par de estos para los tonos.\
**Pasos para la resolución de problemas:** Informe de cualquier instancia de esto a nuestra [equipo de asistencia](https://nation.marketo.com/t5/Support/ct-p/Support).

<br> 

**Error:** ENTITY_IS_LOCKED\
**Categoría:** Acceso y validación\
**Mensaje:** la entidad está bloqueada para su edición\
**Qué está pasando:** El registro se encuentra en un proceso de aprobación en el que se bloquea desde cualquier edición adicional hasta que una persona propietaria de la aprobación lo apruebe o rechace.\
**Pasos para la resolución de problemas:** Véase más arriba.

<br> 

**Error:** EXPIRED_ACCESS
**Categoría:** Autenticación
**Mensaje:** invalid_grant: token de acceso/actualización caducado
**Qué está pasando:** El token de acceso o actualización ha caducado. Los tokens caducan según [configuración de sesión en Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Pasos para la resolución de problemas:** Tendrá que volver a autenticarse. Desconecte la conexión de Salesforce y vuelva a conectar.

<br> 

**Error:** FAILED_WRITE\
**Categoría:** intermitente\
**Mensaje:** se ha llegado al final del archivo\
**Qué está pasando:** Problema de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos del lado del cliente.\
**Pasos para la resolución de problemas:** La lógica de reintento debe encargarse de esto. Si todavía no funciona, trabaje con su administrador de Salesforce para solucionar un déclencheur problemático.

<br> 

**Error:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoría:** Acceso y validación
**Mensaje:** Varía de cliente a cliente.
**Qué está pasando:** Error en una regla de validación personalizada para el objeto.
**Pasos para la resolución de problemas:** Compruebe la regla de validación personalizada que está causando este error. Dado que se trata de una regla personalizada, el error debe tratarse de forma aislada.

<br> 

**Error:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoría:** Acceso y validación\
**Mensaje:** El valor no existe o no coincide con los criterios de filtro\
**Qué está pasando:** Los datos incorrectos existentes en Salesforce se refuerzan al actualizarse.\
**Pasos para la resolución de problemas:** Véase más arriba.

<br> 

**Error:** FIELD_INTEGRITY_EXCEPTION\
**Categoría:** Acceso y validación\
**Mensaje:** El país o territorio existente no reconoce el valor de estado para el campo: Estado/Código de provincia\
**Qué está pasando:** Los datos incorrectos existentes en Salesforce se refuerzan al actualizarse.\
**Pasos para la resolución de problemas:** Véase más arriba.

<br> 

**Error:** INACTIVE_ORGANIZATION\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: organización inactiva\
**Qué está pasando:** Su organización de Salesforce ya no está activa.\
**Pasos para la resolución de problemas:** Desconéctese y vuelva a conectarse desde Salesforce.

**Error:** INACTIVE_USER
**Categoría:** Autenticación
**Mensaje:** invalid_grant: usuario inactivo
**Qué está pasando:** El usuario de Salesforce ya no está activo
**Pasos para la resolución de problemas:** Desconéctese y vuelva a conectarse desde Salesforce.

**Error:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MANTENANCE\
**Categoría:** intermitente\
**Mensaje:** (sin mensaje adicional)\
**Qué está pasando:** La instancia de Salesforce está en modo de mantenimiento.\
**Pasos para la resolución de problemas:** Espere hasta que se haya realizado el mantenimiento del sistema y vuelva a intentar el registro.

**Error:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoría:** Acceso y validación
**Mensaje:** derechos de acceso insuficientes en el id de objeto
**Qué está pasando:** No hay acceso al registro principal de una tarea.
**Pasos para la resolución de problemas:** Véase más arriba.

<br> 

**Error:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoría:** Acceso y validación
**Mensaje:** derechos de acceso insuficientes en el id de objeto
**Qué está pasando:** El registro de actividades más reciente no puede editar el registro específico porque el usuario no tiene acceso de escritura.\
**Pasos para la resolución de problemas:** Conceda al usuario acceso en Salesforce O deshabilite el registro de actividades más reciente para ese objeto para ese usuario.

**Error:** INVALID_FIELD\
**Categoría:** intermitente\
**Mensaje:** Net::ReadTimeout\
**Qué está pasando:** Se agota el tiempo de espera de la solicitud. Esto es probablemente el resultado de demasiadas transacciones lentas.\
**Pasos para la resolución de problemas:** Revise las personalizaciones existentes de los posibles culpables de los problemas de latencia o deshabilite el registro de actividades más reciente de uno o todos los objetos para reducir la carga.

**Error:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoría:** Acceso y validación\
**Mensaje:** No se pueden crear/actualizar campos: ToutApp__Tout_Last_Replied__c. Compruebe la configuración de seguridad de este campo.
**Qué está pasando:** Los usuarios no tienen acceso de escritura a los campos personalizados de Tout necesarios para realizar la transacción de registro de actividad más reciente. Es posible que el equipo haya instalado el paquete pero no haya habilitado los campos correctos para los usuarios.\
**Pasos para la resolución de problemas:** El administrador de Salesforce debe conceder acceso a los campos personalizados O desactivar el registro de actividades más reciente.

**Error:** INVALID_GRANT\
**Categoría:** Autenticación\
**Mensaje:** invalid_grant: ip restringida\
**Qué está pasando:** Estamos tratando de acceder a su Salesforce, pero tiene restricciones de IP que nos impiden hacerlo.\
**Pasos para la resolución de problemas:** El administrador de Salesforce deberá realizar la lista de permitidos de nuestras IP. Los usuarios deben ponerse en contacto con el servicio de asistencia para obtener las direcciones IP.

**Error:** INVALID_TYPE\
**Categoría:** Acceso y validación\
**Mensaje:** CreatedDate, (SELECT Id FROM Tasks) DESDE EL POSIBLE CLIENTE DONDE Email=&#39;emailid&#39;^ERROR en la fila:1:Columna:53sEl tipo de objeto &quot;Posible cliente&quot; no es compatible. Si está intentando utilizar un objeto personalizado, asegúrese de anexar &#39;__c&#39; después del nombre de entidad. Consulte su WSDL o la llamada descrita para obtener los nombres adecuados
**Qué está pasando:** Estamos intentando consultar un tipo de objeto de Salesforce al que el usuario no tiene acceso. Es muy probable que esto esté relacionado con que el usuario no tiene el acceso correcto al objeto Posible cliente.\
**Pasos para la resolución de problemas:** Conceda acceso de lectura y actualización al objeto Posible cliente en Salesforce o desactive el registro de correo electrónico y el registro de actividad más reciente en los registros de posibles clientes.

**Error:** QUERY_TIMEOUT\
**Categoría:** intermitente\
**Mensaje:** La solicitud de consulta se ejecutó demasiado tiempo\
**Qué está pasando:** Véase más arriba.\
**Pasos para la resolución de problemas:** La lógica de reintento debe encargarse de esto. Si sigue sin funcionar, trabaje con el administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** REQUEST_LIMIT_EXCEEDED\
**Categoría:** intermitente\
**Mensaje:**
1 - Se ha superado el límite de ConcurrentPerOrgLongTxn\
2 - Límite total de solicitudes excedido\
3 - ConcurrentRequest\
**Qué está pasando:**
1 - Se ha superado el límite de solicitudes concurrentes, probablemente debido a un código de déclencheur ineficiente.\
2 - Demasiadas integraciones ponen la organización más allá de la ventana móvil de 24 horas.\
**Pasos para la resolución de problemas:**
1 - Revise los déclencheur existentes en los objetos afectados. Deshabilite potencialmente el registro de resumen de uno o varios objetos.\
2 - Comprar más llamadas de API de Salesforce. Deshabilite potencialmente el registro de resumen de uno o varios objetos.

**Error:** REQUIRED_FIELD_MISSING\
**Categoría:** Acceso y validación\
**Mensaje:** Faltan campos obligatorios: `[Amount_Committed_Private_Capital__c]`
**Qué está pasando:** Esto suele ocurrir con el registro de actividad más reciente. Los campos personalizados se configuraron para que fueran obligatorios, pero tienen valores vacíos en ellos. Esto puede suceder si el registro se creó con un valor vacío del campo personalizado y, a continuación, se hizo necesario. El requisito se aplica cuando intentamos actualizar el registro, aunque no estemos tocando el campo personalizado.\
**Pasos para la resolución de problemas:** Actualice manualmente los valores de los campos que faltan. A continuación, puede volver a intentar enviar el mensaje desde ToutApp.

**Error:** SERVER_UNAVAILABLE\
**Categoría:** intermitente\
**Mensaje:** servidor demasiado ocupado\
**Qué está pasando:** Problema de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos del cliente\
**Pasos para la resolución de problemas:** La lógica de reintento debe encargarse de esto. Si todavía no funciona, trabaje con su administrador de Salesforce para solucionar un problema de déclencheur.

**Error:** TXN_SECURITY_NO_ACCESS\
**Categoría:** Acceso y validación\
**Mensaje:** La operación solicitada no está permitida debido a una directiva de seguridad en su organización. Póngase en contacto con su administrador.<br/>
**Qué está pasando:** Se ha configurado algún tipo de restricción de seguridad; consulte https://developer.salesforce.com/forums/?id=&quot;ID de registro&quot;\
**Pasos para la resolución de problemas:** Hable con el administrador de Salesforce y compruebe cuál puede ser la restricción específica.

**Error:** UNABLE_TO_LOCK_ROW\
**Categoría:** intermitente\
**Mensaje:** no se puede obtener acceso exclusivo a este registro o a 1 registro: &quot;ID de registro&quot;\
**Qué está pasando:** Es probable que haya un déclencheur que esté causando múltiples intentos de acceder al mismo registro, posiblemente en el caso de un correo electrónico de grupo.\
**Pasos para la resolución de problemas:** La lógica de reintento debe encargarse de esto. Si sigue sin funcionar, trabaje con el administrador de Salesforce para solucionar un déclencheur problemático.

**Error:** UNKNOWN_EXCEPTION
**Categoría:** Otro\
**Mensaje:** Excepción desconocida\
**Qué está pasando:** Excepción no controlada en Salesforce.\
**Pasos para la resolución de problemas:** Presente un caso con Salesforce y copie los valores numéricos en el mensaje de error. Este es código de Salesforce que no gestiona correctamente un error.
