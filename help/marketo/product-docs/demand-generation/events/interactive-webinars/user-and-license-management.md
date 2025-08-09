---
description: Administración de usuarios y licencias - Documentos de Marketo - Documentación del producto
title: Administración de usuarios y licencias
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 2%

---

# Administración de usuarios y licencias {#user-and-license-management}

Aprenda a añadir y eliminar usuarios, así como a ver sus licencias actuales.

## Añadir un usuario {#add-a-user}

1. Vaya al área de **Admin**.

   ![](assets/user-and-license-management-1.png)

1. Haga clic en **seminarios web interactivos**.

   ![](assets/user-and-license-management-2.png)

1. Haga clic en **Agregar o quitar usuarios**.

   ![](assets/user-and-license-management-3.png)

1. Haga clic en el menú desplegable Usuarios disponibles, seleccione los usuarios que desee agregar y haga clic en **Aceptar**.

   ![](assets/user-and-license-management-4.png)

## Eliminar un usuario {#remove-a-user}

1. Vaya al área de **Admin**.

   ![](assets/user-and-license-management-5.png)

1. Haga clic en **seminarios web interactivos**.

   ![](assets/user-and-license-management-6.png)

1. Haga clic en **Agregar o quitar usuarios**.

   ![](assets/user-and-license-management-7.png)

1. Resalte los usuarios que desee eliminar y presione la tecla Supr del teclado. Haga clic en **Aceptar** cuando haya terminado.

   ![](assets/user-and-license-management-8.png)

## Uso de licencias {#license-usage}

Los seminarios web interactivos ofrecen licencias específicas para crear eventos con tecnología de Adobe Connect. Cada vez que se añada una licencia, aparecerá un nuevo cuadro de uso de licencia. Los administradores de Marketo pueden ver (no editar) las licencias siguiendo los pasos a continuación. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener licencias adicionales.

1. Vaya al área de **Admin**.

   ![](assets/user-and-license-management-9.png)

1. Haga clic en **seminarios web interactivos**.

   ![](assets/user-and-license-management-10.png)

1. Desplácese hacia abajo hasta las tarjetas de Uso de licencias.

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>Fecha de inicio</b></td>
   <td width="80%">Fecha de inicio de la licencia.</td>
  </tr>
  <tr>
   <td width="20%"><b>Fecha de vencimiento</b></td>
   <td width="80%">Fecha de caducidad de la licencia.</td>
  </tr>
  <tr>
   <td width="20%"><b>Tipo</b></td>
   <td width="80%">El tipo de licencia adquirida. Hay tres tipos disponibles: licencia de eventos compartidos, licencia de salas compartidas, licencia de almacenamiento adicional.</td>
  </tr>
  <tr>
   <td width="20%"><b>Capacidad del evento</b></td>
   <td width="80%">Número máximo de participantes que pueden alojarse en un evento.</td>
  </tr>
  <tr>
   <td width="20%"><b>Eventos totales</b></td>
   <td width="80%">Número total de eventos que se han aprovisionado con esta licencia.</td>
  </tr>
  <tr>
   <td width="20%"><b>Eventos consumidos</b></td>
   <td width="80%">Todos los eventos completados y programados actualmente. <a href="#things-to-note">Más información</a></td>
  </tr>
  <tr>
   <td width="20%"><b>Capacidad de almacenamiento</b></td>
   <td width="80%">Cantidad de almacenamiento disponible para almacenar grabaciones, material colateral, imágenes a pantalla completa, documentación y otros recursos.</td>
  </tr>
  </tbody>
</table>

### Cosas que hay que tener en cuenta {#things-to-note}

* Cada vez que se crea un evento, se contabiliza como &quot;consumido&quot; desde su licencia respectiva (a menos que sea una licencia de sala compartida). Se da preferencia a &quot;Licencia de evento compartido&quot; si hay &quot;Licencia de evento compartido&quot; y &quot;Licencia de habitación compartida&quot; de la misma capacidad. Si el evento no se ha entregado y el programa de eventos se elimina antes de la hora programada, el recuento de eventos se reaprovisiona. Si el evento no se entrega y el programa de eventos no se elimina antes de la hora programada, el evento no se reaprovisiona.

* El tipo &quot;Licencia de almacenamiento adicional&quot; simplemente proporciona almacenamiento, por lo tanto el valor en cada campo _además de la Capacidad de almacenamiento de_ se indicará simplemente como &quot;-&quot;.

* El tipo &quot;Licencia de sala compartida&quot; tiene eventos ilimitados y &quot;Licencia de almacenamiento adicional&quot; solo proporciona almacenamiento, por lo que el campo Eventos totales para estas licencias se enumerará simplemente como &quot;-&quot;.

* Una vez agotada la licencia, el mosaico permanece en la pantalla Seminarios web interactivos de la sección Administración con &quot;Eventos totales&quot; y &quot;Eventos consumidos&quot; con el mismo valor. Solo cuando caduque la licencia se eliminará de la pantalla.

## Acceso del usuario {#user-access}

Los seminarios web interactivos tienen la funcionalidad de regular el uso mediante la concesión de permisos a los usuarios de Marketo Engage para crear y ofrecer seminarios web interactivos. Sin embargo, un usuario (o no usuario) de un seminario web interactivo podría tener acceso de lectura y edición a los programas de eventos de seminarios web interactivos creados por otros usuarios.

Los usuarios de Marketo a los que se hayan concedido permisos para seminarios web interactivos y que sean propietarios de un programa de eventos de seminarios web interactivos concreto podrán realizar todas las funciones de seminarios web interactivos relacionadas con ese programa. Esto incluye: crear, acceder, modificar, clonar, mover y eliminar ese programa. Sin embargo, una vez que el usuario ya no es un usuario del seminario web interactivo, el propietario del programa podría acceder y mover el programa, pero no realizar ninguna otra función.

Los usuarios de Marketo a los que se les hayan concedido permisos para seminarios web interactivos y que no sean propietarios de _ni de_ un programa de eventos de seminarios web interactivos en particular podrán realizar funciones limitadas en esos programas. Los usuarios no administradores de Marketo podrán acceder al programa y clonarlo, pero no podrán realizar otras funciones si tienen permisos para seminarios web interactivos. Sin embargo, los usuarios administradores de Marketo _podrán_ realizar todas las funciones, como acceder, modificar, clonar, mover y eliminar ese programa (siempre y cuando tengan permisos para seminarios web interactivos). Una vez revocado este permiso para los usuarios administradores de Marketo y los usuarios no administradores, solo podrían acceder al programa de eventos de seminario web interactivo y no podrían realizar otras funciones.

La restricción de las funciones procesables se indicaría mediante un botón de acción atenuado y un mensaje de desplazamiento. Algunos ejemplos de los botones de acción atenuados son &quot;Diseña tu seminario web&quot; o &quot;Entra en tu seminario web&quot;. En el caso de las funciones no procesables, se enviaría un mensaje en el que se destacarían las restricciones. Consulte el ejemplo siguiente:

![](assets/user-and-license-management-12.png)
