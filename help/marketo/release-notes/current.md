---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: a53178021f3abdbfc5e1cdff76bc1f0483c4b887
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 99%

---

# Notas de la versión: octubre de 2025 {#release-notes-oct-25}

A continuación, encontrará todas las funciones incluidas en la versión de octubre de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **31 de octubre de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico, importador de plantillas (beta)</strong>: importe plantillas de correo electrónico desde el editor de correo electrónico clásico para crear plantillas compatibles con el nuevo Diseñador de correo electrónico en Design Studio.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Importación de plantilla</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: contenido condicional</strong>: función de paridad del nuevo Diseñador de correo electrónico, que le permite lograr una personalización de correo electrónico más allá de los tokens.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: Prueba A/B</strong>: función de paridad del nuevo diseñador de correo electrónico, que le permite realizar pruebas A/B para ver qué tipos de contenido reciben la mejor respuesta.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: temáticas de marca</strong>: ahora puede definir temáticas de marca dentro de Marketo Engage. Las configuraciones del estilo se pueden reutilizar y aplicar en plantillas de correo electrónico y otros recursos de correo electrónico para mantener la uniformidad de la marca.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>Diseñador de correo electrónico: conversor de imagen a HTML</strong>: cargue un archivo de imagen PNG/JPEG compatible de un mensaje de correo electrónico y se convertirá automáticamente a HTML para utilizarlo en el nuevo Diseñador de correo electrónico.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: clonar acción de correo electrónico</strong>: ahora puede clonar un correo electrónico en otra carpeta de programas en Actividades de marketing y reutilizar rápidamente los correos electrónicos existentes.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Actualización de la integración de Salesforce CRM**: se implementará una nueva versión de la integración de CRM nativa en las zonas protegidas activas que tengan habilitado el conector nativo durante siete días, a partir del 13 de noviembre de 2025. Obtenga detalles completos en [esta publicación de Nation](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}

* **Doble barra diagonal de la API de REST en desuso**: el 16 de septiembre de 2025, Adobe realizó la transición a una infraestructura de alojamiento más moderna para las direcciones URL de la API de REST que aprovecha lo último en tecnología, añadiendo seguridad y escalabilidad. Si su suscripción ha estado usando las API con una doble barra diagonal (//) en la URL, lea [esta publicación de Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} para ver los próximos pasos.

* **Cambio a los scripts de Velocity en el nuevo diseñador de correo electrónico**: Adobe Marketo Engage lanzó una función llamada _Contenido condicional_ para el nuevo Diseñador de correo electrónico el pasado junio. La función estaba equipada con scripts de Handlebar en lugar de los scripts de Velocity, con el fin de proporcionar un poco más de flexibilidad en el contenido dinámico. Pero cuando descubrimos que estaba causando que algunos tókenes se resolvieran incorrectamente, decidimos desactivarlo temporalmente. [Más información](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fin de la vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (inicio de sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición al [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Restricciones de direcciones IP obsoletas_: la compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente estará disponible una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Inicio de sesión único (SSO) obsoleto_: la compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Desuso de la función _Reenviar a un amigo_**: el 29 de septiembre de 2025, la función _Reenviar a un amigo_ de los correos electrónicos de Marketo Engage 2.0 (el editor de correo electrónico heredado) quedará completamente en desuso para todas las suscripciones. Esto afecta al token &quot;Reenviar a un amigo&quot; y a los vínculos &quot;Reenviar a un amigo&quot; en los correos electrónicos que ya se han enviado o que se enviarán usando el token. [Más información](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
