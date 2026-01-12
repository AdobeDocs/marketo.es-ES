---
description: 'Notas de la versión, marzo de 2025: Documentos de Marketo: documentación del producto'
title: Notas de la versión, marzo de 2025
feature: Release Information
exl-id: a0e45d8e-6b74-4ab0-a1ba-4dae3754bc8f
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 39%

---

# Notas de la versión: marzo de 2025 {#release-notes-mar-25}

A continuación encontrará todas las funciones incluidas en la versión de marzo de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 28 de marzo de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr>
   <td><strong>Designer de correo electrónico disponible en todos los programas</strong>: ahora se puede acceder a los nuevos correos electrónicos de Designer de correo electrónico en los programas de participación, predeterminados y de eventos (excepto en los programas de seminarios web interactivos). Anteriormente, solo estaban disponibles en Programas de correo electrónico.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td>Características de <strong>GenAI en seminarios web interactivos</strong>: ahora puede generar capítulos y un resumen de los seminarios web a petición. Edite y exporte un archivo HTML de sus datos.</td>
   <td>Enviado</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai">Funciones de GenAI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Mis tokens globales y de Workspace</strong>: configúrelos tanto a nivel global como de espacio de trabajo para permitir un mayor control y productividad sobre las garantías de marca y marketing en los espacios de trabajo de Marketo Engage e incluso en instancias completas.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md#create-a-my-token">Crear un token My global</a></td>
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

A partir de ese momento, los usuarios no han podido crear, clonar ni incrustar ninguna de estas funciones de Social en Marketo Engage. Los recursos sociales existentes seguirán funcionando hasta el 31 de enero de 2025. El 1 de febrero de 2025, los activos sociales dejaron de funcionar. Deberá eliminar cualquier función social incrustada en las páginas de destino. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del miércoles, 31 de marzo de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el miércoles, 31 de marzo de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Nueva característica de Analytics - Beta público**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conocido como Revenue Explorer y Advanced Report Builder) comienza a implementarse para todos los usuarios actuales del Revenue Cycle Explorer a mediados de abril. Esta nueva herramienta ofrece una interfaz flexible de creación de informes y visualización en datos de Marketo Engage, que proporciona detalles granulares sobre progresión, rendimiento, etc. Ofrece una mejor interactividad y visualización, un rendimiento más rápido y una experiencia de usuario más fluida e intuitiva.

Para acceder a esta función, debe haber adquirido el complemento de Analytics de BI avanzado. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
