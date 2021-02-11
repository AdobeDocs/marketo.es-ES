---
unique-page-id: 14745730
description: Diagnósticos de Salesforce - Documentos de marketing - Documentación del producto
title: Diagnóstico de Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---


# Diagnóstico de Salesforce {#salesforce-diagnostics}

Parte de nuestra integración de Salesforce incluye una página de diagnóstico de Salesforce dentro de la aplicación web. Esta página captura los errores del registro de datos fallido en Salesforce. Los errores pueden ser útiles, pero no siempre se pueden leer. Como tal, armamos una hoja de trucos que ayuda a explicar los mensajes de error.

**Error:** API_CURRENTLY_DISABLED\
**Categoría:** Acceso/Validación\
**Mensaje:** API deshabilitada para este usuario\
**Qué está sucediendo:** el usuario no tiene acceso a API\
**Pasos de solución de problemas: el administrador de** Salesforce debe conceder acceso a la API del usuario.

<br> 

**Error:** AUTHENTICATION_FAILURE\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: error de autenticación\
**Qué está sucediendo:error** de autenticación\
**Pasos de solución de problemas:** Desconectar de Salesforce y, a continuación, volver a conectar.

<br> 

**Error:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoría:** Acceso/Validación\
**Mensaje:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;mensaje&quot;:&quot;Sesión caducada o no válida&quot;}\
**Qué está pasando:**

1 - El código de Déclencheur está ocasionando que la actualización falle.\
2 - El usuario no tiene permisos de escritura a nivel de objeto en el objeto dado.

**Pasos de solución de problemas:**

1 - Revise el déclencheur que está fallando.\
2 - Otorgue al usuario acceso de escritura para el objeto O desactive la función que intenta escribir en el objeto.

<br> 

**Error:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoría:** Otro\
**Mensaje:** no se puede hacer referencia al lead convertido\
**Qué está sucediendo:** Estamos intentando registrar un posible cliente convertido durante el registro de Actividades más reciente para Contactos y Posibles clientes. También se han visto un par de estos en los campos.\
**Pasos de solución de problemas:** informe de cualquier caso de esto a nuestro equipo [ de ](https://nation.marketo.com/t5/Support/ct-p/Support)asistencia.

<br> 

**Error:** ENTITY_IS_LOCKED\
**Categoría:** Acceso/Validación\
**Mensaje:** la entidad está bloqueada para edición\
**Qué está sucediendo:** el registro se encuentra en un proceso de aprobación en el que se bloquea cualquier edición adicional hasta que una persona propietaria de la aprobación lo apruebe o lo rechace.\
**Pasos de solución de problemas:** consulte lo anterior.

<br> 

**Error:** EXPIRED_ACCESS, 
**Categoría:** Autenticación 
**Mensaje:** Invalid_Grant: token de acceso/actualización caducado 
**Qué está sucediendo:** El autentificador de acceso o actualización ha caducado. Los tokens caducan según la configuración de [sesión en Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Pasos de solución de problemas:** tendrá que volver a autenticarse. Desconecte la conexión de Salesforce y vuelva a conectarse.

<br> 

**Error:** FAILED_WRITE\
**Categoría:** intermitente\
**Mensaje:** final de archivo alcanzado\
**Qué está sucediendo: problema** de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos en el cliente.\
**Pasos de solución de problemas:la lógica** Reintentar debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar problemas de déclencheur.

<br> 

**Error:** FIELD_CUSTOM_VALIDATION_EXCEPTION 
**Categoría:** Access/Validation 
**Message:** Varía de cliente a cliente.
**Qué está sucediendo:** error en una regla de validación personalizada para el objeto.
**Pasos de solución de problemas:** compruebe la regla de validación personalizada que causa este error. Dado que se trata de una regla personalizada, el error se debe tratar de forma puntual.

<br> 

**Error:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El valor no existe o no coincide con los criterios de filtro\
**Qué está sucediendo: los datos incorrectos** existentes en Salesforce se aplican al actualizar.\
**Pasos de solución de problemas:** consulte lo anterior.

<br> 

**Error:** FIELD_INTEGRITY_EXCEPTION\
**Categoría:** Acceso/Validación\
**Mensaje:** El país o territorio existente no reconoce el valor de estado para el campo: Código de estado o provincia\
**Qué está sucediendo: los datos incorrectos** existentes en Salesforce se aplican al actualizar.\
**Pasos de solución de problemas:** consulte lo anterior.

<br> 

**Error:** INACTIVE_ORGANIZATION\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: organización inactiva\
**Qué está sucediendo:** su organización de Salesforce ya no está activa.\
**Pasos de solución de problemas:** Desconectar y volver a conectarse desde Salesforce.

**Error:** INACTIVE_USER 
**Categoría:** Autenticación 
**Mensaje:** Invalid_Grant: usuario inactivo 
**Qué está sucediendo:** El usuario de Salesforce ya no está activo 
**Resolución de problemas Pasos:** Desconectar y volver a conectarse de Salesforce.

**Error:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MANTENANCE\
**Categoría:** intermitente\
**Mensaje:** (sin mensaje adicional)\
**Qué está sucediendo:la instancia de** Salesforce está en modo de mantenimiento.\
**Pasos de solución de problemas:** espere a que se complete el mantenimiento del sistema y vuelva a intentar el registro.

**Error:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY, 
**Categoría:** Access/Validation 
**Message:** derechos de acceso insuficientes en el identificador de objeto 
**Qué está sucediendo:** Sin acceso al registro principal de una tarea.
**Pasos de solución de problemas:** consulte lo anterior.

<br> 

**Error:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoría:** Acceso/
**Mensaje de validación:derechos de acceso** insuficientes en la identificación de objetos 
**Qué está sucediendo:El registro de Actividades** más reciente no puede editar el registro específico porque el usuario no tiene acceso de escritura.\
**Pasos para la solución de problemas:** conceda al usuario acceso en Salesforce O desactive el registro de Actividades más reciente para ese objeto para ese usuario.

**Error:** INVALID_FIELD\
**Categoría:** intermitente\
**Mensaje:** Net::ReadTimeout\
**Lo que está sucediendo:** la solicitud está agotando el tiempo de espera. Esto es probablemente el resultado de demasiadas transacciones lentas.\
**Pasos de solución de problemas:** revise las personalizaciones existentes de posibles culpables de los problemas de latencia y/o deshabilite el registro de Actividades más recientes para uno o todos los objetos para reducir la carga.

**Error:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoría:** Acceso/Validación\
**Mensaje:** No se pueden crear o actualizar campos: ToutApp__Tout_Last_Replied__c. Compruebe la configuración de seguridad de este campo.
**Qué está sucediendo:** los usuarios no tienen acceso de escritura a los campos personalizados de Tout necesarios para realizar la transacción de registro de Actividades más reciente. Es posible que el equipo haya instalado el paquete pero no haya habilitado los campos correctos para los usuarios.\
**Pasos de solución de problemas: el administrador de** Salesforce debe conceder acceso a los campos personalizados O desactivar el registro de Actividades más reciente.

**Error:** INVALID_GRANT\
**Categoría:** Autenticación\
**Mensaje:** Invalid_Grant: ip restricted\
**Qué está pasando:** Estamos intentando acceder a su Salesforce, pero tiene restricciones de IP establecidas que nos impiden hacerlo.\
**Pasos de solución de problemas:** Su administrador de Salesforce deberá realizar listas de permitidos en nuestras IP. Los usuarios deben ponerse en contacto con la asistencia técnica para obtener las direcciones IP.

**Error:** INVALID_TYPE\
**Categoría:** Acceso/Validación\
**Mensaje:** createdDate, (SELECT Id FROM Tareas) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR en Fila:1:Columna:53sNo se admite el tipo de objeto &#39;Lead&#39;. Si intenta utilizar un objeto personalizado, asegúrese de anexar &#39;__c&#39; después del nombre de la entidad. Consulte su WSDL o describa la llamada para obtener los nombres adecuados
**Qué está sucediendo:** Estamos intentando consulta de un tipo de objeto de Salesforce al que el usuario no tiene acceso. Es muy probable que esté relacionado con que el usuario no tenga el acceso correcto al objeto principal.\
**Pasos para la solución de problemas:** conceda acceso de lectura y actualización al objeto Posible cliente en Salesforce, o desactive el registro por correo electrónico y el registro de Actividades más recientes en los registros de posibles clientes.

**Error:** CONSULTA_TIMEOUT\
**Categoría:** intermitente\
**Mensaje:** La solicitud de consulta se ejecutó demasiado tiempo\
**Qué está pasando:** ver arriba.\
**Pasos de solución de problemas:la lógica** Reintentar debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar problemas de déclencheur.

**Error:** REQUEST_LIMIT_EXCEEDED\
**Categoría:** intermitente\
**Mensaje:**
1 - Se ha superado el límite de ConcurrentPerOrgLongTxn\
2 - Se excedió el límite de solicitudes totales\
3 - ConcurrentRequest\
**Qué está sucediendo:**
1 - Se ha superado el límite de solicitudes simultáneas, probablemente debido a un código de déclencheur ineficiente.\
2 - Demasiadas integraciones colocan a la organización más allá de la ventana móvil de 24 horas.\
**Pasos de solución de problemas:**
1 - Revise los déclencheur existentes en los objetos afectados. Deshabilite potencialmente el registro resumido para uno o varios objetos.\
2 - Comprar más llamadas de API desde Salesforce. Deshabilite potencialmente el registro resumido para uno o varios objetos.

**Error:** REQUIRED_FIELD_MISSING\
**Categoría:** Acceso/Validación\
**Mensaje:** Faltan campos obligatorios:  `[Amount_Committed_Private_Capital__c]`
**Qué está sucediendo:** esto generalmente sucede con el registro de Actividades más reciente. Los campos personalizados se configuraron para que fueran obligatorios pero tienen valores vacíos. Esto puede suceder si el registro se creó con un valor vacío del campo personalizado y, a continuación, se hizo necesario. El requisito se impone cuando intentamos actualizar el registro, aunque no toquemos el campo personalizado.\
**Pasos de solución de problemas: actualice** manualmente los valores de los campos que faltan. A continuación, puede reintentar el mensaje desde ToutApp.

**Error:** SERVER_UNAVAILABLE\
**Categoría:** intermitente\
**Mensaje:** servidor demasiado ocupado\
**Qué está sucediendo:Problema** de rendimiento con Salesforce, probablemente debido a déclencheur subóptimos del cliente\
**Pasos de solución de problemas:la lógica** Reintentar debe gestionar esto. Si todavía no funciona, trabaje con su administrador de Salesforce para solucionar problemas con un déclencheur problemático.

**Error:** TXN_SECURITY_NO_ACCESS\
**Categoría:** Acceso/Validación\
**Mensaje:** La operación solicitada no está permitida debido a una política de seguridad en su organización. Póngase en contacto con el administrador.<br/>
**Qué está sucediendo:** Se ha configurado algún tipo de restricción de seguridad - consulte https://developer.salesforce.com/forums/?id=&quot;record ID&quot;\
**Pasos de solución de problemas:** póngase en contacto con el administrador de Salesforce y vea cuál puede ser la restricción específica.

**Error:** UNABLE_TO_LOCK_ROW\
**Categoría:** intermitente\
**Mensaje:** no se puede obtener acceso exclusivo a este registro o a 1 registros: &quot;ID del registro&quot;\
**Qué está sucediendo:** es probable que haya un déclencheur que esté provocando varios intentos de acceso al mismo registro, posiblemente en el caso de un correo electrónico de grupo.\
**Pasos de solución de problemas:la lógica** Reintentar debe gestionar esto. Si aún no funciona, trabaje con el administrador de Salesforce para solucionar problemas de déclencheur.

**Error:** UNKNOWN_EXCEPTION 
**Categoría:** Otro\
**Mensaje:Excepción** desconocida\
**Qué está pasando: excepción** no controlada en Salesforce.\
**Pasos de solución de problemas:** archivar un caso con Salesforce y copiar los valores numéricos en el mensaje de error. Se trata de un código de Salesforce que no gestiona correctamente un error.
