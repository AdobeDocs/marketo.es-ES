---
description: 'Estado de sincronización de Salesforce: Documentos de Marketo: documentación del producto'
title: Estado de sincronización de Salesforce
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 6%

---

# Estado de sincronización de Salesforce {#salesforce-sync-status}

Utilice el panel Estado de sincronización para ver las estadísticas de sincronización como parte de los pasos de sincronización y su estado de éxito.

Los pasos de sincronización reflejan las operaciones de inserción o extracción de cada tipo de objeto para el esquema de objeto y los propios datos. Las estadísticas abarcan nuevos registros, actualizaciones, eliminaciones y recuentos de errores durante la sincronización. Los usuarios pueden filtrar por fecha, tipo de operación o tipo de objeto. El panel Estado de sincronización muestra el estado de los ciclos de sincronización de los últimos cinco días.

>[!NOTE]
>
>Permisos de administración necesarios

## Ver estado de sincronización {#view-sync-status}

1. Clic **Administrador**.

   ![](assets/salesforce-sync-status-1.png)

1. En Integración, haga clic en Salesforce y, a continuación, en la pestaña Estado de sincronización.

   ![](assets/salesforce-sync-status-2.png)

De forma predeterminada, las estadísticas se ordenarán por las iniciadas más recientemente. Puede ordenar por Iniciado en o Finalizado en (de más reciente a más antiguo) haciendo clic en el icono ordenar.

![](assets/salesforce-sync-status-3.png)

## Estado de sincronización de filtro {#filter-sync-status}

1. Para filtrar los datos, haga clic en el icono de filtro situado en el extremo derecho de la página.

   ![](assets/salesforce-sync-status-4.png)

1. Seleccione la fecha y el intervalo de tiempo y, a continuación, haga clic en las listas desplegables para filtrar por Tipo de objeto, Tipo de operación o Tipo de estado.

   ![](assets/salesforce-sync-status-5.png)

1. Clic **Aplicar**.

   ![](assets/salesforce-sync-status-6.png)

**PASO OPCIONAL**: Para exportar los errores de sincronización, haga clic en **Exportar**. Los datos se exportarán como CSV.

![](assets/salesforce-sync-status-7.png)

## Campos de estado de sincronización {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo</th> 
   <th>Descripción</th> 
   <th>Valores de enumeración</th> 
  </tr> 
  <tr> 
   <td colspan="1">Comenzó el</td> 
   <td colspan="1">La fecha y hora de inicio del ciclo de sincronización (zona horaria del usuario)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Finalizó el</td> 
   <td colspan="1">La fecha y hora de finalización del ciclo de sincronización (zona horaria del usuario)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objeto</td> 
   <td colspan="1">Tipo de objeto</td> 
   <td colspan="1">Contacto, Persona, Tarea, Oportunidad, Posible cliente, Otros como se muestra a continuación</td> 
  </tr>  
  <tr> 
   <td colspan="1">Operación</td> 
   <td colspan="1">Tipo de operación</td> 
   <td colspan="1">Tipos de operaciones como se muestra a continuación</td> 
  </tr>  
  <tr> 
   <td colspan="1">Estado</td> 
   <td colspan="1">Estado del lote</td> 
   <td colspan="1">Correcto, Fallido, Incompleto, En Proceso, Limpiado*</td> 
  </tr>
  <tr> 
   <td colspan="1">Nuevo</td> 
   <td colspan="1">Recuento de registros nuevos</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Actualizado</td> 
   <td colspan="1">Recuento de registros actualizados</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Eliminado</td> 
   <td colspan="1">Recuento de registros eliminados</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Elemento fallido</td> 
   <td colspan="1">Número de registros cuya sincronización falló</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Omitido</td> 
   <td colspan="1">Recuento de registros omitidos porque no se produjeron cambios en los campos de interés de la sincronización</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;Los datos se revirtieron al estado de integridad anterior después de un error en el paso de sincronización.

## Tipo de objeto {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">Cuenta</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tipo de cuenta</td> 
  </tr> 
  <tr> 
   <td colspan="1"> objetos personalizados de </td> 
  </tr>  
  <tr> 
   <td colspan="1">Campaña</td> 
  </tr>  
  <tr> 
   <td colspan="1">Estado de membresía de la campaña</td> 
  </tr>
  <tr> 
   <td colspan="1">Contacto</td> 
  </tr>  
  <tr> 
   <td colspan="1">Plantilla de email</td> 
  </tr>  
  <tr> 
   <td colspan="1">Evento</td> 
  </tr> 
  <tr> 
   <td colspan="1">Persona (posible cliente)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Oportunidad</td> 
  </tr>  
  <tr> 
   <td colspan="1">Rol del contacto y la oportunidad</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tarea</td> 
  </tr>  
  <tr> 
   <td colspan="1">Usuario</td> 
  </tr>  
 </tbody> 
</table>

## Tipo de operación {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Tipo de operación</th> 
   <th>Encontrado con estos objetos</th> 
   <th>Observaciones</th> 
   <th>Tipo de operación</th>
  </tr> 
  <tr> 
   <td colspan="1">Iniciar vínculo con el programa</td> 
   <td colspan="1">Campaña</td> 
   <td colspan="1">Vinculación de campañas a programas</td> 
   <td colspan="1">Actualizar</td>
  </tr>  
  <tr> 
   <td colspan="1">Extraer conversiones</td> 
   <td colspan="1">Persona (posible cliente)*</td> 
   <td colspan="1">Extraer y convertir acciones de SFDC a Marketo. Las unidades (números) son posibles clientes que se convierten en contactos</td> 
   <td colspan="1">Actualización, elemento fallido u omitido</td>
  </tr> 
  <tr> 
   <td colspan="1">Eliminaciones de extracción</td> 
   <td colspan="1">Contacto, Persona (Posible Cliente), Oportunidad, Campaña, Miembros De La Campaña, Contacto De Oportunidad, Objetos Personalizados, Campañas, Estado De Miembro De La Campaña, Función De Contacto De Oportunidad</td> 
   <td colspan="1">Registros eliminados de SFDC que se sincronizan con Marketo</td> 
   <td colspan="1">Eliminado, Elemento fallido u Omitido</td>
  </tr>  
  <tr> 
   <td colspan="1">Actualizaciones de extracción</td> 
   <td colspan="1">Tarea, Persona (posible cliente), Cola de persona (posible cliente), Contacto, Evento, Oportunidad, Cuenta, Tipo de cuenta, Miembros de campaña, Objetos personalizados, Campañas, Estado de miembro de campaña, Eventos, Estado de persona, Oportunidad, Función de contacto de oportunidad</td> 
   <td colspan="1">Actualizaciones de nuevos registros en SFDC sincronizados con Marketo, extraer eventos como actividades</td> 
   <td colspan="1">Elemento nuevo, actualizado, con error u omitido</td>
  </tr>  
  <tr> 
   <td colspan="1">Insertar nuevo</td> 
   <td colspan="1">Tareas, Plantillas de correo electrónico</td> 
   <td colspan="1">Tareas push (actividades)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Actualizaciones push</td> 
   <td colspan="1">Tareas, Plantillas de correo electrónico, Persona, Contacto, Campañas</td> 
   <td colspan="1">Insertar actualizaciones a SFDC y también eliminaciones</td> 
   <td colspan="1">Actualización, elemento fallido u omitido</td>
  </tr>  
  <tr> 
   <td colspan="1">Sincronizar esquema</td> 
   <td colspan="1">Miembros de campaña, Objetos personalizados, Campañas, Estado de miembro de campaña, Tareas, Persona, Oportunidad, Función de contacto de oportunidad, Usuarios</td> 
   <td colspan="1">Sincroniza metadatos para diferentes objetos, para decidir qué campos nuevos sincronizar en el siguiente ciclo</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Sincronizar con el programa</td> 
   <td colspan="1">Campañas</td> 
   <td colspan="1">Sincroniza el programa de Marketo con las campañas de SFDC</td> 
   <td colspan="1">Nuevo, Actualizaciones, Fallido u Omitido</td>
  </tr> 
  <tr> 
   <td colspan="1">Actualizar actividades</td> 
   <td colspan="1">Tareas</td> 
   <td colspan="1">Extraer actividades de Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Actualizar FKS</td> 
   <td colspan="1">Todos</td> 
   <td colspan="1">Actualizar la clave externa de todos los objetos</td> 
   <td colspan="1">N/A</td>
  </tr>  
 </tbody> 
</table>

&#42;La configuración de marca en el nivel de suscripción decide la etiqueta &quot;Posible cliente&quot; o &quot;Persona&quot; en el informe.
