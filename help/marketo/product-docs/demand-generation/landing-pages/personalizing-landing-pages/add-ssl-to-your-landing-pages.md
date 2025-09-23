---
unique-page-id: 2359828
description: 'Añadir SSL a las páginas de aterrizaje: documentación de Marketo'
title: Añadir SSL a sus páginas de destino
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 2%

---

# Añadir SSL a sus páginas de destino {#add-ssl-to-your-landing-pages}

El cifrado SSL (Secure Socket Layer) permite que todas las páginas de destino de una instancia de Marketo Engage sean seguras.

Al rellenar un formulario web o visitar una página de aterrizaje alojada en Marketo Engage, la información se envía de forma predeterminada a través de un protocolo no seguro (HTTP). Según la política de su empresa, es posible que desee proteger la información enviada a Marketo a través de (HTTPS). Por ejemplo, cuando visite `http://info.mydomain.com/`, ahora será `https://info.mydomain.com/`.

Marketo Engage realiza un seguimiento predeterminado de &quot;Página web visitada&quot; y &quot;Haga clic en el vínculo de la página web&quot; a través del protocolo HTTP no seguro. Si desea que los vínculos de seguimiento estén protegidos con su propio certificado, debe hacer que Marketo cree un servidor no compartido independiente para habilitarlo. Proteger todos los aspectos de la interacción de un contacto con usted suele significar proteger tanto las páginas de aterrizaje como los vínculos de seguimiento.

>[!IMPORTANT]
>
>Antes de añadir un SSL, asegúrese de comprobar en su contrato el número total de dominios que puede añadir. De lo contrario, podría incurrir en una tarifa. Si no encuentra la información, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Habilitar la certificación SSL {#enable-ssl-certification}

Agregue automáticamente SSL para todos los alias de dominio que cree como parte de las reglas de la página de aterrizaje.

1. Vaya al área de **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Seleccione **Páginas de aterrizaje** del árbol. En la ficha **Reglas**, haga clic en la lista desplegable **Nuevo** y seleccione **Nuevo alias de dominio**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Escriba su _alias de dominio_ y _página predeterminada_. Seleccione la casilla de verificación **Generar certificado SSL**. Haga clic en **Crear** cuando haya terminado.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Esto agrega automáticamente un certificado SSL para este dominio.

## Habilite SSL para su dominio predeterminado {#enable-ssl-default-domain}

Siga los pasos a continuación para habilitar SSL para su dominio predeterminado.

1. En la sección **Admin**, seleccione **Páginas de aterrizaje**. Haga clic en el botón **Editar** naranja que está junto a _Configuración_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Si lo desea, también puede modificar el nombre de dominio aquí (se requiere un dominio válido).

1. Seleccione la casilla de verificación &quot;Generar certificado SSL&quot; y haga clic en Guardar.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>SSL puede tardar hasta tres minutos en estar en el estado READY. Actualice la página para que aparezcan los cambios.

## Editar SSL para alias de dominios existentes

Siga estos pasos para habilitar SSL para los alias de dominio existentes.

1. Desde el área de _[!UICONTROL Admin]_, expanda **[!UICONTROL Integration]** en la navegación izquierda y seleccione **[!UICONTROL Páginas de aterrizaje]**.

1. En la página, seleccione la ficha **[!UICONTROL Reglas]** en la parte superior.

1. Seleccione la fila de alias de dominio que desee editar y haga clic en **[!UICONTROL Agregar SSL]** en la parte superior.

   ![Área de administración - Integración > Páginas de aterrizaje - pestaña Reglas - seleccionar alias de dominio](./assets/admin-landing-pages-rules-add-ssl.png){width="800" zoomable="yes"}

1. En el cuadro de diálogo, haga clic en **[!UICONTROL Confirmar]**.

   ![Agregar SSL - Confirmar](./assets/generate-ssl-cert-confirm.png){width="400"}

>[!NOTE]
>
>SSL puede tardar hasta tres minutos en estar en el estado READY. Actualice la página para que aparezcan los cambios.

## Mensajes de error {#error-messages}

A continuación, encontrará mensajes de error que puede recibir junto con sus definiciones.

<table><thead>
  <tr>
    <th>Error</th>
    <th>Detalles</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>El dominio ya existe.</i></td>
    <td>Ya existe un dominio con el mismo nombre.</td>
  </tr>
  <tr>
    <td><i>El dominio no está asignado al dominio predeterminado.</i></td>
    <td>El dominio personalizado no está asignado correctamente al dominio predeterminado. Compruebe la configuración de asignación de dominios y asegúrese de que la configuración de DNS apunta al dominio predeterminado correcto.</td>
  </tr>
  <tr>
    <td><i>No se pudieron emitir certificados SSL debido a registros CAA no admitidos. Solicite a su departamento de TI que actualice sus registros de CAA.</i></td>
    <td>Los registros de CAA no están actualizados. Para aquellos que utilizan certificados SSL administrados por Marketo Engage, los registros CAA deben actualizarse a los certificados recomendados por nuestro proveedor. Póngase en contacto con el departamento de TI para actualizar los registros de CAA. Consulte <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">esta página</a> para obtener más información.</td>
  </tr>
  <tr>
    <td><i>Ya se ha emitido el certificado SSL.</i></td>
    <td>Ya existe un certificado SSL para este dominio personalizado. No es necesario realizar ninguna otra acción a menos que el certificado haya caducado o sea necesario volver a emitirlo.</td>
  </tr>
  <tr>
    <td><i>No se ha encontrado el dominio predeterminado. Póngase en contacto con Soporte para obtener ayuda.</i></td>
    <td>Se ha producido un problema al intentar localizar el dominio predeterminado. Póngase en contacto con Asistencia para que puedan investigar.</td>
  </tr>
  <tr>
    <td><i>Error inesperado al crear un dominio. Póngase en contacto con Soporte para obtener ayuda.</i></td>
    <td>Se ha producido un error inesperado. Recopile registros y detalles del error y envíe el problema al <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Soporte técnico de Marketo</a>.</td>
  </tr>
</tbody></table>

## Cosas que hay que tener en cuenta {#things-to-note}

* **Asignación de DNS para el dominio en Marketo Engage**: antes de agregar dominios en la interfaz de usuario, debe [asignar CNAME a un dominio proporcionado por Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personalizados**: Si necesita un SSL personalizado, envíe un [ticket de asistencia](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. No utilice la casilla de verificación de autoservicio para la creación SSL.

* **SSL preexistentes**: Al agregar un dominio, el sistema comprueba los SSL preexistentes, que pueden haberse creado manualmente anteriormente. Si encuentra esta validación, cree su dominio sin seleccionar la creación de SSL y los conectaremos por usted. [Póngase en contacto con el soporte técnico](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para obtener más detalles u opciones.

* **Eliminación de dominios**: Al eliminar automáticamente un dominio **no** se elimina el certificado SSL. Esta protección evita los errores de usuario que hacen que un sitio web no tenga certificados SSL. Si desea quitar los certificados SSL, [póngase en contacto con el soporte técnico](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
