---
unique-page-id: 7504051
description: Obtenga información acerca de la administración de datos de personas en Marketo Engage, incluido el administrador de datos de personas. Utilice esta guía para completar el siguiente paso.
title: Administrar datos de personas
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
TQID: https://experienceleague.adobe.com/rIiC-JXLkaMByk7GizVOcCEcUHN8AL-8Hy66-U2GZhs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 15%

---

# Administrar datos de personas {#manage-person-data}

Aproveche los datos de la persona de [!DNL Web Personalization] seleccionando campos de persona para usarlos en la segmentación.

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Ir a **[!UICONTROL Base de datos]**.

   ![](assets/account-settings-dropdown-database.jpg)

## Adición de un campo de nueva persona {#adding-a-new-person-field}

1. Seleccione **Campo para agregar** de la lista desplegable para agregar un campo de datos de persona a la lista.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Se agrega un nuevo campo en un estado pendiente que puede tardar hasta 24 horas en activarse.

## Eliminación de un campo de persona {#deleting-a-person-field}

1. Haga clic en el icono Eliminar ( ![—](assets/image2015-3-24-13-3a45-3a56.png)) para quitar un campo de la lista. Haga clic en **[!UICONTROL Sí]** para confirmar que desea eliminar el campo.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Administrar los campos de datos de persona**
   >
   >* Solo se pueden incluir campos de datos de persona
   >* Se pueden añadir hasta 30 campos de datos de persona
   >* Añadir campos nuevos puede tardar hasta 24 horas en activarse
   >* La longitud máxima de los tipos de cadena es de 255 caracteres
   >* Los campos ocultos se eliminarán automáticamente

<table>
 <tbody>
  <tr>
   <th><p>Nombre de REST API</p></th>
   <th><p>Nombre de SOAP API</p></th>
   <th><p>Nombre descriptivo</p></th>
  </tr>
  <tr>
   <td><p>departamento</p></td>
   <td><p>Departamento</p></td>
   <td><p>Departamento</p></td>
  </tr>
  <tr>
   <td><p>título</p></td>
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
   <td><p>LeadScore</p></td>
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
   <td><p>LeadRole</p></td>
   <td><p>Función</p></td>
  </tr>
  <tr>
   <td><p>cancelado</p></td>
   <td><p>Suscripción cancelada</p></td>
   <td><p>Suscripción cancelada</p></td>
  </tr>
 </tbody>
</table>

Los siguientes campos de posibles clientes se proporcionan de forma predeterminada para las nuevas cuentas de [!DNL Web Personalization]:

>[!MORELIKETHIS]
>
>[Crear un segmento con datos de persona conocida](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
