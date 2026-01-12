---
description: 'Notas de la versión, agosto de 2025: Documentos de Marketo: documentación del producto'
title: Notas de la versión, agosto de 2025
feature: Release Information
exl-id: f4f71a77-d0c0-41c3-9362-afbfb467cc7a
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 98%

---

# Notas de la versión: agosto de 2025 {#release-notes-aug-25}

A continuación encontrará todas las funciones incluidas en la versión de agosto de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **22 de agosto de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: sistema de informes</strong>: los informes de rendimiento de correo electrónico y de rendimiento de vínculos de correo electrónico ahora muestran datos de los correos electrónicos creados con el nuevo Diseñador de correo electrónico.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: eliminación de Autocompletar</strong>: la opción Autocompletar del editor de personalización de tókenes apuntaba a objetos erróneos y se ha eliminado. No hay planes para volver a implementar dicha opción en este momento.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: optimización de vista previa del correo electrónico</strong>: algunos usuarios experimentaban tiempos de carga más lentos al intentar obtener una vista previa de su correo electrónico en la página de detalles del correo electrónico/plantilla de correo electrónico/fragmento. Esta experiencia se ha optimizado para lograr tiempos de carga hasta un 60 % más rápidos.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: correcciones de plantilla</strong>: algunas plantillas predeterminadas tenían problemas de procesamiento (por ejemplo, no se representaban correctamente en determinados exploradores/modo oscuro, imágenes mal alineadas, botones de CTA mal colocados y algunos más). Todos estos problemas se han corregido con esta versión.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Diseñador de correo electrónico: corrección del bloqueo de contenido</strong>: anteriormente, si se creaba una plantilla de correo electrónico con bloqueo de contenido y esta se utilizaba para crear un correo electrónico, el bloqueo de contenido se mantenía incluso cuando se restablecía el correo electrónico o se seleccionaba “cambiar diseño”. Este problema se ha corregido con esta versión.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Fin de la vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (inicio de sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición al [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Restricciones de direcciones IP obsoletas_: la compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente estará disponible una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Inicio de sesión único (SSO) obsoleto_: la compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Desuso de la función _Reenviar a un amigo_**: el 29 de septiembre de 2025, la función _Reenviar a un amigo_ de los correos electrónicos de Marketo Engage 2.0 (el editor de correo electrónico heredado) quedará en desuso para todas las suscripciones. Esto afecta al token “Reenviar a un amigo” y a los vínculos “Reenviar a un amigo” en los correos electrónicos que ya se han enviado o que se enviarán usando el token. [Más información](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del miércoles, 31 de marzo de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el miércoles, 31 de marzo de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
