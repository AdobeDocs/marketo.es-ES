---
unique-page-id: 12615800
description: 'Importación de cuentas con nombre: documentación de Marketo: documentación del producto'
title: Importar cuentas con nombre
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Importar cuentas con nombre {#import-named-accounts}

¿Ya tiene un CSV lleno de posibles cuentas de destinatario? ¡Importarlos directamente en TAM!

1. Haga clic en **Nuevo** y seleccione. **Importar cuentas con nombre**.

   ![](assets/inaone.png)

1. Se abrirá una nueva ventana. Clic **Examinar**, a continuación, seleccione el archivo de cuentas con nombre que desee importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >En su archivo, indique [tanta información](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) como sea posible. Solo puede agregar información firmográfica; no hay nada que Marketo calcule (es decir, Canalización). Para crear cuentas con nombre basadas en cuentas de CRM, simplemente exporte el nombre de la cuenta y el ID de CRM desde su CRM a un archivo CSV, utilice la opción Nombre de cuenta y asigne el ID de CRM durante el proceso de importación. Para vincular correctamente una cuenta CRM a una cuenta con nombre, debe proporcionar el nombre exacto de la cuenta CRM.

1. Elija entre dos modos desduplicados: Nombre de cuenta o Nombre de dominio. En este ejemplo, elegimos Cuenta. Haga clic en **Modos** y seleccione. **Por nombre de cuenta**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Si elige **Por modo de dominio** No obstante, se deben incluir tanto los campos de cuenta con nombre como los de dominio.

1. Para elegir a qué lista de cuentas se agrega su cuenta con nombre, haga clic en **Lista de cuentas** y realice la selección.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >También puede crear una lista de cuentas completamente nueva simplemente escribiendo su nombre en el cuadro desplegable.

1. Para enviar una notificación de la importación, haga clic en **Enviar alerta a** y seleccione un usuario de Marketo. Usted _no puede_ introduzca manualmente una dirección de correo electrónico.

   ![](assets/inafive-2.png)

1. Clic **Siguiente**.

   ![](assets/inasix-2.png)

1. Asigne cada campo haciendo doble clic en **Campo de Marketo** y seleccione el campo correspondiente. Clic **Siguiente** cuando termine.

   ![](assets/inaseven.png)

   Sin errores!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Comprobar estado de importación&quot; solo muestra los últimos tres días de actividad.

Escenarios en los que se desduplica por nombre de cuenta:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta existente</strong></td> 
   <td><p>Actualizaremos el registro existente</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta nuevo</strong></td> 
   <td>Crearemos un nuevo registro</td> 
  </tr> 
 </tbody> 
</table>

Situaciones en las que se desduplica por nombre de dominio:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importación de un registro con un nuevo nombre de cuenta y un nuevo nombre de dominio</strong></td> 
   <td>Crearemos una nueva cuenta con nombre con la información proporcionada</td> 
  </tr> 
  <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta existente y un nombre de dominio existente</strong></td> 
   <td>Actualizaremos la cuenta con nombre existente</td> 
  </tr> 
   <tr> 
   <td><strong>Importación de un registro con un nombre de cuenta nuevo y un nombre de dominio existente</strong></td> 
   <td>Anexaremos el nuevo nombre de cuenta a la cuenta con nombre existente que coincida con el nombre de dominio y actualizaremos otra información (por ejemplo: industria, estado, etc.)</td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro con nombre de cuenta existente y nombre de dominio nuevo</strong></td> 
   <td>Anexaremos el nuevo nombre de dominio a la cuenta con nombre existente que coincida con el nombre de la cuenta y actualizaremos otra información (por ejemplo: industria, estado, etc.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Cuando Marketo adjunta una cuenta con nombre, estamos actualizando una regla (en segundo plano) que nos permite identificar a las personas que deben formar parte de la cuenta con nombre. Ejemplo: si actualiza &quot;IBM&quot; a &quot;IBM, EE. UU.&quot;, las personas con cualquier nombre de compañía se asociarán a la cuenta con nombre.

Si Marketo encuentra registros que vemos como duplicados, solo procesaremos el primero.
