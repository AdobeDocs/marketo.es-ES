---
unique-page-id: 14745823
description: 'Creación de reglas de flujo de trabajo en Salesforce: documentos de Marketo: documentación del producto'
title: Creación de reglas de flujo de trabajo en Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Creación de reglas de flujo de trabajo en Salesforce {#creating-workflow-rules-in-salesforce}

Al usar Marketo Sales Insight (MSI) y Marketo Sales Connect (MSC) en paralelo, la función Más probable de MSI en Salesforce no se actualizará. Todas las demás funciones de MSI funcionan de la forma habitual (ver momentos interesantes en el iFrame, enviar correos electrónicos, añadir a campañas, etc.). Este artículo ofrece una solución para que los resultados más probables vuelvan a funcionar.

>[!NOTE]
>
>Esto solo afecta a los clientes que usan **tanto** MSI como MSE, y que desean usar la característica Lo mejor en MSI. Si no necesita ni utiliza los resultados más probables, puede hacer caso omiso de.

## Introducción {#getting-started}

La solución incluye la creación de nuevas reglas de flujo de trabajo para copiar valores de los nuevos campos MSE en los antiguos campos MSI. Deberá crear cuatro reglas de flujo de trabajo para el objeto Contact y las mismas cuatro reglas de flujo de trabajo para el objeto Lead en su propia instancia de Salesforce. Esto puede requerir que tenga derechos de administración de CRM (según su función y configuración en CRM).

A continuación se muestran los nombres recomendados de las reglas de flujo de trabajo y la descripción de cada una. Se aplican al objeto Contacto y posible cliente:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Actualizar Campo Desc De Momento Interesante</td> 
   <td><p>Copiar de: Última descripción de Marketo Engagement<br>Copiar en: Último momento interesante Desc</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar campo de tipo de momento interesante</td> 
   <td><p>Copiar de: Último tipo de participación de Marketo<br>Copiar en: Último tipo de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar campo de Source de momento interesante</td> 
   <td><p>Copiar de: Último Source de Marketo Engagement<br>Copiar en: Último momento interesante Source</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar campo Fecha de momento interesante</td> 
   <td><p>Copiar de: Fecha de la última participación de Marketo<br>Copiar a: Fecha del último momento interesante</p></td> 
  </tr> 
 </tbody> 
</table>

## Instrucciones {#instructions}

1. Después de hacer clic en **Configuración**, busque **Flujo de trabajo** y seleccione **Reglas de flujo de trabajo**.

   ![](assets/one-1.png)

1. Seleccione **Nueva regla**.

   ![](assets/two-1.png)

1. Haga clic en el menú desplegable Objeto, seleccione **Posible cliente** y, a continuación, haga clic en **Siguiente**.

   ![](assets/three-1.png)

1. Introduzca &quot;Update Interested Moment Desc Field&quot; en el nombre de la regla. Seleccione el botón de opción **creado y cada vez que se edite**. En la lista desplegable Criterios de regla, seleccione **formula se evalúa como true**. Busque y seleccione la función ISCHANGED. A continuación, resalte el valor de campo predeterminado y haga clic en **Insertar campo**.

   ![](assets/four-1.png)

1. En el elemento emergente &quot;Insertar campo&quot;, elija **Último descripción de la participación de Marketo** y haga clic en **Insertar**.

   ![](assets/five-1.png)

1. Haga clic en **Guardar y siguiente**.

   ![](assets/6.png)

1. En el menú desplegable Agregar acción de flujo de trabajo, seleccione **Nueva actualización de campo**.

   ![](assets/seven.png)

1. En el campo Nombre, introduzca &quot;Actualizar campo de descripción de momento interesante&quot; (Unique Name se generará automáticamente). En el menú desplegable Campo para actualizar, elija **Último momento interesante Desc**. Seleccione el botón de opción **Usar una fórmula para establecer un nuevo valor** y, a continuación, haga clic en **Mostrar editor de fórmulas**.

   ![](assets/eight.png)

1. Haga clic en el botón **Insertar campo**.

   ![](assets/9a.png)

1. Seleccione **Última descripción de Marketo Engagement** y haga clic en **Insertar**. En la página siguiente, haz clic en **Guardar**.

   ![](assets/nine.png)

1. Haga clic en **Listo**.

   ![](assets/twelve.png)

1. Haga clic en **Activar** para activar la regla de flujo de trabajo.

   ![](assets/thirteen.png)

   Después del último paso, puede optar por clonar la regla de flujo de trabajo para los demás campos enumerados en la sección Introducción: Desc, Type, Source, Date. Después de completar las cuatro reglas de flujo de trabajo en el objeto Contact, repita lo mismo para el objeto Lead.
