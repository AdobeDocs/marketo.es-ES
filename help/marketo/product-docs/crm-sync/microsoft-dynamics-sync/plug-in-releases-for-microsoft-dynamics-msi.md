---
unique-page-id: 10099102
description: 'Versiones de complementos para Microsoft Dynamics MSI: documentos de Marketo, documentación del producto'
title: Versiones de complementos para Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 8%

---

# Versiones de complementos para Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

La primera vez que se sincroniza con Microsoft Dynamics, descarga e instala la versión más reciente de los complementos para Marketo Sales Insight (MSI). Marketo Engage actualiza periódicamente estos complementos para que pueda volver al mismo lugar donde desea descargar la nueva versión.

Si está utilizando la solución de sincronización de CRM nativa de Marketo con Dynamics, [descargar el complemento más reciente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Estas versiones funcionan tanto para las versiones locales como en línea de Dynamics.

## Actualizar la solución MSI {#upgrading-your-msi-solution}

1. Importar la versión más reciente de la solución _sobre la versión existente_ de su Dynamics CRM pulsando la tecla **[!UICONTROL Importar]** botón en Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Ejemplo: si su Dynamics CRM tiene la versión 2.0.0.20 y la última versión es 2.0.0.21, debe importar _sobre_ versión 2.0.0.20.

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Seleccionar **[!UICONTROL Fase de actualización]** y **[!UICONTROL Mantener personalizaciones]**, luego haga clic en **[!UICONTROL Importar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Después de una importación correcta, verá dos soluciones MSI: MarketoSalesInsight y MarketoSalesInsight_Upgrade. Seleccione la solución más antigua y haga clic en Aplicar actualización de solución.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

¡Y eso es todo! Después de la actualización solo verá una solución MSI.

## Actualizaciones de versión {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Fecha de lanzamiento</th> 
   <th colspan="1">Versión</th> 
   <th colspan="1">Notas</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Diseño de cuenta para perspectivas: momentos interesantes, cambios de puntuación, actividades web, actividades de correo electrónico</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Puntuación de adopción del programa para enviar correo electrónico</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">Métricas de puntuación de adopción de productos, nuevo panel global (actividad web, correo electrónico, resultados más probables)</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">Quitar la auditoría automática habilitada y los cambios de documentación en la solución MSI</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Corrección de errores: Asignar acceso a los campos de configuración de la API de MSI para los usuarios con la función de perspectiva de ventas</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Corrección de errores: Agregar un mensaje de validación para registros no sincronizados</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Corrección de errores: Para ocultar la contraseña secreta MSI en la configuración de la API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Corrección de errores: Para cambiar la validación del ID de rol MSI para mostrar los botones MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Corrección de errores: Mostrar el campo de propietario y hacer que los campos no sean obligatorios</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Corrección de errores: Eliminando la dependencia de vínculos de la configuración del mapa del sitio MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
