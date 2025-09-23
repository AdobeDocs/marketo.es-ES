---
description: Sincronización de mensajes de clave de llamada y llamada - Documentos de Marketo - Documentación del producto
title: Sincronización de mensajes de clave de llamada y llamada
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 11%

---

# Sincronización de mensajes de clave de llamada y llamada {#syncing-call-and-call-key-messages}

Los objetos de mensajes de clave de llamada y llamada de [!DNL Veeva] CRM se sincronizan de manera predeterminada en Marketo Engage. Marketo sincroniza datos con una antigüedad de hasta 6 meses, en función de la fecha de creación de la llamada.

>[!NOTE]
>
>Marketo conserva los datos de la llamada hasta seis meses después de la fecha de la llamada.

**¿Cuáles son los déclencheur relacionados con el mensaje de clave de llamada y llamada?**

Desencadenadores:

* Añadido a la llamada
* Eliminado de la llamada
* Añadido al mensaje de clave de llamada
* Eliminado del mensaje de clave de llamada
* Llamada actualizada
* Mensaje de clave de llamada actualizado

Filtros:

* Tiene llamada
* Tiene mensaje de clave de llamada

Los siguientes campos de los mensajes Call y Call Key están sincronizados y pueden utilizarse como restricciones y déclencheur.

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
        Etiqueta del campo
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
      <td>Llamar</td>
      <td>Contable</td>
      <td>Busque la cuenta a la que está asociada la llamada.</td>
      <td>Account_vod__c</td>
      <td>Búsqueda (cuenta)</td>
    </tr>
    <tr>
      <td>Llamar</td>
      <td>Tipo de llamada</td>
      <td>Tipo de llamada que el sistema mantiene en función del tipo y el contenido de la llamada. Este campo se utiliza con fines de creación de informes. Los valores válidos son: Detail Only, Detail with Sample, Group Detail, Group Detail with Sample, Sample Only. Estos valores no deben cambiarse, pero las traducciones de estas listas de selección pueden cambiar. Los asistentes tienen el mismo tipo de llamada que la llamada de encabezado. Para una llamada de grupo con 3 profesionales, los 4 registros tienen el tipo de llamada "Detalle del grupo"</td>
      <td>Call_Type_vod__c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
     <td>Llamar</td>
      <td>Contacto</td>
      <td>Busque el contacto (si lo hay) al que está asociada la llamada.</td>
      <td>Contact_vod__c</td>
      <td>Búsqueda (contacto)</td>
    </tr>
    <tr>
      <td>Llamar</td>
      <td>Fecha</td>
      <td>La fecha de la llamada en la que se guardó o envió por primera vez. Este campo se establece mediante un déclencheur en la fecha actual si no se proporciona ninguno de los campos fecha y hora.</td>
      <td>Call_Date_vod__c</td>
      <td>Fecha</td>
    </tr>
    <tr>
      <td>Llamar</td>
      <td>¿Es la llamada del padre?</td>
      <td>Campo de fórmula para determinar si el registro de llamada es el registro de llamada principal o de llamada de asistente. 1 indica que el registro es la llamada principal. 0 indica que se trata de una llamada de asistente.</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>Fórmula (número)</td>
    </tr>
    <tr>
      <td>Llamar</td>
      <td>Estado</td>
      <td>Estado de la llamada: Planificada, guardada o enviada. Utilice el área de trabajo de traducción para cambiar los valores de visualización. Los déclencheur de la llamada consultan este campo para ver si la llamada está bloqueada (enviada). Este valor se establece para el usuario cuando se pulsa el botón Guardar o Enviar.</td>
      <td>Status_vod__c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
      <td>Llamar</td>
      <td>Tipo de registro</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Tipo de registro</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Llamar</td>
      <td>Busca la llamada. Cada mensaje clave está asociado a una llamada.</td>
      <td>Llamar a 2_vod__c</td>
      <td>Master-Detail(Call)</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Categoría</td>
      <td>Registra la categoría del mensaje. Se utiliza principalmente para informes.</td>
      <td>Category_vod__c</td>
      <td>Lista de selección</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Nombre de presentación CLM</td>
      <td>Nombre de presentación CLM estampado</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Nombre del mensaje de clave</td>
      <td>Nombre de mensaje de clave estampada</td>
      <td>Key_Message_Name_vod__c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Nombre del producto</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Fórmula (texto)</td>
    </tr>
    <tr>
      <td>Mensaje clave de llamada</td>
      <td>Reacción</a>
      </td>
      <td>Lista de reproducción del mensaje. Edite la lista de selección para cambiar los valores de reacción.</td>
      <td>Reaction_vod__c</td>
      <td>Lista de selección</td>
    </tr>
  </tbody>
</table>
