---
description: Acceso a información de ventas - Documentos de Marketo - Documentación del producto
title: Eliminar acceso a información de ventas
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Eliminar acceso a información de ventas {#remove-sales-insight-access}

Siga estos pasos para eliminar el acceso a las funciones de Información sobre ventas en Salesforce. Aplicable a Salesforce Classic y Lightning.

## Información general {#overview}

Se requiere permiso para acceder a los objetos mencionados a continuación, a las clases de Apex y a las páginas de visualforce para acceder a todas las funciones de Sales Insight. Si los elimina, se eliminará el acceso a la perspectiva de ventas.

**Configuración de objeto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBestCache</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>Resultados más probables Ver detalles</td> 
   <td>Leer, Crear, Editar, Eliminar, Ver todo, Modificar todo</td> 
  </tr> 
  <tr> 
   <td>Vistas de resultados más probables</td> 
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
   <td>Configuración de Marketo Sales Insight</td> 
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

## Eliminación del acceso a Sales Insight {#removing-access-to-sales-insight}

1. Inicie sesión en su cuenta de Salesforce.

1. Clic **Configurar**.

   ![](assets/remove-sales-insight-access-1.png)

1. En Administrador, haga clic en **Administrar usuarios**, entonces **Perfiles**.

1. Haga clic en el perfil que desea actualizar y, a continuación, **Editar**.

1. Desplácese hacia abajo hasta &quot;Configuración de ficha personalizada&quot; en Configuración de ficha.

1. Seleccione la opción &quot;Pestaña oculta&quot; en la lista desplegable de la Configuración de perspectiva de ventas de Marketo y la Bandeja de salida de ventas de MSI Marketo.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Desplácese hacia abajo hasta &quot;Permisos de objeto personalizados&quot;.

1. Elimine el acceso de &quot;Leer, Crear, Editar, Eliminar&quot; de los siguientes objetos:

   * BestBestCache
   * Resultados más probables Ver detalles
   * Vistas de resultados más probables
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Configuración de Marketo Sales Insight
   * ScoringCache
   * Valores
   * WebActivityCache

1. Desplácese hacia abajo hasta la sección &quot;Acceso a clase Apex habilitado&quot;. Clic **Editar**.

1. En la sección &quot;Clases Apex habilitadas&quot;, seleccione todas las clases que comienzan por &quot;mkto_si&quot;. Esto debería sumar 159 clases.

1. Clic **Eliminar**, entonces **Guardar**.

   ![](assets/remove-sales-insight-access-4.png)

1. Desplácese hacia abajo hasta la sección &quot;Acceso a la página de VisualForce habilitado&quot;. Clic **Editar**.

1. En la sección &quot;Páginas Visualforce habilitadas&quot;, seleccione todas las páginas que empiecen por &quot;mkto_si&quot;. Esto debería sumar 64 páginas.

1. Clic **Eliminar**, entonces **Guardar**.

   ![](assets/remove-sales-insight-access-5.png)

1. Desplácese hacia abajo hasta la sección &quot;Acceso a definiciones de configuración personalizadas habilitadas&quot;. Clic **Editar**.

1. Seleccione &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; y &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Clic **Eliminar**, entonces **Guardar**.

   ![](assets/remove-sales-insight-access-6.png)

¡Eso es todo! Se ha eliminado correctamente el acceso a la información de ventas. Repita los mismos pasos para cualquier otro perfil para el que desee eliminar el acceso.
