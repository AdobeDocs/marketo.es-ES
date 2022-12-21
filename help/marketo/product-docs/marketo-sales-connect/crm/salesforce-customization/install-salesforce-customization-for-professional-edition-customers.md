---
unique-page-id: 27656223
description: Instalación de la personalización de Salesforce para clientes de Professional Edition - Marketo Docs - Documentación del producto
title: Instalación de la personalización de Salesforce para clientes de Professional Edition
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Instalación de la personalización de Salesforce para clientes de Professional Edition {#install-salesforce-customization-for-professional-edition-customers}

Los clientes con Salesforce Professional Edition deberán seguir estos pasos para instalar la personalización.

>[!PREREQUISITES]
>
>* El administrador de conexión de ventas debe conectar sus cuentas de Salesforce y de Conexión de ventas.
>* La instancia de Salesforce utilizada debe tener espacio para instalar trece campos de actividad personalizados.


## Instalación {#installation}

1. En Conexión de ventas, haga clic en el icono de engranaje en la esquina superior derecha y seleccione **Configuración**.

   ![](assets/one-4.png)

1. En Configuración de administración, haga clic en **Salesforce**.

   ![](assets/two-4.png)

1. Compruebe que está conectado a su cuenta de Salesforce.

   >[!CAUTION]
   >
   >Si está conectado, verá un botón verde &quot;Instalar&quot;. **NO** haga clic en este botón, vaya al paso 4 en su lugar.

1. Inicie sesión en la cuenta de Salesforce a la que está conectado y, a continuación, haga clic en [este vínculo](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Se le enviará a la página Instalación de Conexión de Ventas.

   ![](assets/install-package.png)

1. Elija los usuarios para los que desea instalar las personalizaciones: Solo administrador, todos los usuarios o perfiles específicos.
1. Haga clic en el **Instalar** para instalar la personalización.
1. Para confirmar que la instalación se ha realizado correctamente, inicie sesión en su cuenta de Salesforce.
1. Haga clic en **Configuración**, busque &quot;Paquetes instalados&quot; en la barra de búsqueda y haga clic en **Paquetes instalados**.

   Aquí podrá ver Personalizaciones de Marketo Sales Connect .

   Para configurar Sales Connect en su instancia de Salesforce, siga los pasos que comienzan desde la sección &quot;CONFIGURING THE SALES ENGAGE SALESFORCE PACKAGE&quot; en la página 7 de la Guía de Instalación.

   >[!NOTE]
   >
   >Participación de ventas es el nombre anterior de Conexión de ventas.

## Guías {#guides}

[Guía de instalación de Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Guía de instalación de Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
