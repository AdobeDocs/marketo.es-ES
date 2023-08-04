---
description: Heredar documento 1 - Documentos de Marketo - Documentación del producto
title: Heredar documento 1
hide: true
hidefromtoc: true
source-git-commit: b06d1d0f8101895ebefeb821150090aac3044870
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 5%

---

# Heredar documento 1 {#inherit-doc-1}

La auditoría de una instancia heredada puede parecer un...

¿Heredó una instancia de Marketo Engage existente de otro administrador? Si es así, este artículo es para usted...

La lista de comprobación siguiente se ha combinado con los datos de Marketo Champions para ayudarle a ponerse al día rápidamente en su instancia heredada...

>[!TIP]
>
>Si es un usuario Marketo Engage nuevo y no está familiarizado con muchos de los términos, consulte la [Glosario de Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Usuarios y funciones {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Cuántos usuarios</a> ¿hay?</li>
<li>¿Hay algún usuario que debería haber caducado?</li>
<li>¿Su compañía tiene directivas para eliminar usuarios?</li> 
<li>Cuántos usuarios tienen <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Permisos de administración</a>?</li>
<li>Si alguno de estos usuarios se cambia a <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">¿otros roles?</a></li> 
<li>¿Quiénes son los usuarios de API en esta instancia?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Funciones</td> 
   <td><li>¿Cuántos roles hay?</li>  
<li>Qué <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permisos/acceso</a> ¿tiene cada función? ¿Se debe realizar algún ajuste?</li>
<li>¿Cuántos usuarios hay por función?</li>
<li>La frecuencia con la que los usuarios <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">iniciar sesión</a>?</li>
<li>¿Cada usuario de API tiene su <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">función de usuario propio</a>? Si no es así, considere implementar esto para facilitar la resolución de problemas.</li> 
<li>¿Las funciones de usuario y los permisos se alinean con los datos corporativos? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">políticas de privacidad</a>?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Los usuarios y las funciones están claramente definidos en su organización?</li>
<li>¿Cuál es su proceso para agregar un nuevo usuario/administrador?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Zona protegida (si corresponde)</td> 
   <td><li>¿Tiene un <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instancia de zona protegida</a>? Si es así, revise las categorías anteriores para su zona protegida.</li>
<li>Es <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importación de programas</a> ¿está vinculado con su zona protegida?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Pista de auditoría {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Pista de auditoría</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Quién está trabajando</a> en la instancia?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Espacios de trabajo y particiones {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Espacios de trabajo y particiones</td> 
   <td><li>¿Cuántos espacios de trabajo y/o particiones tiene?</li>
<li>¿Cuál es el propósito principal de cada espacio de trabajo y partición?</li>
<li>¿Es necesario auditarlas o cambiarlas?</li>
<li>¿Cuál es la relación entre sus espacios de trabajo y las particiones?</li>
<li>¿Cuántos usuarios tienen acceso a cada espacio de trabajo?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Cómo se definen los espacios de trabajo y las particiones?</li>
<li>¿Cuál es el proceso para añadir espacios de trabajo a la instancia o añadir usuarios a un espacio de trabajo?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Campañas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Configuración de campañas inteligentes</td> 
   <td><li>¿Tiene restricciones en el tamaño de la campaña inteligente?</li>
<li>Si no es así, considere la posibilidad de agregar uno. Se recomienda limitar los límites de las campañas inteligentes al 25 % de la base de datos para evitar una comunicación excesiva o procesar toda la base de datos en flujos de trabajo, esto no solo protege la marca, sino que ayuda a proteger el rendimiento de la instancia.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Límites de comunicación {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Límites de comunicación</td> 
   <td><li>¿Existen límites? ¿Su empresa tiene políticas en las que podrían ser necesarios límites de comunicación?</li>
<li>El Adobe recomienda limitar la comunicación a 1 por día y a 3 por 7 días, con correos electrónicos no operativos bloqueados.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Etiquetas {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Etiquetas</td> 
   <td><li>¿Cuántas etiquetas hay? ¿Cuántas etiquetas se están utilizando? ¿Es necesario añadir alguna?</li>
<li>¿Se requieren etiquetas dentro de los programas?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Canales</td> 
   <td><li>¿Cuántos canales hay? ¿Cuántos están en uso?</li>
<li>¿Son apropiados todos los estados de programas de canal? ¿Muestran progresión dentro del programa?</li>
<li>¿Sus canales están relacionados con tipos de programas específicos?</li>
<li>¿Qué estados se consideran un éxito para cada canal? ¿Se alinean con sus objetivos de marketing?</li>
<li>¿Se está utilizando correctamente el canal operativo?</li>
<li>En el caso del Report Builder avanzado (Explorador del ciclo de ingresos\RCE), ¿está configurado el comportamiento de análisis de canal para que se ajuste a las prácticas del programa que incorporan el coste del período?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Calendario de marketing (si corresponde)</td> 
   <td><li>¿Cuántos tipos de entradas de calendario hay? ¿Siguen siendo relevantes?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Administración de bases de datos {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Administración de campos</td> 
   <td><li>¿Cuántos campos hay? Haga clic en "Exportar nombres de campo" para revisar una lista de sus campos, campos personalizados y sus nombres de API.</li>
<li>¿Cuántos campos personalizados hay?</li>
<li>¿Cuántos campos se están utilizando? Seleccione "Exportar usados por" en la lista desplegable Acciones de campo para revisar los recursos relacionados de un campo.</li>
<li>¿Cuántos se sincronizan entre Marketo Engage y su CRM?</li>
<li>¿Los campos de CRM están sincronizados con los objetos adecuados?</li>
<li>¿Hay alguna vista personalizada configurada para los detalles de la persona? ¿Debería haber?</li>
<li>¿Tiene una convención de nombres para los campos basada en el origen? Si no es así, considere implementar esto.</li>
<li>¿Hay algún campo bloqueado? Asegúrese de comprender por qué lo son.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Actividades personalizadas</td> 
   <td><li>¿Hay alguna actividad personalizada?</li>
<li>Si es así, haga clic en ellas para comprender qué actividades no están relacionadas con un formulario, un correo electrónico o una página de aterrizaje de Marketo.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td> objetos personalizados de </td> 
   <td><li>¿Cuántos objetos personalizados hay? ¿Cómo se sincronizan con su CRM?</li>
<li>¿Cómo utilizan sus programas y consultas de lista estos objetos personalizados?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integraciones {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>¿A qué CRM se está sincronizando? Salesforce? MS Dynamics? Veeva?</li>
<li>¿Es la sincronización personalizada o bidireccional? (KG: CORREGIR LA GRAMÁTICA Y COMPROBAR LA IMPORTANCIA)</li>
<li>[Solo Salesforce] ¿Su instancia tiene implementados los filtros de sincronización personalizados? Póngase en contacto con el Soporte técnico de Marketo para identificar los filtros de sincronización personalizados o solicitar que se implemente una regla de sincronización personalizada.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Páginas de destino</td> 
   <td><li>¿Cuál es el dominio establecido como?</li>
<li>¿Cómo se establece la reserva?</li>
<li>¿Cómo se establece la página principal?</li>
<li>¿Está habilitado el rellenado previo del formulario?</li>
<li>¿Las direcciones URL personalizadas están habilitadas?</li>
<li>¿Hay reglas configuradas para las redirecciones?</li>
<li>¿Tiene alias de dominio establecidos? ¿Está realizando un seguimiento a través de la documentación de cómo utiliza los alias de dominio?</li>
<li>¿Están activados los dominios seguros para las páginas de aterrizaje? Confirme si los recursos de la página de aterrizaje contienen una dirección URL "http".</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>¿Su código de seguimiento de Munchkin está en su sitio web (no en Marketo)?</li>
<li>¿Está habilitada una solicitud de explorador "No rastrear"?</li>
<li>¿Está configurada la API de Munchkin? Si le falta documentación sobre dónde está el código Munchkin en su sitio web, comience con una vista rápida utilizando el "Informe de análisis web" en "Analytics" básico para comprender dónde se coloca el código Munchkin en su sitio web.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Servicios web</td> 
   <td><li>¿Están habilitadas las restricciones de IP? ¿Deberían estarlo?</li>
<li>¿Qué usuarios/aplicaciones realizan llamadas de API en su instancia?</li>
<li>¿Está alcanzando o cerca de alcanzar su límite de API? Si es así, considere la posibilidad de aumentarla o auditar su instancia para desactivar esas llamadas de API.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Perspectiva de ventas de Marketo (si corresponde)</td> 
   <td><li>Tiene el <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Se ha instalado el paquete MSI</a>?</li>
<li>¿Tiene usted <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">actualizado a la última versión de Sales Insight</a>?</li>
<li>¿Ha completado la configuración de Sales Insight? Usuarios empresariales/ilimitados <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">haga clic aquí</a>, Usuarios profesionales <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">haga clic aquí</a>.</li>
<li>¿Tiene usted <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">acceso dado a los usuarios</a> ¿en función del número de puestos que has comprado?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Punto de inicio (si corresponde)</td> 
   <td><li>¿Qué servicios tiene configurados (seminario web, publicidad, etc.)? ¿Están a punto de expirar?</li>
<li>¿Cuántas llamadas de API utilizan sus integraciones de?</li>
<li>¿Tiene las integraciones adecuadas para sus casos de uso?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Webhooks (si procede)</td> 
   <td><li>¿Qué conexiones ha configurado?</li>
<li>¿Ya no se utiliza alguno?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Aplicaciones móviles (si corresponde)</td> 
   <td><li>¿Qué aplicaciones móviles tiene?</li>
<li>¿Qué dispositivos de prueba se han agregado?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Cofre del tesoro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Cofre del tesoro</td> 
   <td><li>¿Qué hay en el cofre del tesoro?</li>
<li>¿Hay funciones que se deben activar o desactivar?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Inspector de campaña</td> 
   <td><li>¿Está activado el Inspector de campaña?</li>
<li>Si no es así, puede activarla para identificar fácilmente qué campañas están activas, sincronizarlas con su CRM o eliminar registros.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Varios {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Actualizaciones de estado del Marketo Engage</td> 
   <td><li>¿Su instancia está suscrita a las actualizaciones de estado del Marketo Engage?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Contactos autorizados</td> 
   <td><li>¿Ha configurado los contactos autorizados adecuados en el Portal de asistencia?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Alertas</td> 
   <td><li>¿Hay alguna alerta activa que se esté enviando a equipos internos desde Marketo Engage?</li>
<li>En caso afirmativo, ¿funcionan correctamente esas alertas?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Notificaciones</td> 
   <td><li>¿Está suscrito a las notificaciones de administración correspondientes?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
