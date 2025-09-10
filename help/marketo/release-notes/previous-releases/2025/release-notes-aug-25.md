---
description: 'Notas de la versión, agosto de 2025: Documentos de Marketo: documentación del producto'
title: Notas de la versión, agosto de 2025
feature: Release Information
source-git-commit: 95dda7d6e09f0e64fbce8e5bd39613f10ebde382
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 43%

---

# Notas de la versión: agosto de 2025 {#release-notes-aug-25}

A continuación encontrará todas las funciones incluidas en la versión de agosto de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 22 de agosto de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Informes</strong>: Los informes de rendimiento de vínculos de correo electrónico y de rendimiento de vínculos de correo electrónico ahora muestran datos de los correos electrónicos creados con el nuevo Designer de correo electrónico.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Eliminación autocompletada</strong>: la opción Autocompletar del editor de personalización de tokens apuntaba a objetos erróneos y se ha eliminado. No hay planes para volver a implementarlo en este momento.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Optimización de vista previa de correo electrónico</strong>: Algunos usuarios experimentaban tiempos de carga más lentos al intentar previsualizar su correo electrónico en la página de detalles de la plantilla/fragmento de correo electrónico/correo electrónico. Esta experiencia se ha optimizado para tiempos de carga hasta un 60 % más rápidos.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Correcciones de plantilla</strong>: Algunas plantillas predeterminadas tenían problemas de procesamiento (por ejemplo, no se representaban correctamente en ciertos exploradores/modo oscuro, imágenes mal alineadas, botones de CTA mal colocados y algunos más). Todas estas se corrigen con esta versión.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Corrección de bloqueo de contenido</strong>: Anteriormente, si se creaba una plantilla de correo electrónico con bloqueo de contenido y esta se utilizaba para crear un correo electrónico, el bloqueo de contenido se mantenía incluso cuando se restablecía el correo electrónico o se seleccionaba "cambiar diseño". Este problema se corrigió en esta versión.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Permiso para editar límites de campañas inteligentes</strong>: Los administradores ahora pueden restringir la capacidad de modificar límites de campañas inteligentes solo para usuarios con permisos.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Fin de vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (iniciando sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición al [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Desaprobación de restricciones de IP_: La compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente habrá una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Desaprobación del inicio de sesión único (SSO)_: La compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescencia de la función _Reenviar a un amigo_**: el 29 de septiembre de 2025, la función _Reenviar a un amigo_ de los correos electrónicos de Marketo Engage 2.0 (el editor de correo electrónico heredado) quedará en desuso para todas las suscripciones. Esto afecta a los vínculos &quot;Reenviar a un amigo&quot; y &quot;Reenviar a un amigo&quot; en los correos electrónicos que ya se han enviado o que se enviarán con el token. [Más información](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado «Autorización» [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
