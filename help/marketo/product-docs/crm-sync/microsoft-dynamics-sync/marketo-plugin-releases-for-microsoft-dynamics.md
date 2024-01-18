---
unique-page-id: 10099389
description: 'Versiones de complementos de Marketo para Microsoft Dynamics: documentos de Marketo, documentación del producto'
title: Versiones de complementos de Marketo para Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: e99fa6d25bcf3c4a03234ce48dd17dd7c396c430
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Versiones de complementos de Marketo para Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

La primera vez que se sincroniza con Microsoft Dynamics, se descarga la versión más reciente de los complementos de Marketo. Marketo actualiza periódicamente estos complementos para que pueda volver al mismo lugar donde desea descargar la nueva versión.

[Descargar el complemento más reciente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} correspondiente a su versión de Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Actualización de la solución de Dynamics {#updating-your-dynamics-solution}

1. Importe la última versión de la solución a través de la versión existente de su Dynamics CRM (por ejemplo, si su Dynamics CRM tiene la versión 1.4 y la última versión es 1.5, importaría _sobre_ versión 1.4).

1. Verá la siguiente ventana emergente. Seleccionar **Actualizar** y **Mantener personalizaciones**, luego haga clic en **Importar**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Últimas versiones {#latest-versions}

>[!NOTE]
>
>Estas versiones funcionan tanto para las versiones locales como en línea de Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Versión</th> 
   <th colspan="1">Fecha de lanzamiento</th> 
   <th>Notas</th> 
  </tr>
  <tr> 
   <td colspan="1">5.0.2.1</td> 
   <td colspan="1">10/13/23</td> 
   <td colspan="1">Corrección de errores: Se han corregido errores relacionados con la sincronización de entidad personalizada.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.2.0</td> 
   <td colspan="1">24/03/23</td> 
   <td colspan="1">Corrección de errores: Se han corregido errores que impedían combinar contactos en MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.8</td> 
   <td colspan="1">27/03/23</td> 
   <td colspan="1">Corrección de errores: Evita que el complemento sobrescriba otras personalizaciones en los elementos de la IU en MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Compatibilidad con la sincronización de campos Conjunto de opciones de selección múltiple (esta función solo está disponible para V9.X y versiones posteriores).</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Se ha agregado compatibilidad con la sincronización de Campaign con MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">22/08/18</td> 
   <td colspan="1">Se ha agregado compatibilidad con el proceso de contacto de candidatos aptos para la versión 9.x de Microsoft Dynamics de forma predeterminada.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">27/6/18</td> 
   <td colspan="1">Corrección de errores: Error de proceso empresarial al intentar instalar las soluciones de Marketo para Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">29/9/17</td> 
   <td colspan="1">Corrección de errores: Revisión interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Corrección de errores: El complemento no se suscribió a eventos que capturaban el cambio de estado del objeto personalizado. Esta corrección es específica de Dynamics CRM local 2011.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">22/7/16</td> 
   <td colspan="1">Corrección de errores: Las actualizaciones de la función de contacto de oportunidad no se recopilaban completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">28/6/16</td> 
   <td colspan="1">Corrección de errores: Se observó una transacción de actualización innecesaria en la función de oportunidad de cliente en el registro de marketo cuando se creó la oportunidad.<p>Corrección de errores: Se registró una transacción de eliminación adicional al eliminar la entidad de rol de oportunidad de cliente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">31/5/16</td> 
   <td colspan="1">Corrección de errores: Se ha realizado la actualización y eliminación de objetos personalizados de forma asíncrona.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">8/4/16</td> 
   <td colspan="1">Corrección de errores: Cuando el posible cliente tenía un filtro de sincronización establecido en NO y la oportunidad y el contacto no tenían un filtro de sincronización, no se generaba el registro de creación para el contacto y la oportunidad cuando se clasificaba al posible cliente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">29/3/16</td> 
   <td>Corrección de errores: Se registró un evento de asignación cuando el filtro de sincronización estaba desactivado.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Corrección de errores: El cliente no pudo crear un posible cliente en CRM porque el usuario que inició sesión no tenía permiso de configuración de Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">18/01/16</td> 
   <td colspan="1">Corrección de errores: Se han creado límites de acceso para los usuarios normales de Dynamics a fin de solucionar problemas de seguridad.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">30/12/15</td> 
   <td>Corrección de errores: Las actualizaciones de Dynamics no se sincronizaban con Marketo para ver pasos e imágenes.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Corrección de errores: Los registros de posibles clientes se sincronizaban con Marketo cuando el filtro de sincronización se establecía en Falso.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
