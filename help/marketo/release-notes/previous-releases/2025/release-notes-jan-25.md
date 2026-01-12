---
description: 'Notas de la versión, enero de 2025: Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2025
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 35%

---

# Notas de la versión: enero de 2025 {#release-notes-jan-25}

A continuación encontrará todas las funciones incluidas en la versión de enero de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 17 de enero de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr>
   <td><strong>Nuevo Designer de correo electrónico</strong>: cree correos electrónicos modernos y eficientes con el nuevo Designer de correo electrónico nativo en Marketo Engage. Acceda a una de las plantillas de correo electrónico predeterminadas prediseñadas o cree las suyas propias fácilmente. Utilice contenido dinámico y acceda a imágenes desde los servicios en la nube de Adobe Experience Manager. Utilice la funcionalidad del acelerador de contenido Gen-AI para crear correos electrónicos innovadores y de rendimiento a escala.
   <p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Para acceder al nuevo diseñador de correo electrónico, su suscripción a Marketo Engage debe migrarse al <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Sistema Identity Management de Adobe (IMS)</a>. Si el suyo aún no se ha actualizado y desea solicitar que se agilice, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) o con el <a href="https://nation.marketo.com/t5/support/ct-p/Support">Soporte técnico de Marketo</a>. Para obtener acceso a la funcionalidad de la generación AI del acelerador de contenido, póngase en contacto con el equipo de cuenta de Adobe.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Información general del diseñador de correo electrónico</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Anular el registro de inscritos en un evento de seminarios web interactivos</strong>: Ahora, si no desea inscribir a un inscrito en el seminario web por algún motivo, puede anular el registro. El flujo de trabajo elimina al solicitante de registro tanto del programa de eventos de Marketo como de Adobe Connect.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Deshabilitar campañas en el archivo</strong>: deshabilite las campañas de déclencheur activas y cancele las ejecuciones por lotes programadas de campañas en una carpeta cuando se archive. Dado que hay una comprobación de permisos adicional para archivar carpetas que contienen campañas activas (Activar campaña de Déclencheur y Programar campaña por lotes), esta característica se deshabilita de forma predeterminada con esta versión y se puede habilitar si navega a <b>Administrador</b> &gt; <b>Cofre del tesoro</b> en la suscripción de Marketo Engage.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación de funciones sociales**: El miércoles 31 de julio de 2024, Marketo Engage comenzó la desaprobación de las siguientes funciones sociales del producto:

   * Sondeos
   * Botón social
   * Oferta de referencia
   * Compartir video
   * Sorteos

A partir de ese momento, los usuarios no han podido crear, clonar ni incrustar ninguna de estas funciones de Social en Marketo Engage. Los recursos sociales existentes seguirán funcionando hasta el 31 de enero de 2025. El 1 de febrero de 2025, los activos sociales dejarán de funcionar. Las funciones sociales incrustadas en las páginas de destino deberán eliminarse. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Obtener actualización de la API de los miembros del programa**: Hemos mejorado la API de [Obtener miembros del programa](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} para admitir la capacidad de recuperar el identificador de los miembros del programa. Esto se realiza añadiendo ID a la lista de campos especificados en el parámetro fields de la solicitud de API.

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del miércoles, 31 de marzo de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el miércoles, 31 de marzo de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
