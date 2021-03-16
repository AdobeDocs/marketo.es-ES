---
unique-page-id: 15695924
description: Clasificación y ajuste de perfiles de cuenta - Documentos de Marketo - Documentación del producto
title: Clasificación y ajuste de perfiles de cuenta
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Clasificación y ajuste de perfiles de cuenta {#account-profiling-ranking-and-tuning}

El perfil de cuenta identifica su perfil de cliente ideal (ICP), clasifica a las empresas en la base de datos en función del PCI y agrega datos del indicador ICP a cuentas promocionadas como cuentas con nombre.

## Resultados del modelo {#model-results}

Los resultados muestran todas sus cuentas conocidas desglosadas por grado. A es el grado más alto, D es el más bajo.

![](assets/results.png)

Aunque es opcional, se recomienda seleccionar la casilla Promocionar automáticamente , ya que le ahorrará un montón de tiempo. Sin embargo, si desea navegar por cada cuenta y [agregarla manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), simplemente deje la casilla sin marcar.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Clasificación</strong></td> 
   <td> 
    <div>
      Clasificación de cuentas basada en el perfil de cliente ideal. A es el mejor ajuste, D es el menos adecuado. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Tendencia</strong></td> 
   <td> 
    <div>
      Aumento estimado de la tasa de conversión en comparación con una selección de cuentas no basada en el PCI. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Cuentas (%)</strong></td> 
   <td> 
    <div>
      Porcentaje de cuentas en la entrada del modelo que tienen esta clasificación. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% de base modelo</strong></td> 
   <td> 
    <div>
      Porcentaje de cuentas modelo que tienen esta clasificación. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Ajuste de modelo {#model-tuning}

En la ficha Modelo, haga clic en el botón Ajustar modelo.

![](assets/two.png)

Hay varias pestañas entre las que elegir, lo que permite una personalización detallada.

![](assets/tuning-page.png)

**Categorías de indicadores**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Cumplimiento</strong></td> 
   <td> 
    <div>
      Certificaciones, puestos relacionados con el cumplimiento/contratación. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Operaciones</strong></td> 
   <td> 
    <div>
      Puestos/contratación relacionados con las operaciones. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      Software HR o Payroll, puestos/contratación relacionados con HR.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ingeniería</strong></td> 
   <td> 
    <div>
      Tecnologías, marcos, puestos/contratación relacionados con la ingeniería. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ventas</strong></td> 
   <td> 
    <div>
      Soluciones y software para ventas, posiciones/contratación relacionadas con ventas. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intención</strong></td> 
   <td> 
    <div>
      Indicadores de intención. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Soluciones de hardware y software, tecnologías, posiciones/contratación relacionadas con TI.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanzas</strong></td> 
   <td> 
    <div>
      Programas informáticos financieros, puestos relacionados con las finanzas/contratación. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Tecnologías de marketing y software, puestos/contratación relacionados con el marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Empresa</strong></td> 
   <td> 
    <div>
      Listas de Forbes o Inc o sociedades de negocios. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Experiencia del cliente y relaciones</strong></td> 
   <td> 
    <div>
      Posiciones/contratación de éxito del cliente y relaciones con el cliente.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Pase el ratón sobre la información del objeto para ver una descripción de cada columna.

![](assets/tool-tip.png)

Haga clic en la lista desplegable Agregar indicador ICP para insertar indicadores adicionales en el modelo.

![](assets/add-icp.png)

Si activa la casilla Exportar, podrá ver el indicador ICP en la página de detalles de la cuenta con nombre, así como utilizar el indicador ICP seleccionado como restricciones en [filtros de cuenta con nombre](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Los indicadores ICP se incluyen como restricciones en los filtros y Déclencheur **Member of Named Account**.

Ponderación del indicador es lo que controla el nivel de importancia que cada indicador recibe en su modelo.

![](assets/weightage.png)

Haga clic en Actualizar modelo para que los cambios surtan efecto.

![](assets/refresh-button.png)

Cuando haya terminado de ajustar el modelo (después de actualizarlo), vuelva a la pestaña Resultados del modelo y haga clic en **Guardar y aplicar clasificaciones**.

![](assets/ranks.png)
