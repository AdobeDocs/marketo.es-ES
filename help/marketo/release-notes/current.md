---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# Notas de la versión: agosto de 2025 {#release-notes-aug-25}

A continuación encontrará todas las funciones incluidas en la versión de agosto de 2025. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **22 de agosto de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Informes</strong>: Los informes de rendimiento de vínculos de correo electrónico y de rendimiento de vínculos de correo electrónico ahora muestran datos de los correos electrónicos creados con el nuevo Designer de correo electrónico.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Optimización de vista previa de correo electrónico</strong>: Algunos usuarios experimentaban tiempos de carga más lentos al intentar previsualizar su correo electrónico en la página de detalles de la plantilla/fragmento de correo electrónico/correo electrónico. Esta experiencia se ha optimizado para tiempos de carga hasta un 60 % más rápidos.</td>
   <td><i>Próximamente</i></td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Correcciones de plantilla</strong>: Algunas plantillas predeterminadas tenían problemas de procesamiento (por ejemplo, no se representaban correctamente en ciertos exploradores/modo oscuro, imágenes mal alineadas, botones de CTA mal colocados y algunos más). Todas estas se corrigen con esta versión.</td>
   <td><i>Próximamente</i></td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Corrección de bloqueo de contenido</strong>: Anteriormente, si se creaba una plantilla de correo electrónico con bloqueo de contenido y esta se utilizaba para crear un correo electrónico, el bloqueo de contenido se mantenía incluso cuando se restablecía el correo electrónico o se seleccionaba "cambiar diseño". Este problema se corrigió en esta versión.</td>
   <td><i>Próximamente</i></td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Eliminación autocompletada</strong>: la opción Autocompletar del editor de personalización de tokens apuntaba a objetos erróneos y se ha eliminado. No hay planes para volver a implementarlo en este momento.</td>
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
 </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Fin de vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (iniciando sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición a [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Desaprobación de restricciones de IP_: La compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente habrá una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Desaprobación del inicio de sesión único (SSO)_: La compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST usando el encabezado &quot;Autorización&quot; [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API de REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
