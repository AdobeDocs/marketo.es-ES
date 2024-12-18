---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: bf6525359d8bc206ed01220823b6c1de5734df55
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 6%

---

# Notas de la versión: enero de 2025 {#release-notes-jan-25}

A continuación encontrará todas las funciones incluidas en la versión de enero de 2025. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas del Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **17 de enero de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr> 
   <td><strong>Nuevo Designer de correo electrónico</strong>: cree correos electrónicos modernos y eficientes con el nuevo Designer de correo electrónico nativo en Marketo Engage. Acceda a una de las plantillas de correo electrónico predeterminadas prediseñadas o cree las suyas propias fácilmente. Utilice contenido dinámico y acceda a imágenes desde los servicios en la nube de Adobe Experience Manager.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
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

* **Obtener actualización de la API de los miembros del programa**: Hemos mejorado la API de [Obtener miembros del programa](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} para admitir la capacidad de recuperar el identificador de los miembros del programa. Esto se realiza añadiendo ID a la lista de campos especificados en el parámetro fields de la solicitud de API.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 30 de junio de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST mediante el encabezado &quot;Autorización&quot; [tal como se describe aquí](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* SOAP **Desaprobación de API de**: La compatibilidad con la API de MarketoSOAP finalizará el 31 de octubre de 2025. SOAP Los servicios que usan capacidades de API de deben migrarse a la [API de REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
