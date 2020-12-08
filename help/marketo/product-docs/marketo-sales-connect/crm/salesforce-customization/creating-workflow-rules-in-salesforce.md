---
unique-page-id: 14745823
description: Creación de reglas de flujo de trabajo en Salesforce - Documentos de marketing - Documentación del producto
title: Creación de reglas de flujo de trabajo en Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Creación de reglas de flujo de trabajo en Salesforce {#creating-workflow-rules-in-salesforce}

Cuando se utiliza Marketing to Sales Insight (MSI) y Marketing TO Sales Connect (MSC) en paralelo, la función MSI Best Bets de Salesforce no se actualizará. Todas las demás funciones de MSI funcionan como de costumbre (ver momentos interesantes en el iFrame, enviar correos electrónicos, agregar campañas, etc.). Este artículo oferta una solución alternativa para que Best Bets funcione de nuevo.

>[!NOTE]
>
>Esto solo afecta a los clientes que utilizan **tanto** MSI como MSE y que desean utilizar la función Best Bets en MSI. Si no necesita o no utiliza Best Bets, puede hacer caso omiso.

## Introducción {#getting-started}

La solución consiste en crear nuevas reglas de flujo de trabajo para copiar valores de nuevos campos MSE en los campos MSI antiguos. Deberá crear cuatro reglas de flujo de trabajo para el objeto Contact y las mismas cuatro reglas de flujo de trabajo para el objeto Lead en su propia instancia de Salesforce. Esto puede requerir que tenga derechos de administrador de CRM (según su función y configuración en el CRM).

A continuación se indican los nombres recomendados de las reglas de flujo de trabajo y la descripción de cada una de ellas. Se aplican al objeto Contacto y posible cliente:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Actualizar el campo Desc de momento interesante</td> 
   <td><p>Copiar de: Última participación de marketing<br>DescCopy a: Último momento interesante Desc</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar el campo Tipo de momento interesante</td> 
   <td><p>Copiar de: Último<br>tipo de compromiso de marketingCopiar en: Último tipo de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar el campo Origen de momento interesante</td> 
   <td><p>Copiar de: Última<br>copia de origen de compromiso de marketing en: Última fuente de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td>Actualizar fecha de momento interesante, campo</td> 
   <td><p>Copiar de: Última<br>fecha de compromiso de marketingCopiar en: Fecha del último momento interesante</p></td> 
  </tr> 
 </tbody> 
</table>

## Instrucciones {#instructions}

1. Después de hacer clic en **Configuración**, busque **Flujo de trabajo** y seleccione Reglas **de flujo de trabajo**.

   ![](assets/one-1.png)

1. Seleccione **Nueva regla**.

   ![](assets/two-1.png)

1. Haga clic en la lista desplegable Objeto, seleccione **Posible cliente** y, a continuación, haga clic en **Siguiente**.

   ![](assets/three-1.png)

1. Escriba &quot;Actualizar el campo Desc del momento interesante&quot; como nombre de regla. Seleccione el botón de radio **creado y cada vez que se edite**. En la lista desplegable Criterios de regla, la **fórmula seleccionada se evalúa como verdadera**. Busque y seleccione la función ISCHANGED. A continuación, resalte el valor de campo predeterminado y haga clic en **Insertar campo**.

   ![](assets/four-1.png)

1. En la ventana emergente &quot;Insertar campo&quot;, elija **Último registro de participación de marketing** y haga clic en **Insertar**.

   ![](assets/five-1.png)

1. Haga clic en **Guardar y siguiente**.

   ![](assets/6.png)

1. En la lista desplegable Añadir acción de flujo de trabajo, seleccione **Nueva actualización** de campo.

   ![](assets/seven.png)

1. En el campo Nombre, escriba &quot;Actualizar el campo Desc de momento interesante&quot; (el nombre único se generará automáticamente). En la lista desplegable Campo que actualizar, elija **Último desfase interesante**. Seleccione el botón de opción **Usar una fórmula para definir un nuevo valor** y, a continuación, haga clic en **Mostrar editor** de fórmulas.

   ![](assets/eight.png)

1. Haga clic en el botón **Insertar campo** .

   ![](assets/9a.png)

1. Seleccione **Último índice de participación de marketing** y haga clic en **Insertar**. En la página siguiente, haga clic en **Guardar**.

   ![](assets/nine.png)

1. Haga clic en **Finalizado**.

   ![](assets/twelve.png)

1. Haga clic en **Activar** para activar la regla de flujo de trabajo.

   ![](assets/thirteen.png)

   Después del último paso, puede clonar la regla de flujo de trabajo para los demás campos que se enumeran en la sección Introducción: Desc, Tipo, Origen, Fecha. Después de completar las cuatro reglas de flujo de trabajo en el objeto Contact, repita lo mismo para el objeto Lead.

