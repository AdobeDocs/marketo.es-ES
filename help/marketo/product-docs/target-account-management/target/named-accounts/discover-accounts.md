---
unique-page-id: 11378812
description: Descubrimiento de cuentas - Documentos de Marketo - Documentación del producto
title: Detectar cuentas
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 1%

---

# Detectar cuentas {#discover-accounts}

Utilice la opción Descubrir para identificar posibles cuentas de destino.

## Descubrir cuentas de CRM {#discover-crm-accounts}

Identifique las posibles cuentas de destino desde su CRM.

>[!NOTE]
>
>Después de conectar tu CRM a Marketo TAM, **Discover cuentas de CRM** mostrará todas las cuentas de CRM y la información relevante para ayudarte a elegir las cuentas con nombre correctas. Marketo agrega información adicional sobre lo que se recibe del CRM.

**Personas** (En Cuentas de Discover CRM y Compañías de Discover Marketo): Incluye contactos y posibles clientes. Los posibles clientes se pueden descubrir usando la coincidencia de [cliente potencial con cuenta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md) de Marketo.

**Personas potenciales** (en Discover Cuentas de CRM y Discover Compañías de Marketo): Muestra cuántos posibles clientes encontró Marketo que podrían pertenecer a una cuenta de CRM.

**Campo personalizado de CRM** (solo en Discover cuentas de CRM): Esto le ayudará a alinear su organización de ventas y marketing para la selección de cuentas de destino correctas. Una vez que [asigne el campo personalizado CRM](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) con Marketo TAM, le mostraremos los datos asignados para ayudarle a identificar sus cuentas de destino.

1. En Cuentas con nombre, haga clic en la lista desplegable **Nuevas** y seleccione **Detectar cuentas de CRM**.

   ![](assets/disc-crm-one.png)

1. Se abrirá una nueva ventana/pestaña. Seleccione las cuentas de CRM que desee agregar a sus cuentas con nombre y haga clic en **Siguiente**.

   ![](assets/disc-crm-two.png)

1. La pantalla de previsualización confirma la cantidad de selecciones. Haga clic en **Crear**.

   ![](assets/disc-three.png)

   ¡Eso es todo lo que hay!

   ![](assets/disc-four.png)

## Descubrir compañías de Marketo {#discover-marketo-companies}

Identifique las empresas adecuadas para la segmentación.

>[!NOTE]
>
>En Discover Marketo Companies, verá compañías de Marketo que no provienen de su CRM.

1. En Cuentas con nombre, haga clic en el menú desplegable **Nuevo** y seleccione **Descubrir compañías de Marketo**.

   ![](assets/one-1.png)

1. Se abrirá una nueva ventana/pestaña. Seleccione las empresas que desee agregar a sus cuentas con nombre y haga clic en **Siguiente**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >En Discover Marketo Companies y Discover CRM, Marketo hace lo siguiente automáticamente:
   >
   >* Busca personas de la base de datos de Marketo que tengan esa compañía en el registro. Si ve varios valores para algunos atributos (por ejemplo, Sector), es porque Marketo encontró valores diferentes en la lista para esas personas individuales. El atributo con la mayor cantidad de visitas gana
   >
   >Solo en **Discover CRM**, Marketo automáticamente:
   >
   >* Sincroniza y asocia los contactos de CRM con la cuenta con nombre
   >
   >Solo en **Descubrir compañías de Marketo**, Marketo automáticamente:
   >
   >* Filtra la mayoría de los proveedores de servicios de Internet y dominios públicos (como yahoo.com, gmail.com) como nombres de empresa
   >
   >* Desduplica cuentas de CRM. Si tiene &quot;Acme&quot; en un registro y &quot;Acme Inc&quot; (o cualquiera de los siguientes sufijos: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), los fusionaremos en TAM como solo &quot;Acme&quot;
   >
   >Si desea que Marketo anule la duplicación de cuentas por ID de CRM o propietario de cuenta en lugar de por nombre de empresa, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Haga clic en la flecha hacia abajo debajo de la columna Cuenta con nombre para mostrar la lista desplegable.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >En adelante, cualquier nueva persona de estas empresas seleccionadas se asignará automáticamente a sus respectivas cuentas con nombre. Compruebe estas empresas y asegúrese de que están asignadas a la cuenta con nombre correcta.

1. Para seleccionar una cuenta existente, haga clic en la lista desplegable **Cuenta con nombre**, elija la cuenta que desee y haga clic en **Siguiente**.

   ![](assets/disc-comp-four.png)

   También tiene la opción de crear una nueva cuenta con nombre escribiendo el nombre deseado directamente en el cuadro desplegable. Haga clic fuera del cuadro cuando termine...

   ![](assets/disc-comp-five.png)

   ...y verá su nueva Cuenta con Nombre. En ese momento, simplemente haga clic en **Siguiente** como en el paso 4.

   ![](assets/disc-comp-six.png)

1. Haga clic en **Crear**.

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
