---
unique-page-id: 10099389
description: 'Versiones de complementos de Marketo para Microsoft Dynamics: Documentos de Marketo: Documentación del producto'
title: Versiones de complementos de Marketo para Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 7%

---

# Versiones de complementos de Marketo para Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Al sincronizar por primera vez con Microsoft Dynamics, se descarga la última versión de los complementos para Marketo. Marketo actualiza periódicamente estos complementos para que pueda volver al mismo lugar y descargar la nueva versión.

[Descargue el último ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) complemento correspondiente a su versión de Dynamics.

![](assets/lead-management-solution.png)

## Actualización de la solución de Dynamics {#updating-your-dynamics-solution}

1. Importe la última versión de la solución sobre la versión existente de su Dynamics CRM (por ejemplo: si su Dynamics CRM tiene la versión 1.4 y la versión más reciente es 1.5, importaría _sobre_ versión 1.4).

1. Verá la siguiente ventana emergente. Seleccione **Actualizar** y **Mantener personalizaciones** y haga clic en **Importar**.

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
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">16/10/20</td> 
   <td colspan="1">Se ha agregado compatibilidad con la sincronización de campañas con MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">22/8/18</td> 
   <td colspan="1">Se ha agregado compatibilidad con el proceso de selección de posibles clientes listo para usar para Microsoft Dynamics versión 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">27/6/18</td> 
   <td colspan="1">Corrección de errores: Error en el proceso empresarial al intentar instalar las soluciones de Marketo para Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">29/9/17</td> 
   <td colspan="1">Corrección de errores: Revisión interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">9/11/16</td> 
   <td colspan="1">Corrección de errores: El complemento no se suscribió a eventos que capturan el cambio de estado del objeto personalizado. Esta corrección es específica de Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">22/7/16</td> 
   <td colspan="1">Corrección de errores: Las actualizaciones de la función de contacto de oportunidad no se capturaban completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">28/6/16</td> 
   <td colspan="1"><p>Corrección de errores: Cuando se creó la oportunidad, se observó una transacción de actualización innecesaria sobre la función de oportunidad del cliente en el registro de marketing. </p><p>Corrección de errores: Se registró una transacción de eliminación adicional al eliminar la entidad customeroportunityrole.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">31/5/16</td> 
   <td colspan="1">Corrección de errores:  Se ha hecho que la actualización y eliminación de objetos personalizados sean asincrónicas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">8/4/16</td> 
   <td colspan="1">Corrección de errores: Cuando el posible cliente tenía un filtro de sincronización establecido en NO y la oportunidad y el contacto no tenían un filtro de sincronización, no se generaba el registro de creación para el contacto y la oportunidad cuando se clasificaba el posible cliente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">29/3/16</td> 
   <td>Corrección de errores: Se registró un evento de asignación cuando se desactivó el filtro de sincronización.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Corrección de errores: El cliente no pudo crear un posible cliente en CRM porque el usuario de inicio de sesión no tenía permiso de configuración de Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">18/1/16</td> 
   <td colspan="1">Corrección de errores: Se han creado límites de acceso para usuarios normales de Dynamics para solucionar problemas de seguridad.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">30/12/15</td> 
   <td>Corrección de errores: Las actualizaciones en Dynamics no se sincronizaban con Marketo para ver los pasos y las imágenes.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">12/11/15</td> 
   <td colspan="1">Corrección de errores: Los registros de posibles clientes se sincronizaban con Marketo cuando el filtro de sincronización estaba establecido en false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
[Descargar la solución de administración de posibles clientes de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)>
>
