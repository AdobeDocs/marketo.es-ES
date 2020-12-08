---
unique-page-id: 14745730
description: Diagnósticos de Salesforce - Documentos de marketing - Documentación del producto
title: Diagnóstico de Salesforce
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Diagnóstico de Salesforce {#salesforce-diagnostics}

Parte de nuestra integración de Salesforce incluye una página de diagnóstico de Salesforce dentro de la aplicación web. Esta página captura los errores del registro de datos fallido en Salesforce. Los errores pueden ser útiles, pero no siempre se pueden leer. Como tal, armamos una hoja de trucos que ayuda a explicar los mensajes de error.

**Error:** API_CURRENTLY_DISABLED\
**Categoría:** Acceso/Validación\
**Mensaje:** API deshabilitada para este usuario\
**Qué está pasando:** El usuario no tiene acceso a API\
**Pasos de solución de problemas:** El administrador de Salesforce debe conceder acceso a la API del usuario.

<br> 

**Error:** AUTHENTICATION_FAILURE\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: error de autenticación\
**Qué está pasando:** Error de autenticación\
**Pasos de solución de problemas:** Desconecte de Salesforce y vuelva a conectarse.

<br> 

**Error:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoría:** Acceso/Validación\
**Mensaje:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;La sesión caducó o no es válida&quot;}\
**Qué está pasando:**

1 - El código de activación está ocasionando que la actualización falle.\
2 - El usuario no tiene permisos de escritura a nivel de objeto en el objeto dado.

**Pasos de solución de problemas:**

1 - El activador de revisión está fallando.\
2 - Otorgue al usuario acceso de escritura para el objeto O desactive la función que intenta escribir en el objeto.

<br> 

**Error:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoría:** Otros\
**Mensaje:** no se puede hacer referencia al lead convertido\
**Qué está pasando:** Estamos intentando iniciar sesión en un posible cliente convertido durante el registro de Actividades más reciente para Contactos y Posibles clientes. También se han visto un par de estos en los campos.\
**Pasos de solución de problemas:** Comuníquese con el equipo de [soporte técnico](http://nation.marketo.com/community/support_solutions)de cualquier caso.

<br> 

**Error:** ENTITY_IS_LOCKED\
**Categoría:** Acceso/Validación\
**Mensaje:** la entidad está bloqueada para edición\
**Qué está pasando:** El registro se encuentra en un proceso de aprobación donde se bloquea cualquier edición adicional hasta que una persona propietaria de la aprobación lo apruebe o lo rechace.\
**Pasos de solución de problemas:** Véase más arriba.

<br> 

**Error:** EXPIRED_ACCESS **Categoría:** Mensaje de autenticación **:** Invalid_Grant: token **de acceso/actualización caducado Qué está sucediendo:** El autentificador de acceso o actualización ha caducado. Los tokens caducan según la configuración de [sesión de Salesforce](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Pasos de solución de problemas:** Tendrá que volver a autenticarse. Desconecte la conexión de Salesforce y vuelva a conectarse.

<br> 

**Error:** FAILED_WRITE\
**Categoría:** Intermitente\
**Mensaje:** se alcanzó el final del archivo\
**Qué está pasando:** Problema de rendimiento con Salesforce, probablemente debido a desencadenantes no óptimos en el lado del cliente.\
**Pasos de solución de problemas:** La lógica de reintento debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar un problema de activación.

<br> 

**Error:** FIELD_CUSTOM_VALIDATION_EXCEPTION **Categoría:** Access/Validation **Message:** Varía de cliente a cliente.
**Qué está pasando:** Error en una regla de validación personalizada para el objeto.
**Pasos de solución de problemas:** Compruebe la regla de validación personalizada que causa este error. Dado que se trata de una regla personalizada, el error se debe tratar de forma puntual.

<br> 

**Error:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El valor no existe o no coincide con los criterios del filtro\
**Qué está pasando:** Los datos incorrectos existentes en Salesforce se aplican al actualizar.\
**Pasos de solución de problemas:** Véase más arriba.

<br> 

**Error:** FIELD_INTEGRITY_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El país o territorio existente no reconoce el valor del estado para el campo: Código de estado o provincia\
**Qué está pasando:** Los datos incorrectos existentes en Salesforce se aplican al actualizar.\
**Pasos de solución de problemas:** Véase más arriba.

<br> 

**Error:** INACTIVE_ORGANIZATION\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: organización inactiva\
**Qué está pasando:** La organización de Salesforce ya no está activa.\
**Pasos de solución de problemas:** Desconectar y volver a conectar de Salesforce.

**Error:** INACTIVE_USER **Categoría:** Mensaje de autenticación **:** Invalid_Grant: usuario **inactivo ¿Qué está sucediendo?:** El usuario de Salesforce ya no está activo **Pasos de solución de problemas:** Desconectar y volver a conectar de Salesforce.

**Error:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MANTENANCE\
**Categoría:** Intermitente\
**Mensaje:** (sin mensaje adicional)\
**Qué está pasando:** La instancia de Salesforce está en modo de mantenimiento.\
**Pasos de solución de problemas:** Espere hasta que se complete el mantenimiento del sistema y vuelva a intentar el registro.

**Error:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY **Categoría:** Access/Validation **Message:** derechos de acceso insuficientes en la identificación **de objetos Qué está sucediendo:** No hay acceso al registro principal de una tarea.
**Pasos de solución de problemas:** Véase más arriba.

<br> 

**Error:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoría:** Access/Validation** ****Mensaje:** derechos de acceso insuficientes en la identificación del objeto** ****Qué está sucediendo:** El registro de Actividades más reciente no puede editar el registro específico porque el usuario no tiene acceso de escritura.\
**Pasos de solución de problemas:** Otorgue al usuario acceso en Salesforce O desactive el registro de Actividades más recientes para ese objeto para ese usuario.

**Error:** INVALID_FIELD\
**Categoría:** Intermitente\
**Mensaje:** Net::ReadTimeout\
**Qué está pasando:** La solicitud está agotando el tiempo de espera. Esto es probablemente el resultado de demasiadas transacciones lentas.\
**Pasos de solución de problemas:** Revise las personalizaciones existentes de posibles culpables de los problemas de latencia y/o deshabilite el registro de Actividades más reciente de uno o todos los objetos para reducir la carga.

**Error:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoría:** Acceso/Validación\
**Mensaje:** No se pueden crear o actualizar campos: ToutApp__Tout_Last_Replied__c. Compruebe la configuración de seguridad de este campo.\
**Qué está pasando:** Los usuarios no tienen acceso de escritura a los campos personalizados de Tout necesarios para realizar la transacción de registro de Actividades más reciente. Es posible que el equipo haya instalado el paquete pero no haya habilitado los campos correctos para los usuarios.\
**Pasos de solución de problemas:** El administrador de Salesforce debe otorgar acceso a los campos personalizados O desactivar el registro de Actividades más reciente.

**Error:** INVALID_GRANT\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: ip restricted\
**Qué está pasando:** Estamos tratando de acceder a su Salesforce, pero tiene en vigor restricciones de IP que nos impiden hacerlo.\
**Pasos de solución de problemas:** El administrador de Salesforce tendrá que realizar listas de permitidos en nuestras IP. Los usuarios deben ponerse en contacto con la asistencia técnica para obtener las direcciones IP.

**Error:** INVALID_TYPE\
**Categoría:** Acceso/Validación\
**Mensaje:** createdDate, (SELECT Id FROM Tareas) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR en la fila:1:Column:53sNo se admite el tipo de objeto &#39;Lead&#39;. Si intenta utilizar un objeto personalizado, asegúrese de anexar &#39;__c&#39; después del nombre de la entidad. Consulte su WSDL o describa la llamada para obtener los nombres adecuados\
**Qué está pasando:** Estamos intentando consulta de un tipo de objeto de Salesforce al que el usuario no tiene acceso. Es muy probable que esté relacionado con que el usuario no tenga el acceso correcto al objeto principal.\
**Pasos de solución de problemas:** Otorgue acceso de lectura y actualización al objeto Posible cliente en Salesforce, o bien desactive el registro por correo electrónico y el registro de Actividades más recientes en los registros de posibles clientes.

**Error:** CONSULTA_TIMEOUT\
**Categoría:** Intermitente\
**Mensaje:** La solicitud de consulta se ejecutó demasiado tiempo\
**Qué está pasando:** Véase más arriba.\
**Pasos de solución de problemas:** La lógica de reintento debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar problemas con un activador problemático.

**Error:** REQUEST_LIMIT_EXCEEDED\
**Categoría:** Intermitente\
**Mensaje:**
1 - Se ha superado el límite de ConcurrentPerOrgLongTxn\
2 - Se excedió el límite de solicitudes totales\
3 - ConcurrentRequest\
**Qué está pasando:**
1 - Se ha superado el límite de solicitudes simultáneo, probablemente debido a un código de activación ineficiente.\
2 - Demasiadas integraciones colocan a la organización más allá de la ventana móvil de 24 horas.\
**Pasos de solución de problemas:**
1 - Revise los activadores existentes en los objetos afectados. Deshabilite potencialmente el registro resumido para uno o varios objetos.\
2 - Comprar más llamadas de API desde Salesforce. Deshabilite potencialmente el registro resumido para uno o varios objetos.

**Error:** REQUIRED_FIELD_MISSING\
**Categoría:** Acceso/Validación\
**Mensaje:** Faltan los campos obligatorios: [Amount_Commit_Private_Capital__c]\
**Qué está pasando:** Esto suele ocurrir en el registro de Actividades más reciente. Los campos personalizados se configuraron para que fueran obligatorios pero tienen valores vacíos. Esto puede suceder si el registro se creó con un valor vacío del campo personalizado y, a continuación, se hizo necesario. El requisito se impone cuando intentamos actualizar el registro, aunque no toquemos el campo personalizado.\
**Pasos de solución de problemas:** Actualice manualmente los valores de los campos que faltan. A continuación, puede reintentar el mensaje desde ToutApp.

**Error:** SERVER_UNAVAILABLE\
**Categoría:** Intermitente\
**Mensaje:** servidor demasiado ocupado\
**Qué está pasando:** Problema de rendimiento con Salesforce, probablemente debido a desencadenantes no óptimos del cliente\
**Pasos de solución de problemas:** La lógica de reintento debe gestionar esto. Si todavía no funciona, trabaje con el administrador de Salesforce para que le moleste disparar un activador problemático.

**Error:** TXN_SECURITY_NO_ACCESS\
**Categoría:** Acceso/Validación\
**Mensaje:** La operación solicitada no está permitida debido a una política de seguridad en su organización. Póngase en contacto con el administrador.\
**Qué está pasando:** Se ha configurado algún tipo de restricción de seguridad - consulte `https://developer.salesforce.com/forums/?id="record` ID&quot;\
**Pasos de solución de problemas:** Póngase en contacto con el administrador de Salesforce y vea cuál puede ser la restricción específica.

**Error:** UNABLE_TO_LOCK_ROW\
**Categoría:** Intermitente\
**Mensaje:** no se puede obtener acceso exclusivo a este registro o a 1 registro: &quot;ID del registro&quot;\
**Qué está pasando:** Es probable que haya un activador que esté ocasionando varios intentos de acceso al mismo registro, posiblemente en el caso de un correo electrónico de grupo.\
**Pasos de solución de problemas:** La lógica de reintento debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar problemas con un activador problemático.

**Error:** UNKNOWN_EXCEPTION\
**Categoría:** Otros\
**Mensaje:** Se produjo una excepción desconocida\
**Qué está pasando:** Excepción no controlada en Salesforce.\
**Pasos de solución de problemas:** Rellene un caso con Salesforce y copie los valores numéricos en el mensaje de error. Se trata de un código de Salesforce que no gestiona correctamente un error.
