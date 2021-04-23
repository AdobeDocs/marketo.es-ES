---
unique-page-id: 11379928
description: Detalles del cambio en pista de auditoría - Documentos de Marketo - Documentación del producto
title: Cambiar detalles en pista de auditoría
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1913'
ht-degree: 0%

---

# Cambiar detalles en pista de auditoría {#change-details-in-audit-trail}

La pista de auditoría ofrece una buena cantidad de información sobre quién está haciendo qué en su suscripción a Marketo. Aquí están los detalles.

## Pista de auditoría de activos {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Recurso/Tipo</th> 
   <th colspan="1">Acción</th> 
   <th colspan="1">Detalles del cambio</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>Programa predeterminado</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Crear</td> 
   <td>Tipo de canal "tipo de canal"<br>o<br>Clonado desde "nombre de programa"</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en el espacio de trabajo "nombre del espacio de trabajo" <br>Ubicación "carpeta de campaña" o "programa de participación" <br>Nombre del programa clonado "nuevo nombre"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Editar canal</td> 
   <td>Nuevo canal "nuevo nombre de canal" Canal antiguo "nombre de canal antiguo" </td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Agregue el valor "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Editar token "token name" nuevo valor "new value" antiguo valor "old value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Eliminar token "nombre de token"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Añadir "nombre de comportamiento" de comportamiento de Analytics</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td><p>Editar el comportamiento de Analytics "nombre de comportamiento"</p><p>Comportamiento antiguo "nombre de comportamiento"</p></td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Eliminar el comportamiento de Analytics "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Agregar valor de costo de período "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Editar coste de período Nuevo valor de coste "#", Nuevo mes de programa "aaaa-mm", Valor de coste antiguo "#", Mes de programa antiguo "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Eliminar coste del periodo. Valor "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>Correo electrónico</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Crear</td> 
   <td>Creado con la plantilla "nombre de plantilla" <br>o <br>Clonado desde "nombre de recurso"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha actualizado "De nombre" a "nuevo de nombre"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha actualizado "De correo electrónico" a "newemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha actualizado "Responder a" a "newreplytoemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha actualizado "Asunto" a "nueva línea de asunto"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha añadido la segmentación "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Segmentación eliminada</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha añadido el fragmento "snippet_name"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha eliminado un fragmento</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Edita el correo electrónico roto de la plantilla "template_name" (NOTA: esto sucede hoy si edita el código directamente)</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Descripción nueva "descripción nueva" Descripción antigua "descripción antigua"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Editar módulo <code>"<module name>" <attribute></code> a "value"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "Estudio de diseño" en la carpeta "nombre de carpeta" <br>Nombre de recurso clonado "nombre"<br>o<br>Clonado para "Actividades de marketing" en el programa "nombre de programa"<br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Mover</td> 
   <td>Se ha movido a "Design studio" a la carpeta "nombre de carpeta"<br>o<br>Se ha movido a "actividades de marketing" al programa "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Borrador</td> 
   <td>Se redactó el correo electrónico porque se aprobó el fragmento "nombre de fragmento"<br>o<br>Correo electrónico porque se aprobó la plantilla "nombre de plantilla"</td> 
  </tr> 
   <td rowspan="17">Programa de correo electrónico</td> 
   <td>Crear</td> 
   <td>Tipo de canal "tipo de canal"<br>o<br>Clonado desde "nombre de programa"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Cambiar nombre</td> 
   <td colspan="1">Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en el espacio de trabajo "nombre del espacio de trabajo" <br>Ubicación "Carpeta de campaña o programa de participación" <br>Nombre del programa clonado "nuevo nombre"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Anular</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Editar canal</td> 
   <td>Canal nuevo "canal nuevo" Canal antiguo "canal antiguo"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Agregue el valor "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Editar token "token name" Nuevo valor "new value" antiguo valor "old value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Eliminar token "nombre de token"</td> 
  </tr> 
  <tr> 
   <td>Modificación de la programación</td> 
   <td>Establezca la programación para que comience en "fecha de inicio, hora de inicio" y termine en "fecha de finalización, hora de finalización".</td> 
  </tr> 
  <tr> 
   <td>Modificación de la programación</td> 
   <td>Se ha cambiado la programación a "nueva fecha, nueva hora".</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Añadir "nombre de comportamiento" de comportamiento de Analytics</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Editar el comportamiento de Analytics "nombre de comportamiento"<br>El antiguo comportamiento "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Eliminar el comportamiento de Analytics "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Agregar valor de costo de período "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Editar coste de período Nuevo valor de coste "#", Nuevo mes de programa "aaaa-mm", Valor de coste antiguo "#", Mes de programa antiguo "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Eliminar coste del periodo. Valor "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Plantilla de correo electrónico</td> 
   <td>Crear</td> 
   <td>En blanco o clonado desde "nombre de plantilla"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Descripción nueva "descripción nueva", descripción anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>HTML editado</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "nombre de carpeta" <br> Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="23">Programa de participación</td> 
   <td>Crear</td> 
   <td>Tipo de canal "tipo de canal"<br> o<br> Clonado desde "nombre de programa"</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en el espacio de trabajo "nombre del espacio de trabajo" <br>Ubicación "Carpeta de campaña o programa de participación" <br>Nombre del programa clonado "nuevo nombre"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Editar canal</td> 
   <td>Canal nuevo "canal nuevo" Canal antiguo "canal antiguo"</td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td><p>Agregar flujo</p><p>Nombre "name" Colocación "#"</p></td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td><p>Editar flujo</p><p>Nombre de la nueva emisión: "nuevo nombre" Nombre de flujo antiguo: "nombre antiguo"</p><p>Nueva ubicación: Colocación antigua "new #" (nuevo #): "old #"</p></td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td>Eliminar nombre de flujo "name"</td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td>Añada contenido<br>Nombre de flujo "nombre de flujo"<br>Escriba "Correo electrónico" o "Programa"<br>Nombre "nombre de correo electrónico" o "nombre de programa"<br>Nombre de campaña inteligente</td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td>Activar contenido<br>Nombre del flujo "nombre del flujo"<br>Nombre del contenido "nombre del correo electrónico" o "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td>Desactivar contenido<br>Nombre del flujo "nombre del flujo"<br>Nombre del contenido "nombre del correo electrónico" o "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Modificación del flujo del programa</td> 
   <td>Eliminar contenido<br>Nombre del flujo "nombre del flujo"<br>Nombre del contenido "nombre del correo electrónico" o "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Agregue el valor "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Editar token "token name" Nuevo valor "new value" antiguo valor "old value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Eliminar token "nombre de token"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Añadir "nombre de comportamiento" de comportamiento de Analytics</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Editar el comportamiento de Analytics "nombre de comportamiento"<br>El antiguo comportamiento "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Eliminar el comportamiento de Analytics "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Cambiar el estado del programa. Nuevo valor "on/off" Valor antiguo "off/on"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Agregar valor de costo de período "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Editar coste de período Nuevo valor de coste "#", Nuevo mes de programa "aaaa-mm", Valor de coste antiguo "#", Mes de programa antiguo "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Eliminar coste del periodo. Valor "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="18">Programa de eventos</td> 
   <td>Crear</td> 
   <td>Tipo de canal "tipo de canal"<br>o<br>Clonado desde "nombre de programa"</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en el espacio de trabajo "nombre del espacio de trabajo" <br>Ubicación "carpeta de campaña" o "programa de participación" <br>Nombre del programa clonado "nuevo nombre"</td> 
  </tr> 
  <tr> 
   <td>Editar canal</td> 
   <td>Canal nuevo "canal nuevo" Canal antiguo "canal antiguo" </td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Agregue el valor "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Editar token "token name" Nuevo valor "new value" antiguo valor "old value"</td> 
  </tr> 
  <tr> 
   <td>Modificar token del programa</td> 
   <td>Eliminar token "nombre de token"</td> 
  </tr> 
  <tr> 
   <td>Modificación de la programación</td> 
   <td>Establezca la programación para que comience en "fecha de inicio, hora de inicio" y termine en "fecha de finalización, hora de finalización".</td> 
  </tr> 
  <tr> 
   <td>Modificación de la programación</td> 
   <td>Se ha cambiado la programación a "nueva fecha, nueva hora".</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Añadir "nombre de comportamiento" de comportamiento de Analytics</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Editar el comportamiento de Analytics "nombre de comportamiento"<br>El antiguo comportamiento "nombre de comportamiento"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración del programa</td> 
   <td>Eliminar "nombre de comportamiento" del comportamiento de Analytics</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Agregar valor de costo de período "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Editar coste de período Nuevo valor de coste "#", Nuevo mes de programa "aaaa-mm", Valor de coste antiguo "#", Mes de programa antiguo "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Eliminar coste del periodo. Valor "#" mes del programa "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modificar la configuración del programa</td> 
   <td colspan="1">Se ha añadido el asociado de eventos "partner_name"</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Carpetas</td> 
   <td>Crear</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha agregado el token "token_name", valor "value"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Token modificado "token_name" nuevo valor "token_value" antiguo valor "old_token_value"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Token eliminado "token_name"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Forms</td> 
   <td>Crear</td> 
   <td>Muy pronto. Más información o Clonado desde "nombre de formulario"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Descripción nueva "descripción nueva" Descripción antigua "descripción antigua"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Configuración de formulario editada </td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Detalles del campo editado</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "Estudio de diseño" en la carpeta "nombre de carpeta" <br>Nombre de recurso clonado "nombre"<br>o<br>Clonado para "Actividades de marketing" en el programa "nombre de programa"<br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Mover</td> 
   <td>Se ha movido a "Design studio" a la carpeta "nombre de carpeta"<br>o<br>Se ha movido a "actividades de marketing" al programa "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>Aprobar</td> 
   <td>Utilizado por # assets </td> 
  </tr> 
  <tr> 
   <td rowspan="9">Página de aterrizaje</td> 
   <td>Crear</td> 
   <td>Creado con la plantilla "nombre de plantilla" <br>o <br>Clonado desde "nombre de recurso"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Nueva descripción "descripción nueva" Anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha añadido "Imagen", Se ha eliminado "Imagen", Se ha editado el componente de imagen</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha agregado "Texto enriquecido", Se ha eliminado "Texto enriquecido", Se ha editado el componente Texto enriquecido</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en "Estudio de diseño" en la carpeta "nombre de carpeta"<br>Nombre de recurso clonado "nombre"<br>URL de recurso clonado "www.url.com"<br>o<br>Clonado para "Actividades de marketing" en el programa "nombre de programa" <br>Nombre de recurso clonado "nombre"<br>URL de recurso clonado "www.url.com"</td> 
  </tr> 
  <tr> 
   <td>Mover</td> 
   <td>Se ha movido a "Design studio" a la carpeta "nombre de carpeta"<br> o<br> Se ha movido a "actividades de marketing" al programa "nombre del programa"</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Borrador</td> 
   <td>La página de aterrizaje se redactó porque se aprobó la plantilla "nombre de plantilla"</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Plantilla de página de aterrizaje</td> 
   <td>Crear</td> 
   <td><p>Vacío<br>o<br>Clonado desde "nombre de recurso"</p></td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Descripción nueva "descripción nueva" descripción anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "nombre de carpeta" <br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>Utilizado por # assets </td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Lista (estática)</td> 
   <td>Crear</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "Base de datos de personas" en la carpeta "nombre de carpeta" <br>Nombre de recurso clonado "nombre"<br>o<br>Clonado para "Actividades de marketing" en el programa "nombre de programa"<br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td rowspan="12">Campaña inteligente</td> 
   <td>Crear</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Activar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Desactivar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Anular</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Mover</td> 
   <td>Se ha movido a "Programas" en el programa "nombre de programa"<br>o<br>Se ha movido a "Carpetas" en la carpeta "nombre de carpeta"</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Nueva descripción "descripción nueva" Anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado en "Programas" en el programa "nombre de programa" <br>Nombre de recurso clonado "nombre"<br>o<br>Clonado en "Carpeta" en la carpeta "nombre de carpeta"<br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración de listas inteligentes</td> 
   <td>Muestra una instantánea del estado actual, incluidos los nombres y valores de filtros y déclencheur</td> 
  </tr> 
  <tr> 
   <td>Modificación de la programación de campañas</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modificación de la acción del paso de flujo</td> 
   <td>Muestra una instantánea del estado actual, incluidos los nombres y valores de cada paso de flujo</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Lista inteligente</td> 
   <td>Crear</td> 
   <td>Clonado desde "nombre de lista inteligente"</td> 
  </tr> 
  <tr> 
   <td>Exportar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Nueva descripción "descripción nueva" Anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "Base de datos de personas" en la carpeta "nombre de carpeta" <br>Nombre de recurso clonado "nombre"<br>o<br>Clonado para "Actividades de marketing" en el programa "nombre de programa" <br>Nombre de recurso clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Modificar la configuración de listas inteligentes</td> 
   <td>Muestra una instantánea del estado actual, incluidos los nombres y valores de filtros y déclencheur </td> 
  </tr> 
  <tr> 
   <td rowspan="11">Fragmento</td> 
   <td>Crear</td> 
   <td><p>Vacío<br>o<br>Clonado a partir de "nombre de fragmento"</p></td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha añadido la segmentación "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Segmentación eliminada</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Editado</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre</td> 
   <td>Nuevo nombre "nuevo nombre", nombre anterior "nombre anterior"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Nueva descripción "descripción nueva" Anterior "descripción anterior"</td> 
  </tr> 
  <tr> 
   <td>Clonar</td> 
   <td>Clonado para "nombre de carpeta" <br>Nombre de fragmento clonado "nombre"</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td>Utilizado por # assets</td> 
  </tr> 
  <tr> 
   <td>Aprobar sin borrador</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Aprobar</td> 
   <td><p>N/D</p></td> 
  </tr> 
 </tbody> 
</table>

## Pista de auditoría del administrador {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Área de administración</th> 
   <th>Acción</th> 
   <th>Detalles del cambio</th> 
  </tr> 
  <tr> 
   <td>Restricciones de IP</td> 
   <td>Editar</td> 
   <td>Se han editado las restricciones de IP a lo siguiente: "bloque" permitido/bloqueado, dirección IP "#", restricciones IP deshabilitadas ""</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Partición</td> 
   <td>Crear</td> 
   <td>Partición creada con el nombre "nombre de partición"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>partición "nombre de partición" eliminada</td> 
  </tr> 
  <tr> 
   <td>Seguridad de la contraseña</td> 
   <td>Editar</td> 
   <td>La seguridad de la contraseña cambió a la plantilla: Seguridad estándar, longitud mínima: #, parte inferior superior: #, número: #, mayúsculas y minúsculas mezcladas: # , caducidad : #, tiempo de espera de sesión: #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">Función<br><br></td> 
   <td>Crear</td> 
   <td>Función creada con "nombre de función" (NOTA: si necesita detalles sobre permisos agregados, póngase en contacto con el servicio de asistencia técnica): <br>muestra una instantánea de los permisos asignados a la función</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>Se eliminó la función "Nombre de función"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Función editada de "nombre anterior" a "nuevo nombre" (NOTA: si necesita detalles sobre permisos editados, póngase en contacto con el servicio de asistencia técnica): <br>muestra una instantánea de los permisos asignados a la función<br></td> 
  </tr> 
  <tr> 
   <td>Informe de lista inteligente</td> 
   <td>Editar</td> 
   <td>Se editó SmarList para iniciar sesión y descargarla: "true o false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Usuario<br><br><br><br></td> 
   <td>Crear (invitar)</td> 
   <td>Usuario invitado con: Correo electrónico "dirección de correo electrónico", Nombre "nombre y apellido", Acceso caduca "en blanco o con una fecha", Usuario de API "true o false" - <br>muestra una instantánea de las funciones y los espacios de trabajo asignados al usuario</td> 
  </tr> 
  <tr> 
   <td colspan="1">Eliminar</td> 
   <td colspan="1">usuario "nombre de usuario" eliminado</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>Se ha cambiado el nombre del usuario de "nombre antiguo" a "nuevo nombre" por correo electrónico: "email", apiUser: El acceso "true o false" caduca: "en blanco o con fecha"</td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>El usuario se ha editado para el correo electrónico: "email", apiUser: "true o false", el acceso caduca: "en blanco o con fecha"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Editar</td> 
   <td colspan="1">Muestra una instantánea del estado actual, incluidas las funciones y los espacios de trabajo asignados al usuario</td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Licencia de calendario emitida por correo electrónico: nombre del "correo electrónico del usuario": "nombre del usuario"</td> 
  </tr> 
  <tr> 
   <td>Restablecer</td> 
   <td>Restablecimiento de contraseña para el nombre "nombre" y el correo electrónico "correo electrónico"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Espacio de trabajo</td> 
   <td>Crear</td> 
   <td>Espacio de trabajo creado con el nombre "nombre del espacio de trabajo"</td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>"nombre de espacio de trabajo" espacio de trabajo eliminado</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Filtrado en pista de auditoría](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
