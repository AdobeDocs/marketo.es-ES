---
unique-page-id: 3571797
description: Paso 2 de 3 -Crear un usuario de Salesforce para Marketing (Professional) - Documentos de marketing - Documentación del producto
title: 'Paso 2 de 3: Crear un usuario de Salesforce para Marketing (Professional)'
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Paso 2 de 3: Creación de un usuario de Salesforce para Marketing (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Estos pasos deben ser completados por un administrador de Salesforce

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Añadir campos de marketing a Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



En este artículo, personalizará los permisos de campo con un diseño de página de Salesforce y creará un usuario de sincronización de Marketing-Salesforce.

## Definir diseños de página {#set-page-layouts}

Salesforce Professional establece la accesibilidad a nivel de campo con los diseños de página, en lugar de los Perfiles de Salesforce Enterprise/Unlimited. Los siguientes pasos permitirán que el usuario de Marketing sincronice los campos personalizados.

1. Escriba los diseños **de página** en la barra de búsqueda de navegación sin pulsar **Intro** y haga clic en Diseño **de** página en **Posibles clientes**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Haga clic en **Editar** junto a Diseño de posibles clientes.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Haga clic y arrastre una nueva **sección** al diseño de página.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Introduzca &quot;Marcado&quot; en Nombre **de** sección y haga clic en **Aceptar**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Haga clic y arrastre el campo Fecha **de** adquisición a la sección **Comercialización** .

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Repita el paso anterior para los campos siguientes:

   * Programa de adquisición
   * ID de Programa de adquisición
   * Exclusión correo electrónico
   * Ciudad afectada
   * Compañía referida
   * País afectado
   * Área metropolitana vinculada
   * Código de área telefónica inducida
   * Código postal adjunto
   * Región de estado indirecto
   * Puntuación de posible cliente
   * Remitente del reenvío original
   * Motor de búsqueda original
   * Frase de búsqueda original
   * Información de origen original
   * Tipo de origen original

   >[!NOTE]
   >
   >Estos campos deben estar en el diseño de página para que Marketing pueda leerlos o escribirlos.

   >[!TIP]
   >
   >Cree dos columnas para los campos arrastrándolas hacia abajo hasta el lado derecho de la página. Puede mover los campos de un lado al otro para equilibrar la longitud de las columnas.

1. Haga clic en **Guardar** cuando termine de agregar campos.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Repita todos los pasos anteriores para el diseño **de página de** contacto de Salesforce.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Recuerde hacer clic en **Guardar** cuando termine con el diseño **de página de** contacto.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Asegúrese de que el campo Evento **de** todo el día se ha agregado al diseño **de página de** Evento.

## Crear usuario de sincronización {#create-sync-user}

Marketo requiere credenciales para acceder a Salesforce. Esto se realiza mejor con un usuario dedicado creado con los pasos a continuación.

>[!NOTE]
>
>Si su organización no dispone de licencias adicionales de Salesforce, puede utilizar un usuario **de** Marketing existente con el perfil de administrador **** del sistema.

1. Escriba &quot;usuarios&quot; en la barra de búsqueda de Nav y haga clic en **Usuarios** en **Administrar usuarios**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Haga clic en **Nuevo usuario**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Rellene los campos obligatorios y seleccione Licencia **de usuario: Salesforce**, establezca el **Perfil: Administrador** del sistema, marque Usuario **** de mercadotecnia y haga clic en **Guardar**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Asegúrese de que la dirección de correo electrónico especificada sea válida. Deberá iniciar sesión como usuario de sincronización para restablecer la contraseña.

¡Excelente! Ahora tiene una cuenta que Marketing puede utilizar para conectarse a Salesforce. Hagámoslo.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Paso 3 de 3: Connect Marketing y Salesforce (Professional)](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



