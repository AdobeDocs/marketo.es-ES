---
description: Administración de usuarios y licencias - Documentos de Marketo - Documentación del producto
title: Administración de usuarios y licencias
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: c7479355c7f5fda97ce6ad0f18a5c3c6a597e535
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Administración de usuarios y licencias {#user-and-license-management}

Aprenda a añadir y eliminar usuarios, así como a ver sus licencias actuales.

## Añadir un usuario {#add-a-user}

1. Vaya a la **Administrador** área.

   ![](assets/user-and-license-management-1.png)

1. Clic **Seminarios web interactivos**.

   ![](assets/user-and-license-management-2.png)

1. Clic **Agregar o quitar usuarios**.

   ![](assets/user-and-license-management-3.png)

1. Haga clic en el menú desplegable Usuarios disponibles, seleccione los usuarios que desee agregar y haga clic en **OK**.

   ![](assets/user-and-license-management-4.png)

## Eliminar un usuario {#remove-a-user}

1. Vaya a la **Administrador** área.

   ![](assets/user-and-license-management-5.png)

1. Clic **Seminarios web interactivos**.

   ![](assets/user-and-license-management-6.png)

1. Clic **Agregar o quitar usuarios**.

   ![](assets/user-and-license-management-7.png)

1. Resalte los usuarios que desee eliminar y presione la tecla Supr del teclado. Clic **OK** cuando termine.

   ![](assets/user-and-license-management-8.png)

## Uso de licencias {#license-usage}

Los seminarios web interactivos ofrecen licencias específicas para crear eventos con tecnología de Adobe Connect. Cada vez que se añada una licencia, aparecerá un nuevo cuadro de uso de licencia. Los administradores de Marketo pueden ver (no editar) las licencias siguiendo los pasos a continuación. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener licencias adicionales.

1. Vaya a la **Administrador** área.

   ![](assets/user-and-license-management-9.png)

1. Clic **Seminarios web interactivos**.

   ![](assets/user-and-license-management-10.png)

1. Desplácese hacia abajo hasta las tarjetas de Uso de licencias.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>Fecha de inicio</b></td>
   <td>Fecha de inicio de la licencia.</td>
  </tr>
  <tr> 
   <td><b>Fecha de caducidad</b></td>
   <td>Fecha de caducidad de la licencia.</td>
  </tr>
  <tr> 
   <td><b>Tipo</b></td>
   <td>El tipo de licencia adquirida. Hay tres tipos disponibles: licencia de eventos compartidos, licencia de salas compartidas, licencia de almacenamiento adicional.</td>
  </tr>
  <tr> 
   <td><b>Capacidad del evento</b></td>
   <td>Número máximo de participantes que pueden alojarse en un evento.</td>
  </tr>
  <tr> 
   <td><b>Eventos totales</b></td>
   <td>Número total de eventos que se han aprovisionado con esta licencia.</td>
  </tr>
  <tr> 
   <td><b>Eventos consumidos</b></td>
   <td>Número total de eventos completados.</td>
  </tr>
  <tr> 
   <td><b>Capacidad de almacenamiento</b></td>
   <td>Cantidad de almacenamiento disponible para almacenar grabaciones, garantías, heros images, documentación y otros recursos.</td>
  </tr>
  </tbody>
</table>

**Cosas que hay que tener en cuenta**

* El tipo &quot;Licencia de almacenamiento adicional&quot; solo proporciona almacenamiento, por lo tanto el valor en cada campo _además_ La capacidad de almacenamiento se indicará simplemente como &quot;-&quot;.

* El tipo &quot;Licencia de sala compartida&quot; tiene eventos ilimitados y &quot;Licencia de almacenamiento adicional&quot; solo proporciona almacenamiento, por lo que el campo Eventos totales para estas licencias se enumerará simplemente como &quot;-&quot;.

* Cada vez que se cree un evento, se contará como &quot;consumido&quot; desde su licencia respectiva (a menos que sea una licencia de sala compartida). Se dará preferencia a &quot;Licencia de evento compartido&quot; si hay &quot;Licencia de evento compartido&quot; y &quot;Licencia de habitación compartida&quot; de la misma capacidad. Si el evento no se ha entregado y si el programa de eventos se elimina antes de la hora programada, el recuento de eventos se reaprovisiona restando un evento de los eventos consumidos.

* Una vez agotada la licencia, el mosaico permanece en la pantalla Seminarios web interactivos de la sección Administración con &quot;Eventos totales&quot; y &quot;Eventos consumidos&quot; con el mismo valor. Solo cuando caduque la licencia se eliminará de la pantalla.
