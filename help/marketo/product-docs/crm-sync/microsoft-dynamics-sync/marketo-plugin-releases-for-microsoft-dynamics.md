---
unique-page-id: 10099389
description: 'Versiones de complementos de Marketo para Microsoft Dynamics: Marketo Docs: Documentación del producto'
title: Versiones de complementos de Marketo para Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Versiones de complementos de Marketo para Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

La primera vez que sincroniza con Microsoft Dynamics, descarga la última versión de los complementos para Marketo. Marketo actualiza periódicamente estos complementos para que pueda volver al mismo lugar y descargar la nueva versión.

[Descargar el complemento más reciente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) correspondiente a su versión de Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Actualización de la solución Dynamics {#updating-your-dynamics-solution}

1. Importe la última versión de la solución sobre la versión existente de su Dynamics CRM (por ejemplo: si su Dynamics CRM tiene la versión 1.4 y la versión más reciente es 1.5, importaría _over_ versión 1.4).

1. Verá la siguiente ventana emergente. Select **Actualizar** y **Mantener personalizaciones** y haga clic en **Importar**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Últimas versiones {#latest-versions}

>[!NOTE]
>
>Estas versiones funcionan tanto para las versiones locales como en línea de Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Versión</th> 
   <th colspan="1">Fecha de versión</th> 
   <th>Notas</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Compatibilidad con la sincronización de campos Multiselect Optionset (esta función solo está disponible para V9.X y versiones posteriores). .</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Se ha agregado compatibilidad con la sincronización de campañas con MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Se ha agregado compatibilidad con el proceso de selección de posibles clientes listo para usar para Microsoft Dynamics versión 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Corrección de errores: Error en el proceso empresarial al intentar instalar las soluciones de Marketo para Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Corrección de errores: Revisión interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Corrección de errores: El complemento no se suscribió a eventos que capturan el cambio de estado del objeto personalizado. Esta corrección es específica de Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Corrección de errores: Las actualizaciones de la función de contacto de oportunidad no se capturaban completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>Corrección de errores: Cuando se creó la oportunidad, se observó una transacción de actualización innecesaria sobre la función de oportunidad del cliente en el registro de marketing. </p><p>Corrección de errores: Se registró una transacción de eliminación adicional al eliminar la entidad customeroportunityrole.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Corrección de errores: Se ha hecho que la actualización y eliminación de objetos personalizados sean asincrónicas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Corrección de errores: Cuando el posible cliente tenía un filtro de sincronización establecido en NO y la oportunidad y el contacto no tenían un filtro de sincronización, no se generaba el registro de creación para el contacto y la oportunidad cuando se clasificaba el posible cliente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Corrección de errores: Se registró un evento de asignación cuando se desactivó el filtro de sincronización.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Corrección de errores: El cliente no pudo crear un posible cliente en CRM porque el usuario de inicio de sesión no tenía permiso de configuración de Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Corrección de errores: Se han creado límites de acceso para usuarios normales de Dynamics para solucionar problemas de seguridad.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Corrección de errores: Las actualizaciones en Dynamics no se sincronizaban con Marketo para ver los pasos y las imágenes.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Corrección de errores: Los registros de posibles clientes se sincronizaban con Marketo cuando el filtro de sincronización estaba establecido en false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Descargar la solución de administración de posibles clientes de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
