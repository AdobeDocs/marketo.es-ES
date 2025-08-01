---
unique-page-id: 27656223
description: Instalar  [!DNL Salesforce] Personalización para clientes de Professional Edition - Documentos de Marketo - Documentación del producto
title: Instalar  [!DNL Salesforce] Personalización para clientes de Professional Edition
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Instalar la personalización de [!DNL Salesforce] para clientes de Professional Edition {#install-salesforce-customization-for-professional-edition-customers}

Los clientes con [!DNL Salesforce] Professional Edition tendrán que seguir estos pasos para instalar la personalización.

>[!PREREQUISITES]
>
>* El administrador de [!DNL Sales Connect] debe conectar sus cuentas de [!DNL Salesforce] y [!DNL Sales Connect].
>* La instancia [!DNL Salesforce] utilizada necesita espacio para instalar trece campos de actividad personalizados.

## Instalación {#installation}

1. En [!DNL Sales Connect], haga clic en el icono de engranaje en la esquina superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-4.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Salesforce]**.

   ![](assets/two-4.png)

1. Compruebe que está conectado a su cuenta de [!DNL Salesforce].

   >[!CAUTION]
   >
   >Si está conectado, verá un botón verde &quot;[!UICONTROL Instalar]&quot;. **NO** haga clic en este botón, continúe con el paso 4.

1. Inicie sesión en la cuenta de [!DNL Salesforce] a la que está conectado y haga clic en [este vínculo](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Se le enviará a la página de instalación de [!DNL Sales Connect].

   ![](assets/install-package.png)

1. Elija los usuarios para los que desea instalar las personalizaciones: Solo administrador, todos los usuarios o perfiles específicos.
1. Haga clic en el botón **[!UICONTROL Instalar]** para instalar la personalización.
1. Para confirmar que la instalación se haya realizado correctamente, inicie sesión en su cuenta de [!DNL Salesforce].
1. Haga clic en **[!UICONTROL Configuración]**, busque &quot;Paquetes instalados&quot; en la barra de búsqueda y haga clic en **[!UICONTROL Paquetes instalados]**.

   Ahí verá las personalizaciones de Marketo Sales Connect.

   Para poder configurar [!DNL Sales Connect] en su instancia de [!DNL Salesforce], siga los pasos que comienzan desde la sección &quot;CONFIGURACIÓN DEL PAQUETE DE SALESFORCE DE SALES ENGAGE&quot; en la página 7 de la Guía de instalación.

   >[!NOTE]
   >
   >[!DNL Sales Engage] es el nombre anterior de [!DNL Sales Connect].

## Guías {#guides}

[Guía de instalación de Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Guía de instalación de Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
