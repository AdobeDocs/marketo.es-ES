---
description: Añadir conjunto de permisos de información de ventas - Documentos de Marketo - Documentación del producto
title: Agregar conjunto de permisos de perspectiva de ventas
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Agregar conjunto de permisos de perspectiva de ventas {#add-sales-insight-permission-set}

Siga estos pasos para agregar acceso a las funciones de Información de ventas en Salesforce. Aplicable a Salesforce Classic y Lighening

>[!PREREQUISITES]
>
>[Actualice el paquete de Sales Insight Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} a la versión 1.8000 o superior de para utilizar esta función.

>[!IMPORTANT]
>
>Si anteriormente ha proporcionado acceso a Sales Insight a todos los perfiles o ha implementado Sales Insight para todos los usuarios, debe [eliminar acceso de nivel de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para utilizar este conjunto de permisos.

## Información general {#overview}

El permiso &quot;Aplicación de Marketo&quot; forma parte del paquete de Sales Insight Salesforce. Incluye acceso a los objetos mencionados a continuación, clases de Apex y páginas de visualforce. Son necesarios para acceder a todas las funciones de Información sobre ventas.

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

## Adición del conjunto de permisos de la aplicación Marketo a los usuarios {#adding-marketo-app-permission-set-to-users}

1. Inicie sesión en su cuenta de Salesforce.

1. Clic **Configurar**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. En Administrador, haga clic en para mostrar **Administrar usuarios**, entonces **Usuarios**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. En Todos los usuarios, seleccione el usuario al que desee proporcionar acceso y, a continuación, haga clic en **Asignaciones de conjuntos de permisos**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Clic **Editar asignaciones**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Seleccionar **Acceso a aplicaciones Marketo** en los conjuntos de permisos disponibles, **Añadir**. Clic **Guardar**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Ahora, cuando se desplace hacia abajo por la página Detalles del usuario, verá &quot;Acceso a la aplicación de Marketo&quot; en Asignaciones de conjuntos de permisos.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Los usuarios que no tengan acceso a Sales Insight verán este mensaje: &quot;No cuenta con privilegios suficientes para acceder a esta pestaña&quot;.

¡Eso es todo! Se ha añadido correctamente el acceso a Información de ventas. Repita los mismos pasos para cualquier otro perfil al que desee agregar acceso.
