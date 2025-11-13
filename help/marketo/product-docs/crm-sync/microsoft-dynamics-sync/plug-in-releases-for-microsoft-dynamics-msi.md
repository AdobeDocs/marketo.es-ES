---
unique-page-id: 10099102
description: Versiones de complementos para  [!DNL Microsoft Dynamics] MSI - Documentos de Marketo - Documentación del producto
title: Versiones de complementos para  [!DNL Microsoft Dynamics] MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6fb25aab33dfc0f6792950a7d5d802a9e4be8303
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Versiones de complemento para [!DNL Microsoft Dynamics] MSI {#plug-in-releases-for-microsoft-dynamics-msi}

La primera vez que se sincroniza con [!DNL Microsoft Dynamics], descarga e instala la versión más reciente de los complementos para Marketo Sales Insight (MSI). Marketo actualiza periódicamente estos complementos para que pueda volver al mismo lugar donde desea descargar la nueva versión.

Si está usando la solución nativa de sincronización CRM de Marketo para [!DNL Dynamics], [descargue el complemento más reciente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} correspondiente a su versión de [!DNL Dynamics]. Para aquellos que tienen una sincronización personalizada y han comprado Marketo Sales Insight, el paquete [está aquí](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Estas versiones funcionan tanto para las versiones locales como en línea de [!DNL Dynamics].

## Actualizar la solución MSI {#upgrading-your-msi-solution}

1. Importe la última versión de la solución _sobre la versión existente_ de su CRM [!DNL Dynamics] presionando el botón **[!UICONTROL Importar]** en [!DNL Dynamics].

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Ejemplo: si su CRM [!DNL Dynamics] tiene la versión 2.0.0.20 y la última versión es 2.0.0.21, importaría _más de_ la versión 2.0.0.20.

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Seleccione **[!UICONTROL Fase para la actualización]** y **[!UICONTROL Mantener personalizaciones]**; a continuación, haga clic en **[!UICONTROL Importar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Después de una importación correcta, verá dos soluciones MSI: MarketoSalesInsight y MarketoSalesInsight_Upgrade. Seleccione la solución más antigua y haga clic en Aplicar actualización de solución.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

¡Y eso es todo! Después de la actualización solo verá una solución MSI.

## Actualizaciones de versión {#version-updates}

<table>
 <tbody>
  <tr>
   <th>Fecha de la versión</th>
   <th>Versión</th>
   <th>Notas</th>
  </tr>
  <tr>
   <td>02/14/24</td>
   <td>2.00.31</td>
   <td>Cambios en la paginación de la actividad web anónima.
   <p>
   Cifrar información de clave secreta de la vista de usuario. La contraseña debe cambiarse después de importar el nuevo paquete para que se produzca el cifrado.
   <p>
   Al actualizar el complemento MSI para Dynamics, se recomienda actualizar tanto la clave secreta de la API de SOAP como las credenciales MSI como una forma de actualización para garantizar que no se tengan permisos de acceso con el nuevo paquete instalado.</td>
  </tr>
  <tr>
   <td>10/18/23</td>
   <td>2.00.30</td>
   <td>Consolidar el registro de errores de MSI y eliminar las notificaciones de información para que no se muestren en la entidad de error de Marketo.</td>
  </tr>
  <tr>
   <td>05/19/23</td>
   <td>2.00.29</td>
   <td>Se han corregido los problemas de paginación de Actividad web y Momentos interesantes en el panel global.</td>
  </tr>
  <tr>
   <td>23/03/23</td>
   <td>2.00.28</td>
   <td>Se creó un <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">nuevo paquete</a> para MSI para conexiones no nativas con CRM.</td>
  </tr>
  <tr>
   <td>02/03/22</td>
   <td>2.0.0.27</td>
   <td>Diseño de cuenta para perspectivas: momentos interesantes, cambios de puntuación, actividades web, actividades de correo electrónico.</td>
  </tr>
  <tr>
   <td>01/05/22</td>
   <td>2.0.0.26</td>
   <td>Puntuación de adopción del programa para enviar correo electrónico.</td>
  </tr>
  <tr>
   <td>28/10/21</td>
   <td>2.0.0.25</td>
   <td>Métricas de puntuación de adopción de productos, nuevo panel global (actividad web, correo electrónico, resultados más probables).</td>
  </tr>
  <tr>
   <td>02/10/21</td>
   <td>2.0.0.22</td>
   <td>Quitar la auditoría automática habilitada y los cambios de documentación en la solución MSI.</td>
  </tr>
  <tr>
   <td>10/01/20</td>
   <td>2.0.0.21</td>
   <td>Corrección de errores: Asignar acceso a los campos de configuración de la API MSI a los usuarios con el rol de Insight de ventas.</td>
  </tr>
  <tr>
   <td>20/07/20</td>
   <td>2.0.0.20</td>
   <td>Corrección de errores: Agregue un mensaje de validación para los registros no sincronizados.</td>
  </tr>
  <tr>
   <td>06/12/20</td>
   <td>2.0.0.19</td>
   <td>Corrección de errores: Para ocultar la contraseña secreta MSI en la configuración de la API de MSD.</td>
  </tr>
  <tr>
   <td>26/05/20</td>
   <td>2.0.0.18</td>
   <td>Corrección de errores: Para cambiar la validación del ID de rol MSI para mostrar los botones MSI.</td>
  </tr>
  <tr>
   <td>21/05/20</td>
   <td>2.0.0.17</td>
   <td>Corrección de errores: Mostrar el campo de propietario y hacer que los campos no sean obligatorios.</td>
  </tr>
  <tr>
   <td>28/04/20</td>
   <td>2.0.0.16</td>
   <td>Corrección de errores: Eliminando la dependencia de vínculo de la configuración del mapa del sitio de MSD CRM.</td>
  </tr>
 </tbody>
</table>
