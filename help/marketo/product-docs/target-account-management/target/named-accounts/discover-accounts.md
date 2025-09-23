---
unique-page-id: 11378812
description: Descubrimiento de cuentas - Documentos de Marketo - Documentación del producto
title: Cuentas de Discover
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 1%

---

# Cuentas de Discover {#discover-accounts}

Utilice la opción Descubrir para identificar posibles cuentas de destino.

## [!UICONTROL Detectar cuentas de CRM] {#discover-crm-accounts}

Identifique las posibles cuentas de destino desde su CRM.

>[!NOTE]
>
>Después de conectar tu CRM a Marketo TAM, **[!UICONTROL Discover cuentas de CRM]** mostrará todas las cuentas de CRM y la información relevante para ayudarte a elegir las cuentas con nombre correctas. Marketo agrega información adicional sobre lo que se recibe del CRM.

**[!UICONTROL Personas]** (En [!UICONTROL Discover Cuentas CRM] y [!UICONTROL Discover Compañías Marketo]): Incluye contactos y posibles clientes. Los posibles clientes se pueden descubrir usando la coincidencia de [cliente potencial con cuenta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md) de Marketo.

**[!UICONTROL Personas potenciales]** (en [!UICONTROL Discover Cuentas de CRM] y [!UICONTROL Discover Compañías de Marketo]): Muestra cuántos posibles clientes encontró Marketo que podrían pertenecer a una cuenta de CRM.

**Campo personalizado de CRM** (solo en Discover cuentas de CRM): Esto le ayudará a alinear su organización de ventas y marketing para la selección de cuentas de destino correctas. Una vez que [asigne el campo personalizado CRM](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) con Marketo TAM, le mostraremos los datos asignados para ayudarle a identificar sus cuentas de destino.

1. En [!UICONTROL Cuentas con nombre], haga clic en la lista desplegable **[!UICONTROL Nuevas]** y seleccione **[!UICONTROL Detectar cuentas de CRM]**.

   ![](assets/disc-crm-one.png)

1. Se abrirá una nueva ventana/pestaña. Seleccione las cuentas de CRM que desee agregar a sus [!UICONTROL cuentas con nombre] y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/disc-crm-two.png)

1. La pantalla de previsualización confirma la cantidad de selecciones. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/disc-three.png)

   ¡Eso es todo lo que hay!

   ![](assets/disc-four.png)

## [!UICONTROL Descubrir Compañías De Marketo] {#discover-marketo-companies}

Identifique las empresas adecuadas para la segmentación.

>[!NOTE]
>
>En [!UICONTROL Descubrir Compañías de Marketo], verá compañías de Marketo que no provienen de su CRM.

1. En [!UICONTROL Cuentas con nombre], haga clic en la lista desplegable **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Descubrir compañías de Marketo]**.

   ![](assets/one-1.png)

1. Se abrirá una nueva ventana/pestaña. Seleccione las empresas que desee agregar a sus [!UICONTROL cuentas con nombre] y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >En [!UICONTROL Discover Compañías de Marketo] y Discover CRM, Marketo automáticamente:
   >
   >* Busca personas de la base de datos de Marketo que tengan esa compañía en el registro. Si ve varios valores para algunos atributos (por ejemplo, Sector), es porque Marketo encontró valores diferentes en la lista para esas personas individuales. El atributo con la mayor cantidad de visitas gana
   >
   >Solo en **Discover CRM**, Marketo automáticamente:
   >
   >* Sincroniza y asocia los contactos de CRM con la [!UICONTROL cuenta con nombre]
   >
   >Solo en **[!UICONTROL Descubrir compañías de Marketo]**, Marketo automáticamente:
   >
   >* Filtra la mayoría de los proveedores de servicios de Internet y dominios públicos (como yahoo.com, gmail.com) como nombres de empresa
   >
   >* Desduplica cuentas de CRM. Si tiene &quot;Acme&quot; en un registro y &quot;Acme Inc&quot; (o cualquiera de los siguientes sufijos: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), los fusionaremos en TAM como solo &quot;Acme&quot;

1. Haga clic en la flecha abajo debajo de la columna [!UICONTROL Cuenta con nombre] para mostrar la lista desplegable.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >En adelante, cualquier nueva persona de estas empresas seleccionadas se asignará automáticamente a sus respectivas cuentas con nombre. Compruebe estas empresas y asegúrese de que estén asignadas a la [!UICONTROL cuenta con nombre] correcta.

1. Para seleccionar una cuenta existente, haga clic en la lista desplegable **[!UICONTROL Cuenta con nombre]**, elija la cuenta que desee y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/disc-comp-four.png)

   También tiene la opción de crear una nueva [!UICONTROL cuenta con nombre] escribiendo el nombre deseado directamente en el cuadro desplegable. Haga clic fuera del cuadro cuando termine...

   ![](assets/disc-comp-five.png)

   ...y verá su nueva [!UICONTROL cuenta con nombre]. En ese momento, simplemente haga clic en **[!UICONTROL Siguiente]** como en el paso 4.

   ![](assets/disc-comp-six.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/disc-comp-seven.png)

   ¡Buen trabajo!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Si ve una discrepancia entre las cuentas de CRM que ha seleccionado y lo que hay en la cuadrícula de Discover CRM, es probable que se deba a uno o más de los siguientes factores:
>
>* Tener cuentas de CRM diferentes con nombres similares que se deduplicaron
>* Aún no se ha producido la siguiente sincronización programada

>[!MORELIKETHIS]
>
>[Coincidencia de cliente potencial con cuenta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
