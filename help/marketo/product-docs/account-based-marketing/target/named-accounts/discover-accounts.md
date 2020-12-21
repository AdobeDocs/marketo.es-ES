---
unique-page-id: 11378812
description: Cuentas de Discover - Documentos de marketing - Documentación del producto
title: Cuentas de Discover
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---


# Cuentas de Discover {#discover-accounts}

Utilice la opción Discover para identificar posibles cuentas de destinatario.

## Cuentas CRM de Discover {#discover-crm-accounts}

Identifique las cuentas de destinatario potenciales de su CRM.

>[!NOTE]
>
>Después de conectar su CRM a ABM de Marketing, **Cuentas de CRM de Discover** mostrará todas las cuentas de CRM e información relevante para ayudarle a elegir las cuentas con nombre correctas. Marketo agrega información adicional sobre lo que se ha recibido de CRM.

**Personas**  (En Cuentas CRM de Discover y Compañías de Marketing de Discover): Incluye Contactos y Posibles clientes. Los posibles clientes se pueden descubrir mediante la coincidencia [de cliente potencial a cuenta](/help/marketo/product-docs/account-based-marketing/target/named-accounts/lead-to-account-matching.md) de Marketing.

**Posibles personas**  (En las cuentas CRM de Discover y en las Compañías de marketing de Discover): Muestra cuántos posibles clientes encontrados por el Marketing que podrían pertenecer a una cuenta CRM.

**Campo**  CRM personalizado (solo en cuentas CRM de Discover): Esto le ayudará a alinear su organización de ventas y marketing para seleccionar las cuentas de destinatario correctas. Una vez que [asigne el campo CRM personalizado](/help/marketo/product-docs/account-based-marketing/setup-abm/create-a-custom-field-for-crm-discovery.md) a ABM de Marketing, le mostraremos los datos asignados para ayudarle a identificar sus cuentas de destinatario.

1. En Cuentas con nombre, haga clic en la lista desplegable **Nueva** y seleccione **Cuentas CRM de Discover**.

   ![](assets/disc-crm-one.png)

1. Se abrirá una nueva ventana/ficha. Seleccione las cuentas de CRM que desee agregar a sus cuentas con nombre y haga clic en **Siguiente**.

   ![](assets/disc-crm-two.png)

1. La pantalla previsualización confirma la cantidad de selecciones. Haga clic en **Crear**.

   ![](assets/disc-three.png)

   ¡Eso es todo lo que hay!

   ![](assets/disc-four.png)

## Compañías de Discover Marketing {#discover-marketo-companies}

Identifique las compañías correctas para la segmentación.

>[!NOTE]
>
>En las Compañías de Discover Marketing, verá compañías de Marketing que no provienen de su CRM.

1. En Cuentas con nombre, haga clic en la lista desplegable **Nueva** y seleccione **Compañías de Discover Marketing**.

   ![](assets/one-1.png)

1. Se abrirá una nueva ventana/ficha. Seleccione las compañías que desee agregar a sus cuentas con nombre y haga clic en **Siguiente**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >En las Compañías de mercadotecnia de Discover y en CRM de Discover, Marketo automáticamente:
   >
   >* Encuentra personas de la base de datos de Marketing que tienen esa compañía en su registro. Si ve varios valores para algunos de los atributos (por ejemplo, Industria), es porque Marketing encontró valores diferentes enumerados para esas personas individuales. El atributo con la mayor cantidad de visitas gana
   >
   >Solo en **CRM de Discover**, Marcado automáticamente:
   >
   >* Sincroniza y asocia contactos de CRM con la cuenta con nombre
   >
   >Solo en **Compañías de Discover Marketing to**, Marcado automáticamente:
   >
   >* Filtros a la mayoría de los Proveedores de servicio de Internet y Dominios públicos (por ejemplo, yahoo.com, gmail.com) como nombres de compañía
      >
      >
   * Desduplica las cuentas de CRM. Si tiene &quot;Acme&quot; en un registro y &quot;Acme Inc&quot; (o cualquiera de los sufijos siguientes: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, LP, Ltd, PA, PC, PLC, PLLC), los fusionaremos en ABM como simplemente &quot;Acme&quot;.
   >
   >Si desea que Marketing desduplice cuentas por ID de CRM o Propietario de cuenta en lugar de por nombre de Compañía, póngase en contacto con [Asistencia técnica de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Haga clic en la flecha hacia abajo situada debajo de la columna Cuenta con nombre para mostrar la lista desplegable.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >A partir de ahora, cualquier persona nueva de estas compañías seleccionadas se asignará automáticamente a sus respectivas cuentas con nombre. Compruebe con el doble estas compañías y asegúrese de que están asignadas a la cuenta con nombre correcta.

1. Para seleccionar una cuenta existente, haga clic en la lista desplegable **Cuenta con nombre**, elija la cuenta que desee y haga clic en **Siguiente**.

   ![](assets/disc-comp-four.png)

   También tiene la opción de crear una nueva cuenta con nombre escribiendo el nombre deseado directamente en el cuadro desplegable. Haga clic fuera del cuadro cuando termine...

   ![](assets/disc-comp-five.png)

   ...y verá su nueva cuenta con nombre. En ese punto, haga clic en **Siguiente** como en el paso 4.

   ![](assets/disc-comp-six.png)

1. Haga clic en **Crear**.

   ![](assets/disc-comp-seven.png)

   ¡Buen trabajo!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Si ve una discordancia entre las cuentas de CRM que seleccionó y lo que hay en la cuadrícula de CRM de Discover, probablemente se deba a una o varias de las siguientes causas:
>
>* Tener cuentas CRM diferentes con nombres similares que se han desdoblado
>* Aún no se ha producido la siguiente sincronización programada


>[!MORELIKETHIS]
>
>[Coincidencia de posibles clientes con cuentas](/help/marketo/product-docs/account-based-marketing/target/named-accounts/lead-to-account-matching.md)
