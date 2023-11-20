---
description: 'Paso 2 de 3: Creación de un usuario de Veeva CRM para Marketo Engage - Documentos de Marketo - Documentación del producto'
title: 'Paso 2 de 3: Creación de un usuario de Veeva CRM para Marketo Engage'
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 4%

---

# Paso 2 de 3: Crear un usuario de Veeva CRM para Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>Los pasos de este artículo debe completarlos un administrador de Veeva CRM.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Agregar campos de Marketo a Salesforce (profesional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

En este artículo, personalizará los permisos de campo con un diseño de página de Veeva CRM y creará un usuario de sincronización de Marketo-Veeva CRM.

## Definir diseños de página {#set-page-layouts}

Los siguientes pasos permitirán al usuario de sincronización de Marketo actualizar los campos personalizados.

1. Haga clic en los diseños de página Cuenta (cuenta de persona) en la barra de búsqueda de navegación sin pulsar Intro y, a continuación, haga clic en **[!UICONTROL Diseño de página]** en Contactos.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Haga clic en **[!UICONTROL Diseños de página]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Clic **[!UICONTROL HCP - Profesional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Haga clic y arrastre un nuevo **[!UICONTROL Sección]** en el diseño de página.

1. Introduzca &quot;Marketo&quot; en Nombre de sección y haga clic en **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Haga clic en el campo Score y arrástrelo a la sección Marketo.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Repita el paso anterior para los siguientes campos:

   * Ciudad inferida
   * Compañía inferida
   * País inferido
   * Área metropolitana inferida
   * Código de área telefónico inferido
   * Código postal inferido
   * Región del estado inferida

   >[!NOTE]
   >
   >Estos campos deben estar en el diseño de página para que Marketo pueda leerlos y escribirlos.

   >[!TIP]
   >
   >Cree dos columnas para los campos arrastrándolas hacia abajo hasta el lado derecho de la página. Puede mover campos de un lado al otro para equilibrar las longitudes de las columnas.

1. Cuando haya terminado con el diseño HCP-Professional, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Repita esto para otros diseños de página de cuenta.

## Crear un perfil {#create-a-profile}

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de navegación y haga clic en **[!UICONTROL Perfiles]** vínculo.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Clic **[!UICONTROL Nuevo]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Seleccione Usuario estándar, asigne un nombre al perfil &quot;Sincronización de Marketo-Salesforce&quot; y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Definición de permisos de perfil {#set-profile-permissions}

1. Clic **[!UICONTROL Editar]** para establecer los permisos de seguridad.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. En la sección Permisos administrativos, asegúrese de que **[!UICONTROL API habilitada]** está seleccionado.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Asegúrese de marcar la casilla La contraseña nunca caduca.

1. En la sección Permisos generales de usuario, asegúrese de que **[!UICONTROL Editar eventos]** y **[!UICONTROL Editar tareas]** están seleccionados.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. En la sección Permisos de objeto estándar, asegúrese de que **[!UICONTROL Leer]**, **[!UICONTROL Crear]**, **[!UICONTROL Editar]**, y **[!UICONTROL Eliminar]** Los permisos de se comprueban en busca de cuentas y contactos.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. En la sección Permisos de objetos personalizados, asegúrese de que los permisos de lectura estén comprobados para **[!UICONTROL Llamada]**, **[!UICONTROL Mensaje de clave de llamada]** y cualquier otro objeto personalizado deseado.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Cuando termine, haga clic en **[!UICONTROL Guardar]** en la parte inferior de la página.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Definir permisos de campo {#set-field-permissions}

1. Hable con los especialistas en marketing para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite se muestren en Marketo, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a [!UICONTROL Seguridad de nivel de campo] sección. Clic **[!UICONTROL Ver]** para editar la accesibilidad de los objetos Contacto y Cuenta.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

1. Haga clic en cada objeto **[!UICONTROL Editar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Busque los campos innecesarios, asegúrese de que el acceso de lectura y el acceso de edición están _desenfrenado_. Clic **[!UICONTROL Guardar]** cuando termine.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Editar solo la accesibilidad de los campos personalizados.

1. Cuando termine de deshabilitar todos los campos innecesarios, compruebe Acceso de lectura y Acceso de edición para ver los siguientes campos de objeto. Clic **[!UICONTROL Guardar]** cuando termine.

<table>
 <tbody>
  <tr>
   <th>Objeto
   <th>Campos
  </tr>
  <tr>
   <td>Cuenta</td>
   <td>Campo Tipo</td>
  </tr>
  <tr>
   <td>Evento</td>
   <td>Todos los campos</td>
  </tr>
  <tr>
   <td>Tarea</td>
   <td>Todos los campos</td>
  </tr>
 </tbody>
</table>

## Crear usuario de sincronización {#create-sync-user}

Marketo requiere credenciales para acceder a Veeva CRM. Esto se realiza mejor con un usuario dedicado creado con los pasos a continuación.

>[!NOTE]
>
>Si su organización no tiene licencias adicionales de Veeva CRM, puede utilizar un usuario de marketing existente con el perfil de administrador del sistema.

1. Introduzca &quot;usuarios&quot; en la barra de búsqueda de navegación y haga clic en **[!UICONTROL Usuarios]** en Administrar usuarios.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Clic **[!UICONTROL Nuevo usuario]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Rellene los campos obligatorios, seleccione la licencia de usuario: Salesforce, establezca el perfil: Sincronizar usuario de Marketo y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Asegúrese de que la dirección de correo electrónico que ha introducido sea válida. Deberá iniciar sesión como el usuario de sincronización para restablecer la contraseña.

¡Excelente! Ahora tiene una cuenta que Marketo Engage puede utilizar para conectarse a Veeva CRM. Vamos a hacerlo...

>[!MORELIKETHIS]
>
>[Paso 3 de 3: Conectar Marketo y Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
