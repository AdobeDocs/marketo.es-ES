---
description: Información general sobre Adobe Identity Management para Marketo Engage, incluidos el tiempo de migración, la administración de usuarios de Admin Console y los niveles de perfil como administrador del sistema y administrador de productos.
title: Información general sobre Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
TQID: https://experienceleague.adobe.com/6af3WC1QOameThPvZTRmanxHl8nkFZaHquHJytngGmI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
subfeature_v2:
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 366
ht-degree: 6%

---

# Información general sobre Adobe Identity Management {#adobe-identity-management-overview}

Todas las nuevas suscripciones a Adobe Marketo Engage (el 31 de julio de 2023 o posterior) están integradas con el sistema Identity Management de Adobe.

Para las suscripciones integradas en Adobe identity, Adobe Admin Console se utiliza para la administración de usuarios. Los conceptos relacionados con la identidad, como el inicio de sesión único, también se administran en Admin Console.

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
  <td>Responsable de configurar los conceptos de identidad de la organización de Adobe y del producto de Marketo Engage en Adobe Admin Console. Se ha concedido la función en la configuración de organización Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos Adobe Admin Console</strong></td>
  <td>Responsable de otorgar derechos a los usuarios para el producto Marketo Engage en Adobe Admin Console. Función otorgada en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador de perfil de producto de Adobe Admin Console</strong></td>
  <td>Responsable de la administración de usuarios dentro de un perfil de producto. No pueden administrar usuarios que no pertenezcan a ese perfil específico. Un administrador de perfil de producto no tiene acceso a la aplicación de Marketo a menos que se añada al perfil de producto como usuario. Su función seguiría siendo un usuario estándar (espacio de trabajo predeterminado si tiene más de un espacio de trabajo).
</td>
 </tr>
 <tr>
  <td><strong>Administrador de Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso a Marketo Engage con privilegios administrativos. Se ha concedido la función en Marketo Engage, no en Adobe Admin Console (aparece solo como "Administrador" en el modal <b>Editar usuario</b>).</td>
 </tr>
 <tr>
  <td><strong>Usuario de Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso a Marketo Engage. Sin privilegios administrativos.</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [Configuración de administración](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Agregar o quitar un administrador de productos](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [Agregar o quitar un usuario](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
