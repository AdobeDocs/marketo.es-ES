---
description: Sincronización de mensajes clave de llamada y llamada - Documentos de Marketo - Documentación del producto
title: Sincronización de mensajes clave de llamada y de llamada
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# Sincronización de mensajes clave de llamada y de llamada {#syncing-call-and-call-key-messages}

Los objetos de mensaje clave de llamada y llamada de en Veva CRM se sincronizan de forma predeterminada en Marketo Engage. Marketo sincroniza datos que tienen hasta 6 meses de antigüedad, según la fecha de la llamada.

>[!NOTE]
>
>Marketo retiene los datos de llamadas hasta seis meses a partir de la fecha de la llamada.

**¿Cuáles son los déclencheur o filtros relacionados con los mensajes de clave de llamada y de llamada?**

Desencadenadores:

* Se ha añadido a la llamada
* Eliminada de la llamada
* Se ha agregado al mensaje de clave de llamada
* Eliminado del mensaje de clave de llamada
* Llamada actualizada
* Mensaje de clave de llamada actualizado

Filtros:

* Tiene llamada
* Tiene mensaje clave de llamada

Los campos siguientes de los mensajes de llamada y clave de llamada se sincronizan y se pueden utilizar como restricciones y déclencheur.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Objeto
      </th>
      <th>
        Etiqueta de campo
      </th>
      <th>
        Descripción
      </th>
      <th>
        Nombre del campo
      </th>
      <th>
        Tipo de datos
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>La llamada</td>
      <td>Contador</td>
      <td>Busque la cuenta a la que está asociada la llamada.</td>
      <td>Account_vod_c</td>
      <td>Búsqueda (cuenta)</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>Tipo de llamada</td>
      <td>Tipo de llamada que se mantiene en el sistema según el tipo y el contenido de la llamada. Este campo se utiliza para generar informes. Los valores válidos son: Detalle solamente, Detalle con muestra, Detalle del grupo, Detalle del grupo con muestra, Solo muestra. Estos valores no deben cambiarse, pero las traducciones de estas listas de selección pueden modificarse. Los asistentes tienen el mismo tipo de llamada que la llamada de encabezado. Para una llamada de grupo con 3 profesionales, los 4 registros tienen el tipo de llamada "Detalle de grupo"</td>
      <td>Call_Type_vod_c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
     <td>La llamada</td>
      <td>Contacto</td>
      <td>Busque el contacto (si lo hay) al que está asociada la llamada.</td>
      <td>Contact_vod_c</td>
      <td>Lookup(Contact)</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>Fecha</td>
      <td>La fecha de la llamada cuando se guardó o envió por primera vez. Este campo se configura mediante un déclencheur a la fecha actual si no se proporciona el campo de fecha y hora.</td>
      <td>Call_Date_vod_c</td>
      <td>Fecha</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>Productos detallados</td>
      <td>Campo de ayuda para mostrar la lista de productos detallados para una llamada de . Los nombres de producto deben delimitarse con espacios dobles y orden de prioridad de izquierda a derecha. Este campo no controla el procesamiento y se incluye para que las listas e informes relacionados sean más fáciles de usar.</td>
      <td>Detailed_Products_vod_c</td>
      <td>Área de texto (255)</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>¿Es la llamada principal?</td>
      <td>Campo de fórmula para determinar si el registro de llamada es la llamada principal o un registro de llamada de asistente. 1 indica que el registro es la llamada principal. 0 indica que es una llamada de asistente.</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>Fórmula (número)</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>Estado</td>
      <td>Estado de la llamada — Planificada, guardada o enviada. Utilice el área de trabajo de traducción para cambiar los valores de visualización. Los déclencheur de la llamada miran este campo para ver si la llamada está bloqueada (enviada). Este valor se define para el usuario cuando se pulsa el botón Guardar o Enviar.</td>
      <td>Status_vod_c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
      <td>La llamada</td>
      <td>Tipo de registro</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Tipo de registro</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>La llamada</td>
      <td>Busque la llamada . Cada mensaje clave está asociado con una llamada a .</td>
      <td>Call2_vod_c</td>
      <td>Master-Detail(Call)</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>Categoría</td>
      <td>Registra la categoría del mensaje. Se utiliza principalmente para la creación de informes.</td>
      <td>Category_vod_c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>Nombre de presentación CLM</td>
      <td>Nombre de presentación de CLM marcado</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>Nombre del mensaje clave</td>
      <td>Nombre del mensaje clave marcado</td>
      <td>Key_Message_Name_vod__c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>Nombre del producto</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Fórmula (texto)</td>
    </tr>
    <tr>
      <td>Mensaje de clave de llamada</td>
      <td>Reacción</a>
      </td>
      <td>Lista de reacciones al mensaje. Edite la lista de selección para cambiar los valores de reacción.</td>
      <td>Reaction_vod_c</td>
      <td>Lista de selección</td>
    </tr>
  </tbody>
</table>
