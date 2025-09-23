---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 76%

---

# Notas de la versión: septiembre de 2025 {#release-notes-sep-25}

A continuación encontrará todas las funciones incluidas en la versión de septiembre de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 19 de septiembre de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Retención de actividades de seminarios web bajo demanda</strong>: Los usuarios de seminarios web interactivos ahora tienen disponibles los datos del tablero de seminarios web bajo demanda durante más de 30 días (anteriormente solo eran hasta 30 días desde el día del seminario web).</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Cambio a Velocity Scripting en el nuevo Designer de correo electrónico**: Adobe Marketo Engage lanzó una función llamada _Contenido condicional_ para el nuevo Designer de correo electrónico el pasado junio. La función estaba equipada con scripts de Handlebar en lugar de scripts de Velocity, en un esfuerzo por proporcionar un poco más de flexibilidad en el contenido dinámico. Pero cuando descubrimos que estaba causando que algunos tokens se resolvieran incorrectamente, decidimos desactivarlo temporalmente. [Más información](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fin de la vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (inicio de sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición al [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Restricciones de direcciones IP obsoletas_: la compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente estará disponible una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Inicio de sesión único (SSO) obsoleto_: la compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Desuso de la función _Reenviar a un amigo_**: el 29 de septiembre de 2025, la función _Reenviar a un amigo_ de los correos electrónicos de Marketo Engage 2.0 (el editor de correo electrónico heredado) quedará en desuso para todas las suscripciones. Esto afecta al token “Reenviar a un amigo” y a los vínculos “Reenviar a un amigo” en los correos electrónicos que ya se han enviado o que se enviarán usando el token. [Más información](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado «Autorización» [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
