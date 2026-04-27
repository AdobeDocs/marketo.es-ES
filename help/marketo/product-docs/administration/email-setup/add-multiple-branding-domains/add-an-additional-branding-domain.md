---
unique-page-id: 11377395
description: Agregue dominios de promoción de la marca adicionales para varias marcas en una instancia, de modo que cada una tenga sus propios vínculos de seguimiento de marca.
title: Añadir un dominio de personalización de marca adicional
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 6638f4a24aac6cf828f443d17b896a9dec9bca16
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 21%

---

# Añadir un dominio de personalización de marca adicional {#add-an-additional-branding-domain}

Agregue un dominio de promoción de la marca adicional cuando ejecute varias marcas desde una sola instancia de Marketo y desee que cada una tenga sus propios vínculos de seguimiento de marca.

>[!PREREQUISITES]
>
>Debe [reemplazar el vínculo de seguimiento genérico](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} por un dominio con marca antes de agregar dominios con marca adicionales.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Haga clic en **[!UICONTROL Agregar]** para agregar un dominio de marca adicional.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Escriba el nombre del nuevo dominio de promoción de la marca, seleccione _Convertir en dominio principal_ o _Generar certificado SSL_ (ambos opcionales) y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Convertir en dominio principal_: conviértalo en su dominio principal, y todos los correos electrónicos existentes no enviados se establecerán en &quot;Predeterminado&quot; y todos los correos electrónicos recién creados se establecerán de forma predeterminada en el dominio principal. Puede [sobrescribir esto por correo electrónico](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Generar certificado SSL_: puede crear una capa de sockets seguros (SSL) con la creación del dominio. El primer dominio de seguimiento iniciará una configuración única de infraestructura que puede tardar unas horas. Se le notificará una vez finalizado y podrá configurar el primer dominio. Para agregar SSL a los dominios existentes, comuníquese con [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Editar SSL para dominios existentes

Siga estos pasos para habilitar SSL para los dominios existentes.

1. En el área _[!UICONTROL Administrador]_, seleccione **[!UICONTROL Correo electrónico]**.

1. En la ficha _[!UICONTROL Dominio]_, seleccione la fila de dominio y haga clic en **[!UICONTROL Agregar SSL]**.

   ![Administrador - Correo electrónico - Dominio - Agregar SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. En el cuadro de diálogo, haga clic en **[!UICONTROL Confirmar]**.

   ![Agregar SSL - Confirmar](./assets/generate-ssl-cert-confirm.png){width="400"}

## Mensajes de error {#error-messages}

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
    <td><i>SSL certificate has already been issued.</i></td>
    <td>Ya existe un certificado SSL para este dominio personalizado. No further action is needed unless the certificate has expired or needs to be reissued.</td>
  </tr>
  <tr>
    <td><i>The default domain was not found. Please contact Support for assistance.</i></td>
    <td>Se ha producido un problema al intentar localizar el dominio predeterminado. Please reach out to Support so they can investigate.</td>
  </tr>
  <tr>
    <td><i>Unexpected error encountered while creating a domain. Please contact Support for assistance.</i></td>
    <td>An unexpected error has occurred. Please gather logs and error details, and escalate the issue to <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
</tbody></table>

## Things to Note {#things-to-note}

* **DNS mapping for domain to Marketo Engage**: Before adding adding domains in the UI, you must [map CNAMEs to a Marketo-provided domain](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Custom SSLs**: If you need a custom SSL, please submit a [Support ticket](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Do not use the self-service checkbox for SSL creation.

* **Pre-existing SSLs**: While adding a domain, the system checks for pre-existing SSLs, which may have been manually created prior. If you encounter this validation, create your domain without selecting SSL creation, and we will connect them for you. [Contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} more additional details/options.

* **Deletion of domains**: Automatically deleting a domain **does not** delete the SSL certificate. Esta protección evita los errores de usuario que hacen que un sitio web no tenga certificados SSL. If you do want to remove the SSL certificates, [contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* If the domain you add is listed as anything other than a CNAME, the ability to add further branded tracking domains will be locked out. You will need to edit any existing domain and ensure it is a CNAME record and not, say, an A record. The Add button dynamically checks for CNAMES and CNAMES only.

>[!MORELIKETHIS]
>
>[Edit Your Default Branding Domain](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
