---
description: 'Información general de Adobe Identity Management: documentos de Marketo, documentación del producto'
title: Información general sobre Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 1defe6e8c7b4e458203169150ec77df4f615e5d2
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Información general sobre Adobe Identity Management {#adobe-identity-management-overview}

Todas las nuevas suscripciones de Adobe Marketo Engage (del 31 de julio de 2023 o posterior) están integradas con el sistema Identity Management de Adobe. Las suscripciones de Marketo Engage existentes se están migrando actualmente al sistema Identity Management de Adobe en cualquier evento de ventas, que incluye renovaciones, eventos de recontratación y/o complementos. Las migraciones fuera de un evento de ventas no son compatibles en este momento.

>[!NOTE]
>
>El Soporte de Marketo no puede proporcionar ninguna actualización con respecto a la migración de IMS de Adobe. El equipo de cuenta de Adobe se pondrá en contacto con el calendario estimado en los próximos meses. Para obtener más información, consulte [este artículo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} y las [preguntas más frecuentes](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Para las suscripciones integradas en Adobe Identity, Adobe Admin Console se utiliza para la administración de usuarios. Los conceptos relacionados con la identidad, como el inicio de sesión único, también se administran en el Admin Console.

* Más información sobre [Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html){target="_blank"}.
* Encuentra más información acerca de [configurar tu organización de Adobe relacionada con tu suscripción a Marketo](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Si desea implementar el inicio de sesión único y su suscripción se ha incorporado a Adobe Identity sin SSO implementado en la organización de Adobe, envíe un ticket a [Soporte técnico de Marketo](https://nation.marketo.com/){target="_blank"} y especifique el tema como &quot;Marketo en Admin Console, implementación de SSO&quot;.

## Niveles de perfil {#profile-levels}

Las suscripciones de Adobe Marketo Engage integradas en el sistema Identity Management de Adobe admiten varios perfiles. A continuación se indican los tipos de perfiles de usuario relevantes para esta integración.

<table>
 <tr>
  <td><strong>Administrador del sistema de Adobe Admin Console</strong></td>
  <td>Responsable de configurar los conceptos de identidad de la organización de Adobe y del producto de Marketo Engage en Adobe Admin Console. Se ha concedido la función en la configuración de organización de Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos Adobe Admin Console</strong></td>
  <td>Responsable de otorgar derechos a los usuarios para el producto de Marketo Engage en Adobe Admin Console. Función otorgada en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador de perfil de producto de Adobe Admin Console</strong></td>
  <td>Responsable de la administración de usuarios dentro de un perfil de producto. No pueden administrar usuarios que no pertenezcan a ese perfil específico. Un administrador de perfil de producto no tiene acceso a la aplicación de Marketo a menos que se añada al perfil de producto como usuario. Su función seguiría siendo un usuario estándar (espacio de trabajo predeterminado si tiene más de un espacio de trabajo).
</td>
 </tr>
 <tr>
  <td><strong>Administrador de Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso a un Marketo Engage con privilegios administrativos. Se ha concedido la función en Marketo Engage, no en Adobe Admin Console (aparece como "Admin" en el modal <b>Editar usuario</b>).</td>
 </tr>
 <tr>
  <td><strong>Usuario Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso al Marketo Engage. Sin privilegios administrativos.</td>
 </tr>
</table>

## Preguntas frecuentes {#faq}

Las preguntas más frecuentes [se pueden encontrar aquí](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configuración de administración](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Agregar o quitar un administrador de productos](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Agregar o quitar un usuario](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
