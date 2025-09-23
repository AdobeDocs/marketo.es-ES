---
description: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (empresarial/ilimitado): Documentos de Marketo: documentación del producto'
title: 'Paso 2 de 3: Creación de un usuario de Salesforce para Marketo (empresarial/ilimitado)'
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 4%

---

# Paso 2 de 3: Crear un usuario de Salesforce para Marketo (para empresas y sin límites) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estos pasos debe completarlos un administrador de Salesforce

>[!PREREQUISITES]
>
>[Paso 1 de 3: agregar campos de Marketo a Salesforce (empresarial/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

En este artículo, configurará los permisos de usuario en el perfil de Salesforce y creará una cuenta de integración de Marketo y Salesforce.

## Crear un perfil {#create-a-profile}

1. Haga clic en **[!UICONTROL Configuración]**.

   CAPTURA DE PANTALLA

1. Escriba &quot;perfiles&quot; en la barra de búsqueda de navegación y haga clic en el vínculo Perfiles.

   CAPTURA DE PANTALLA

1. Haga clic en Nuevo perfil.

   CAPTURA DE PANTALLA

1. Seleccione Usuario estándar, asigne un nombre al perfil &quot;Sincronización de Marketo-Salesforce&quot; y haga clic en Guardar.

   CAPTURA DE PANTALLA

## Definición de permisos de perfil {#set-profile-permissions}

1. Haga clic en Editar para establecer los permisos de seguridad.

   CAPTURA DE PANTALLA

1. En la sección Permisos administrativos, asegúrese de que las siguientes casillas estén marcadas:

   * API habilitada
   * Editar plantillas de HTML
   * Administrar documentos públicos
   * Administrar plantillas públicas

   >[!TIP]
   >
   >Asegúrese de marcar la casilla La contraseña nunca caduca.

1. En la sección Permisos generales de usuario, asegúrese de que las siguientes casillas estén marcadas:

   * Convertir posibles clientes
   * Editar eventos
   * Editar tareas

1. En la sección Permisos de objeto estándar, asegúrese de que los permisos Leer, Crear, Editar y Eliminar están marcados para:

   * Cuentas
   * Campañas
   * Contactos
   * Clientes potenciales
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permisos a las campañas si planea utilizar la sincronización de campañas.

   CAPTURA DE PANTALLA

1. Cuando termine, haga clic en Guardar en la parte inferior de la página.

   CAPTURA DE PANTALLA

## Definir permisos de campo {#set-field-permissions}

1. Hable con los especialistas en marketing para averiguar qué campos personalizados son necesarios para sincronizar.

   >[!NOTE]
   >
   >Este paso evitará que los campos que no necesite se muestren en Marketo, lo que reducirá el desorden y acelerará la sincronización.

1. En la página de detalles del perfil, vaya a la sección Seguridad de nivel de campo. Haga clic en Ver para editar la accesibilidad de los objetos:

   * Posible cliente
   * Contacto
   * Cuenta
   * Oportunidad

   >[!TIP]
   >
   >Puede configurar otros objetos según las necesidades de su organización.

1. Para cada objeto, haga clic en Editar.

   CAPTURA DE PANTALLA

1. Busque los campos innecesarios, asegúrese de que las opciones Acceso de lectura y Acceso de edición no estén seleccionadas. Haga clic en Guardar cuando termine.

   >[!NOTE]
   >
   >Editar solo la accesibilidad de los campos personalizados.

   CAPTURA DE PANTALLA

1. Una vez deshabilitados todos los campos innecesarios, debe comprobar los campos Acceso de lectura y Acceso de edición para los siguientes campos de objeto. Haga clic en Guardar cuando termine.

   TABLA

   CAPTURA DE PANTALLA

## Crear cuenta de sincronización de Marketo y Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Cree una cuenta de Salesforce específica (por ejemplo, `marketo@yourcompany.com`) para distinguir los cambios realizados por Marketo frente a otros usuarios de Salesforce.

1. Escriba &quot;Administrar usuarios&quot; en la barra de búsqueda de navegación y haga clic en Usuarios. Haga clic en Nuevo usuario.

   CAPTURA DE PANTALLA

   CAPTURA DE PANTALLA

1. Rellene los campos obligatorios. A continuación, seleccione la Licencia de usuario: Salesforce y el Perfil que ha creado anteriormente. Haga clic en Guardar cuando haya terminado.

   CAPTURA DE PANTALLA

Se ha completado el paso 2 de 3.
