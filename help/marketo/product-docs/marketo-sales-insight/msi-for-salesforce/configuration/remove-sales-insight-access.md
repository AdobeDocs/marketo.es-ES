---
description: Acceso a Insight de ventas - Documentos de Marketo - Documentación del producto
title: Eliminar acceso de Insight de ventas
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 2%

---

# Eliminar el acceso de [!DNL Sales Insight] {#remove-sales-insight-access}

Siga estos pasos para quitar el acceso a las características de [!DNL Sales Insight] en [!DNL Salesforce]. Aplicable a [!DNL Salesforce] Classic y Lightning.

## Información general {#overview}

Se requiere permiso para acceder a los objetos mencionados abajo, las clases Apex y las páginas visualforce para acceder a todas las características de [!DNL Sales Insight]. Si elimina estos elementos, se eliminará el acceso a [!DNL Sales Insight].

**Configuración del objeto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBestCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Ver detalles</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Vistas</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>[!DNL Marketo Sales Insight] Configuración</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>Valores</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
 </tbody> 
</table>

* Acceso a clases Apex: 159 clases Apex que comienzan con &quot;mkto_si&quot;
* Acceso a la página de Visualforce: 64 páginas de Visualforce que comienzan con &quot;mkto_si&quot;
* Definiciones de ajustes personalizados: Configuración de mkto_si.Marketo y Preferencias de mkto_si.User

## Quitando acceso a [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Inicie sesión en su cuenta de [!DNL Salesforce].

1. Haga clic en **[!UICONTROL Configuración]**.

   ![](assets/remove-sales-insight-access-1.png)

1. En [!UICONTROL Administrador], haga clic en **[!UICONTROL Administrar usuarios]** y luego en **[!UICONTROL Perfiles]**.

1. Haz clic en el perfil que deseas actualizar y luego **[!UICONTROL Editar]**.

1. Desplácese hacia abajo hasta &quot;[!UICONTROL Configuración de ficha personalizada]&quot; en [!UICONTROL Configuración de ficha].

1. Seleccione la opción &quot;[!UICONTROL Tab Hidden]&quot; en la lista desplegable para la bandeja de salida [!DNL Marketo Sales Insight] y MSI [!DNL Marketo Sales].

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Desplácese hacia abajo hasta &quot;[!UICONTROL Permisos de objetos personalizados]&quot;.

1. Elimine el acceso de &quot;Leer, Crear, Editar, Eliminar&quot; de los siguientes objetos:

   * BestBestCache
   * [!DNL Best Bets] Ver detalles
   * [!DNL Best Bets] vistas
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Configuración de [!DNL Marketo Sales Insight]
   * ScoringCache
   * Valores
   * WebActivityCache

1. Desplácese hacia abajo hasta la sección &quot;[!UICONTROL Acceso habilitado a la clase Apex]&quot;. Haga clic en **[!UICONTROL Editar]**.

1. En la sección &quot;[!UICONTROL Clases Apex habilitadas]&quot;, seleccione todas las clases que empiecen por &quot;mkto_si&quot;. Esto debería sumar 159 clases.

1. Haz clic en **[!UICONTROL Quitar]** y después en **[!UICONTROL Guardar]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Desplácese hacia abajo hasta la sección &quot;[!UICONTROL Acceso habilitado a la página de VisualForce]&quot;. Haga clic en **[!UICONTROL Editar]**.

1. En la sección &quot;[!UICONTROL Páginas de Visualforce habilitadas]&quot;, seleccione todas las páginas que comiencen por &quot;mkto_si&quot;. Esto debería sumar 64 páginas.

1. Haz clic en **[!UICONTROL Quitar]** y después en **[!UICONTROL Guardar]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Desplácese hacia abajo hasta la sección &quot;[!UICONTROL Acceso a definiciones de configuración personalizadas habilitadas]&quot;. Haga clic en **[!UICONTROL Editar]**.

1. Seleccione &quot;Configuración de Marketo Sales Insight.mkto_si.Marketo&quot; y &quot;Preferencias de usuario de Marketo Sales Insight.mkto_si.User&quot;.

1. Haz clic en **[!UICONTROL Quitar]** y después en **[!UICONTROL Guardar]**.

   ![](assets/remove-sales-insight-access-6.png)

¡Eso es todo! Ha eliminado correctamente el acceso de [!DNL Sales Insight]. Repita los mismos pasos para cualquier otro perfil para el que desee eliminar el acceso.
