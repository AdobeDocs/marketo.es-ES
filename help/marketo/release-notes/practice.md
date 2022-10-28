---
description: Notas de la versión de la práctica - Documentos de Marketo - Documentación del producto
title: Notas de la versión de la práctica
hide: true
hidefromtoc: true
source-git-commit: f57bb27c1b33e1c47c69f68c3719a35ee3f2d82e
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 2%

---

# Notas de la versión: Octubre de 2022 {#release-notes-oct-22}

A continuación encontrará todas las funciones incluidas en la versión del 22 de octubre. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

Las siguientes funciones empezarán a lanzarse en **14 de octubre de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario). Las funciones de la versión y las fechas exactas están sujetas a cambios.

## Organización en canales múltiples {#cross-channel-orchestration}

_**Chat dinámico**_

* **Organizar automáticamente los flujos de diálogo para la conversación dinámica**: Mejore su lienzo de diálogo lleno organizando todo en el lienzo en un formato limpio y fácil de leer con la pulsación de un botón a través de la organización automática.

* **Compatibilidad con tipos de datos adicionales para Dynamic Chat**: Tres nuevos tipos de datos (booleano, entero, flotante) le permiten aprovechar los campos de Marketo Engage existentes en Dynamic Chat para cosas como el targeting basado en puntuaciones o preguntar a los visitantes sí/no preguntas.

* **Vínculos de reunión para Dynamic Chat**: Opción para incluir automáticamente un vínculo de equipos o reunión para Google y Outlook en cada invitación de calendario que se envíe a los visitantes.

* **Notificaciones de reuniones programadas para chat dinámico**: Los representantes de ventas reciben notificaciones automatizadas por correo electrónico con respecto a las reuniones programadas, así como cualquier información relevante sobre la interacción de bots de chat del visitante.

* **Roles y permisos para Dynamic Chat**: Los administradores pueden utilizar permisos granulares para controlar la visibilidad y el uso de la aplicación y crear funciones de usuario personalizadas.

   * Acceso total: los usuarios pueden aprovechar al máximo la función (p. ej., publicar cuadros de diálogo, cambiar esquema de colores, etc.)
   * Acceso de solo lectura: los usuarios pueden ver información, pero no pueden realizar cambios (por ejemplo, consulte Criterios de audiencia o Diseñador de flujo, pero no modificar)
   * Acceso restringido: los usuarios no pueden ver ni acceder a las secciones Configuración o Integraciones

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

## Experiencia de próxima generación {#next-generation-experience}

* **Pantallas actualizadas en la experiencia de próxima generación**: Ofrecemos pantallas adicionales y actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador:

   * Detalles de la plantilla de página de aterrizaje
   * Lista de plantillas de correo electrónico

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md">Alternar conmutador</a></td>
  </tr>
  </tbody>
</table>

* **Mejora utilizada por la pestaña en Detalles de plantilla de correo electrónico**: En la nueva experiencia, verá información adicional relacionada con los recursos que utilizan la plantilla de correo electrónico, incluidos Estado del recurso, Última modificación y Última modificación por. También puede buscar, ordenar y filtrar la lista de recursos que usan.

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td>n.a</td>
  </tr>
  </tbody>
</table>

* **Modelos del filtro de recursos de informes**: Nuevo diseño para los modelos de configuración de informes que muestran un nuevo árbol de recursos en el menú de configuración y un filtro para Fecha de creación y modificación.

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td>n.a</td>
  </tr>
  </tbody>
</table>

## Entorno de datos de marketing {#marketing-data-environment}

* **Integración del Privacy Service de Adobe**: Armonice con el Privacy Service para automatizar el cumplimiento de las normas de privacidad de datos en todos los productos de Experience Cloud. Actualmente, este servicio solo está disponible para los clientes Marketo Engage que hayan incorporado al sistema Identity Management de Adobe.

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

## Mejoras de API {#api-enhancements}

* **Importación masiva de posibles clientes: Asociación de vendedores**: Paridad con la API de Lead REST para poder asociar posibles clientes con los vendedores durante el proceso de importación de posibles clientes en masa, lo que reduce la complejidad y el número de llamadas de API necesarias.

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">Importación masiva de posibles clientes</a></td>
  </tr>
  </tbody>
</table>

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Integración de perspectivas de ventas con Dynamic Chat**: El panel de perspectivas ahora incluye actividades de chat dinámico en la cuadrícula inteligente junto con un resumen semanal y tarjetas de detalle.

<table> 
  <tr> 
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de documentación</b></td>
  </tr>
  <tr> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integración de Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Anuncios {#announcements}

* **Forms 1.0**: La desaprobación de Forms 1.0 se completará con la versión de octubre. Los recursos de Forms 1.0 ya no podrán enviar datos al Marketo Engage y devolverán errores si se intenta hacerlo.

* **Forms sin script**: Forms dejará de funcionar cuando Javascript esté deshabilitado en el explorador. El envío de formularios requerirá que Javascript esté habilitado.
