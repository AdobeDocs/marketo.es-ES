---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6d09e0f684844d7d2ced6205d7becde90ffcd7c7
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 41%

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
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Flujo de trabajo de Collaboration de contenido</strong>: ahora puede realizar comentarios y colaborar con otros usuarios de Marketo en un recurso de correo electrónico. Etiquete a los integrantes del equipo (usuarios de Marketo que tengan los permisos de recursos adecuados) y recibirán un correo electrónico o una notificación rápida.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Correo electrónico de Designer - Permisos del asistente de IA</strong>: Los administradores de Marketo pueden proporcionar a usuarios específicos acceso a las funciones de GenAI.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Modo oscuro</strong>: Ahora puede utilizar el Modo oscuro, que permite a los clientes de correo electrónico y a las aplicaciones compatibles mostrar correos electrónicos con fondos más oscuros y colores más claros para texto, botones y otros elementos de la interfaz de usuario.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Correcciones de redireccionamiento</strong>: Algunos usuarios experimentaban problemas de redireccionamiento con las direcciones URL de los mensajes de correo electrónico creados con el nuevo Designer (por ejemplo, al pegar directamente las direcciones URL o al marcar los recursos de correo electrónico, no siempre funcionaba). Este problema se ha resuelto. Además, los vínculos a los recursos de correo electrónico de <b>Plantillas de correo electrónico</b> &gt; <b>Detalles</b> &gt; <b>Utilizado por</b> se redirigirán al recurso de correo electrónico correspondiente.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Cambio a Velocity Scripting en el nuevo Designer de correo electrónico**: Adobe Marketo Engage lanzó una función llamada _Contenido condicional_ para el nuevo Designer de correo electrónico el pasado junio. La función estaba equipada con scripts de Handlebar en lugar de scripts de Velocity, en un esfuerzo por proporcionar un poco más de flexibilidad en el contenido dinámico. Pero cuando descubrimos que estaba causando que algunos tokens se resolvieran incorrectamente, decidimos desactivarlo temporalmente. [Más información](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fin de vida útil de Marketo Engage Identity**: en agosto de 2025, Adobe empezó a eliminar gradualmente la compatibilidad con Marketo Engage Identity (iniciando sesión a través de `login.marketo.com`). Para evitar que se interrumpa el acceso a Marketo Engage, debe realizar la transición al [Adobe Identity](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} a más tardar el 30 de septiembre de 2025.

   * _Desaprobación de restricciones de IP_: La compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente habrá una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Desaprobación del inicio de sesión único (SSO)_: La compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescencia de la función _Reenviar a un amigo_**: el 29 de septiembre de 2025, la función _Reenviar a un amigo_ de los correos electrónicos de Marketo Engage 2.0 (el editor de correo electrónico heredado) quedará en desuso para todas las suscripciones. Esto afecta a los vínculos &quot;Reenviar a un amigo&quot; y &quot;Reenviar a un amigo&quot; en los correos electrónicos que ya se han enviado o que se enviarán con el token. [Más información](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado «Autorización» [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
