---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 978bbe4de06a0e269b60108e5a91edc5499dc9c1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 7%

---

# Notas de la versión: marzo de 2025 {#release-notes-mar-25}

A continuación encontrará todas las características incluidas en la versión de marzo del 25. Consulte la disponibilidad de funciones en su edición de Adobe Systems Marketo Engage.

Las notas de la versión específicas para Adobe Systems Dynamic Chat [se pueden encontrar aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las características señaladas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Comuníquese con su representante Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y inicio se lanzarán el **28 de marzo de 2025**, con una despliegue gradual de las características restantes en las semanas siguientes. Las características y fechas de la versión están sujetas a cambios. Verifique el estado junto a cada característica.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr> 
   <td><strong>Email Designer disponible en todos los programas</strong>: Los correos electrónicos de Nuevo Email Designer ahora son accesibles a través de los programas de participación, predeterminados y eventos (con la única excepción de interactivo programas de seminarios web). Anteriormente, solo estaban disponibles en programas de correo electrónico. Con esta actualización, la clonación también está disponible.</td>
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Características de GenAI en interactivo seminarios web</strong>: Ahora puede generar capítulos, así como un resumen para seminarios web bajo demanda. Editar y exporte un archivo HTML de sus datos.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Mis tokens</strong> globales y Espacio de trabajo: configurar mis tokens tanto a nivel espacio de trabajo como global para permitir una productividad y un control mejorados sobre marca y marketing colateral en Marketo Engage espacios de trabajo y igualado instancias completas.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Tokens para cualquier atributo</strong> de activación: amplía el lista de tokens de activación disponibles desde la lista de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">este documento</a> para admitir el uso de datos de cualquier atributo de actividad desencadenante en campos de flujo de campaña. Impresión datos de un atributo de actividad a un momento interesante o establezca el último ID de transacción de un posible cliente desde un actividad personalizado en un campo posible cliente.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Desuso** de funciones de Social: El miércoles 31 de julio de 2024, Marketo Engage comenzó la obsolescencia de las siguientes funciones de Social dentro del producto:

   * Sondeos
   * Botón social
   * Oferta recomendada
   * Compartir video
   * Sorteos

Desde entonces, los usuarios no han podido crear, clonar o incrustar ninguna de esas características Social en Marketo Engage. Los Social existentes activos seguirán funcionando hasta el 31 de enero de 2025. El 1 de febrero de 2025, Social activos dejó de funcionar. Será necesario eliminar todas las funciones sociales incrustadas en las páginas de aterrizaje. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Obsolescencia** del parámetro &quot;access_token&quot; de la API de REST: El `access_token` parámetro consulta utilizado para autenticar las llamadas a la API REST de Marketo quedará obsoleto y no estará disponible después del 30 de junio de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST mediante el encabezado [&quot;Autorización&quot;, tal y como se describe aquí](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desuso de** la API SOAP: El soporte para la API SOAP de Marketo finalizará el 31 de octubre de 2025. Los servicios que usan capacidades de API SOAP deben migrarse a la [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} de REST.

* **Nuevo Analytics Feature - Public Beta**: [Avanzadas BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conocida como Revenue Explorer y Avanzadas Report Builder) comienza a implementarse para todos los usuarios actuales de Revenue Cycle Explorer a mediados de abril. Este nuevo herramienta ofrece una interfaz flexible de sistema de informes y visualización en Marketo Engage datos, proporcionando detalles granulares sobre progresión, rendimiento y más. Cuenta con interactividad y visualización más ricas, un rendimiento más rápido y un experiencia del usuario más fluido e intuitivo.

Para acceder a esta función, debe haber adquirido el complemento Avanzadas BI Analytics. Póngase en contacto con el equipo de Adobe Systems cuentas (su administrador de cuenta) para obtener más información.
