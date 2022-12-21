---
unique-page-id: 7504051
description: 'Administrar datos de persona: documentos de Marketo: documentación del producto'
title: Administrar datos de personas
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 8%

---

# Administrar datos de personas {#manage-person-data}

Aproveche los datos de persona para la personalización web seleccionando campos de persona para utilizarlos en la segmentación.

1. Vaya a **Configuración de la cuenta**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Vaya a **Base de datos**.

   ![](assets/account-settings-dropdown-database.jpg)

## Adición de un nuevo campo de persona {#adding-a-new-person-field}

1. Select **Campo para agregar** en la lista desplegable para añadir un campo de datos de persona a la lista.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Se añade un nuevo campo en estado pendiente y puede tardar hasta 24 horas en activarse.

## Eliminación de un campo de persona {#deleting-a-person-field}

1. Haga clic en el icono Eliminar ( ![—](assets/image2015-3-24-13-3a45-3a56.png)) para quitar un campo de la lista. Haga clic en **Sí** para confirmar que desea eliminar el campo.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Administración de los campos de datos de persona**
   >
   >* Solo se pueden incluir los campos de datos de persona
   >* Puede agregar hasta 30 campos de datos de persona
   >* La adición de nuevos campos puede tardar hasta 24 horas en activarse
   >* La longitud máxima de los tipos de cadena es de 255 caracteres
   >* Los campos ocultos se eliminarán automáticamente


<table> 
 <tbody> 
  <tr> 
   <th><p>Nombre de la API de REST</p></th> 
   <th><p>Nombre de API SOAP</p></th> 
   <th><p>Nombre descriptivo</p></th> 
  </tr> 
  <tr> 
   <td><p>departamento</p></td> 
   <td><p>Departamento</p></td> 
   <td><p>Departamento</p></td> 
  </tr> 
  <tr> 
   <td><p>title</p></td> 
   <td><p>Título</p></td> 
   <td><p>Cargo</p></td> 
  </tr> 
  <tr> 
   <td><p>clasificación</p></td> 
   <td><p>Calificación</p></td> 
   <td><p>Calificación</p></td> 
  </tr> 
  <tr> 
   <td><p>leadScore</p></td> 
   <td><p>Puntuación de posible cliente</p></td> 
   <td><p>Puntuación</p></td> 
  </tr> 
  <tr> 
   <td><p>leadStatus</p></td> 
   <td><p>LeadStatus</p></td> 
   <td><p>Estado</p></td> 
  </tr> 
  <tr> 
   <td><p>prioridad</p></td> 
   <td><p>Prioridad</p></td> 
   <td><p>Prioridad</p></td> 
  </tr> 
  <tr> 
   <td><p>leadRole</p></td> 
   <td><p>Función de posible cliente</p></td> 
   <td><p>Rol</p></td> 
  </tr> 
  <tr> 
   <td><p>cancelar suscripción</p></td> 
   <td><p>Suscripción cancelada</p></td> 
   <td><p>Suscripción cancelada</p></td> 
  </tr> 
 </tbody> 
</table>

Los siguientes campos de posibles clientes se proporcionan predeterminados para las nuevas cuentas de Personalización web:

>[!MORELIKETHIS]
>
>[Crear un segmento utilizando datos de personas conocidas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
