---
unique-page-id: 15695924
description: Clasificación y ajuste de perfiles de cuenta - Documentos de Marketo - Documentación del producto
title: Clasificación y ajuste de perfiles de cuenta
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 2%

---

# Clasificación y ajuste de perfiles de cuenta {#account-profiling-ranking-and-tuning}

La generación de perfiles de cuenta identifica su perfil de cliente ideal (ICP), clasifica las compañías de su base de datos según el ICP y agrega datos del indicador ICP a las cuentas promocionadas como [!UICONTROL cuentas con nombre].

>[!IMPORTANT]
>
>A partir de 2025, la generación de perfiles de cuenta ya no estará disponible para los nuevos usuarios. Seguirá funcionando para los usuarios existentes.

## Resultados del modelo {#model-results}

Los resultados muestran todas sus cuentas conocidas desglosadas por grado. A es el grado más alto, D es el más bajo.

![](assets/results.png)

Aunque es opcional, le recomendamos que seleccione la casilla Promocionar automáticamente, ya que le ahorrará mucho tiempo. Sin embargo, si desea revisar cada cuenta y [agregarlas manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), simplemente deje la casilla sin marcar.

<table> 
 <tbody> 
  <tr> 
   <td><strong><span class="uicontrol">Clasificación</span></strong></td> 
   <td> 
    <div>
      Clasificación de la cuenta basada en el perfil de cliente ideal. A es el mejor ajuste, D es el menos ajustado. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Propensión</span></strong></td> 
   <td> 
    <div>
      Aumento estimado de la tasa de conversión en comparación con una selección de cuentas no basada en ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Cuentas (%)</span></strong></td> 
   <td> 
    <div>
      Porcentaje de cuentas en la entrada del modelo que tienen esta clasificación. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">% de base de modelo</span></strong></td> 
   <td> 
    <div>
      Porcentaje de cuentas en base de modelo que tienen esta clasificación. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Ajuste de modelo {#model-tuning}

En la ficha Modelo, haga clic en el botón **[!UICONTROL Ajustar modelo]**.

![](assets/two.png)

Hay varias pestañas entre las que elegir, lo que permite una personalización en profundidad.

![](assets/tuning-page.png)

**Categorías de indicador**

<table> 
 <tbody> 
  <tr> 
   <td><strong><span class="uicontrol">Cumplimiento</span></strong></td> 
   <td> 
    <div>
      Certificaciones, puestos/contratación relacionados con el cumplimiento. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Operaciones</span></strong></td> 
   <td> 
    <div>
      Posiciones/contrataciones relacionadas con las operaciones. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">HR</span></strong></td> 
   <td> 
    <div>
      Software de RRHH o Nómina, puestos/contratación relacionados con RRHH.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Ingeniería</span></strong></td> 
   <td> 
    <div>
      Tecnologías, marcos, puestos/contratación relacionados con la ingeniería. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Ventas</span></strong></td> 
   <td> 
    <div>
      Soluciones y software para ventas, puestos/contratación relacionados con ventas. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Intención</span></strong></td> 
   <td> 
    <div>
      Indicadores de intención. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">IT</span></strong></td> 
   <td> 
    <div>
      Soluciones de hardware y software, tecnologías, puestos/contratación relacionados con TI.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Finanzas</span></strong></td> 
   <td> 
    <div>
      Software financiero, puestos/contratación relacionados con las finanzas. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Marketing</span></strong></td> 
   <td> 
    <div>
      Tecnologías de marketing y software, puestos/contratación relacionados con el marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Business</span></strong></td> 
   <td> 
    <div>
      Forbes o Inc listados o asociaciones de negocios. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">Experiencia del cliente y relaciones</span></strong></td> 
   <td> 
    <div>
      Éxito del cliente y relaciones con el cliente/contratación.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Pase el ratón sobre la información del objeto para ver una descripción de cada columna.

![](assets/tool-tip.png)

Haga clic en el menú desplegable [!UICONTROL Agregar indicador ICP] para insertar indicadores adicionales en el modelo.

![](assets/add-icp.png)

Marcar la casilla [!UICONTROL Export] le permite ver el indicador ICP en la página de detalles de [!UICONTROL Cuenta con nombre], así como usar el indicador ICP seleccionado como restricciones en [filtros de cuenta con nombre](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Los indicadores ICP se incluyen como restricciones en **[!UICONTROL Miembros de filtros y Déclencheur de la cuenta con nombre]**.

[!UICONTROL Peso del indicador] es lo que controla el nivel de importancia que cada indicador recibe en su modelo.

![](assets/weightage.png)

Haga clic en **[!UICONTROL Actualizar modelo]** para que los cambios surtan efecto.

![](assets/refresh-button.png)

Cuando haya terminado de ajustar el modelo (después de actualizarlo), vuelva a la ficha Resultados del modelo y haga clic en **[!UICONTROL Guardar y aplicar clasificaciones]**.

![](assets/ranks.png)
