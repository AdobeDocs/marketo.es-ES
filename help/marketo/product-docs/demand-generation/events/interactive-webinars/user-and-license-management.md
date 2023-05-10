---
description: 'Administración de usuarios y licencias: Documentos de Marketo: Documentación del producto'
title: Administración de usuarios y licencias
hide: true
hidefromtoc: true
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: 093af2946aa0279aff20d4388312fa7630e693a2
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Administración de usuarios y licencias {#user-and-license-management}

Aprenda a añadir y eliminar usuarios, así como a ver sus licencias actuales.

## Agregar un usuario {#add-a-user}

1. Vaya a la **Administrador** .

   ![](assets/user-and-license-management-1.png)

1. Haga clic en **Seminarios web interactivos**.

   ![](assets/user-and-license-management-2.png)

1. Haga clic en **Agregar o eliminar usuarios**.

   ![](assets/user-and-license-management-3.png)

1. Haga clic en la lista desplegable Usuarios disponibles , seleccione los usuarios que desee agregar y haga clic en **OK**.

   ![](assets/user-and-license-management-4.png)

## Eliminar un usuario {#remove-a-user}

1. Vaya a la **Administrador** .

   ![](assets/user-and-license-management-5.png)

1. Haga clic en **Seminarios web interactivos**.

   ![](assets/user-and-license-management-6.png)

1. Haga clic en **Agregar o eliminar usuarios**.

   ![](assets/user-and-license-management-7.png)

1. Resalte los usuarios que desee eliminar y pulse la tecla Eliminar del teclado. Haga clic en **OK** cuando haya terminado.

   ![](assets/user-and-license-management-8.png)

## Uso de licencias {#license-usage}

Los seminarios web interactivos ofrecen licencias específicas para crear eventos de Adobe Connect. Cada vez que se añade una licencia, aparece un nuevo cuadro de uso de la licencia. Los administradores de Marketo pueden ver (no editar) las licencias siguiendo los pasos a continuación. Póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas) para obtener licencias adicionales.

1. Vaya a la **Administrador** .

   ![](assets/user-and-license-management-9.png)

1. Haga clic en **Seminarios web interactivos**.

   ![](assets/user-and-license-management-10.png)

1. Desplácese hacia abajo hasta las tarjetas de Uso de licencias.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>Fecha de inicio</b></td>
   <td>Fecha en la que comienza la licencia.</td>
  </tr>
  <tr> 
   <td><b>Fecha de caducidad</b></td>
   <td>Fecha en la que caduca la licencia.</td>
  </tr>
  <tr> 
   <td><b>Tipo</b></td>
   <td>Tipo de licencia adquirida. Hay tres tipos disponibles: Licencia de eventos compartidos, Licencia de salas compartidas, Licencia de almacenamiento adicional.</td>
  </tr>
  <tr> 
   <td><b>Capacidad del evento</b></td>
   <td>Número máximo de participantes que se pueden alojar en un evento.</td>
  </tr>
  <tr> 
   <td><b>Eventos totales</b></td>
   <td>El número total de eventos que se han aprovisionado con esta licencia.</td>
  </tr>
  <tr> 
   <td><b>Eventos consumidos</b></td>
   <td>El número total de eventos completados.</td>
  </tr>
  <tr> 
   <td><b>Capacidad de almacenamiento</b></td>
   <td>Cantidad de almacenamiento disponible para almacenar grabaciones, colaterales, heros images, documentación y otros recursos.</td>
  </tr>
  </tbody>
</table>

**Aspectos a tener en cuenta**

* El tipo &quot;Licencia de almacenamiento adicional&quot; solo proporciona almacenamiento, por lo que el valor de cada campo _than_ La Capacidad de Almacenamiento de Información se incluirá simplemente como &quot;-&quot;.

* El tipo &quot;Licencia de habitación compartida&quot; tiene eventos ilimitados y &quot;Licencia de almacenamiento adicional&quot; solo proporciona almacenamiento, por lo que el campo Eventos totales para estas licencias se enumerará simplemente como &quot;-&quot;.

* Cada vez que se crea un evento, se cuenta como &quot;consumido&quot; a partir de su licencia correspondiente (a menos que sea una licencia de sala compartida). Se dará preferencia a la &quot;Licencia de Evento Compartido&quot; si existen tanto la &quot;Licencia de Evento Compartido&quot; como la &quot;Licencia de Sala Compartida&quot; de la misma capacidad. Si el evento no se ha entregado y si el programa de eventos se elimina antes de la hora programada, el recuento de eventos se reabastece restando un evento de los eventos consumidos.

* Una vez agotada la licencia, su mosaico permanece en la pantalla Seminarios web interactivos de la sección Administración con &quot;Eventos totales&quot; y &quot;Eventos consumidos&quot; con el mismo valor. Solo se eliminará de la pantalla cuando la licencia caduque.
