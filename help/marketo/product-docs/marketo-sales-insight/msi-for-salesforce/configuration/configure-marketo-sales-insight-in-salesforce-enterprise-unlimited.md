---
unique-page-id: 2360368
description: Configurar la perspectiva de ventas de marketing en Salesforce Enterprise/Unlimited - Documentos de marketing - Documentación del producto
title: Configurar la perspectiva de ventas de marketing en Salesforce Enterprise/Unlimited
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---


# Configurar la perspectiva de ventas de marketing en Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

A continuación se indican los pasos que debe seguir para configurar la perspectiva de ventas de marketing en las ediciones Enterprise/Unlimited de Salesforce. Empecemos.

>[!PREREQUISITES]
>
>* [Configurar la sincronización de campos de Marketo en Salesforce Enterprise/Unlimited Edition](https://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [Instalación del paquete de perspectiva de ventas de marketing en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**Se requieren permisos de administración**

## Configurar la perspectiva de ventas en Marketing {#configure-sales-insight-in-marketo}

1. Abra una nueva ventana del explorador para obtener las credenciales de perspectiva de ventas de marketing de su cuenta de Marketing to.

1. Vaya al área Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Introduzca una clave secreta de API de su elección y haga clic en **Guardar**. NO utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La clave secreta de API es como una contraseña para su organización y debe ser segura.

1. Haga clic en **Vista** en el panel Configuración de la API restante para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verá una ventana emergente de confirmación. Haga clic en **Aceptar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Escriba el nombre del sitio remoto (puede ser algo así como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es la URL del host de marketing del panel Configuración de la API de jabón en Marketing. Haga clic en **Guardar**. Ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Vuelva a hacer clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Escriba el nombre del sitio remoto (puede ser algo así como &quot;MarketoRestAPI&quot;). Introduzca la dirección URL del sitio remoto, que es la dirección URL de la API desde el panel Configuración de la API de reposo en MarketingTo. Haga clic en **Guardar**. Ha creado la configuración del sitio remoto para la API de descanso.

## Configurar la perspectiva de ventas de marketing {#set-up-marketo-sales-insight}

1. Inicie sesión en la instancia de Marketing y haga clic en **Administración**.

   ![](assets/login-admin.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Escriba una **Clave secreta de API** y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

1. Vuelva a Salesforce y haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;sitio remoto&quot; y haga clic en **Configuración de sitio remoto** en **Controles de seguridad**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Escriba **Nombre del sitio remoto** y **Dirección URL del sitio remoto**, luego haga clic en **Guardar**.

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >Usted elige su **Nombre del sitio remoto** (la API de marketing se usa aquí). La **URL del sitio remoto** se encuentra en el campo Host de marketing del cuadro de diálogo Editar configuración de API del paso 4.

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;page layout&quot; y seleccione el **Diseño de página** en **Posibles clientes**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Haga clic en **Páginas de VisualForce** a la izquierda. Arrastre **Sección** al diseño debajo de la sección Vínculos personalizados.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Perspectiva de ventas de marketing&quot; como **Nombre de sección**. Seleccione **1-Columna** y haga clic en **Aceptar**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastre y suelte **Posible cliente** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >El nombre de este cuadro cambiará según el tipo de objeto. Por ejemplo, si está modificando el diseño de página para Contactos, dirá Contacto.

1. Haga clic con el doble en el bloque **Posible cliente** que acaba de agregar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite la altura a **450** píxeles y haga clic en **Aceptar**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Se recomienda una altura de 410 píxeles para los objetos Cuentas y oportunidades.

1. Haga clic en **Campos** a la izquierda. A continuación, busque y arrastre la etiqueta **Participación** al diseño **Perspectiva de ventas de marketing**.

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Repita también el paso anterior para estos campos.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Participación</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de puntuación relativo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgencia</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Fecha del último momento interesante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último momento interesante Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Última fuente de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último tipo de momento interesante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Haga clic en **Guardar** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita este proceso para agregar secciones de página de VisualForce y campos de perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.

1. Repita los pasos del 5 al 7 para agregar secciones de página de Visualforce para Contacto, Cuenta y Oportunidad. A continuación, repita los pasos del 8 al 10 para agregar campos de perspectiva de ventas para **Contacto**. Asegúrese de guardar después de realizar cualquier cambio.

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de marketing deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Así es como.

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Campos** en **Posibles clientes**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Haga clic en **Asignar campos de posibles clientes**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleccione **Contact.Engagement** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita y asigne también estos campos.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Campo personalizado Persona de marketing</th> 
   <th colspan="1" rowspan="1">Campo personalizado de contacto de Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Participación</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de puntuación relativo</p></td> 
   <td colspan="1" rowspan="1"><p>Valor de puntuación de contacto.Relativo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgencia</p></td> 
   <td colspan="1" rowspan="1"><p>Valor de Contact.Urgency</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Fecha del último momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Última fecha de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último momento interesante Desc</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Último momento interesante Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Última fuente de momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Última fuente de momento interesante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último tipo de momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Último tipo de momento interesante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Haga clic en **Guardar** cuando haya terminado.

## Configuración de perspectiva de ventas de marketing {#marketo-sales-insight-config}

1. Haga clic en **+** y, a continuación, seleccione **Configuración de perspectiva de ventas de marketing**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Marque **Habilitar API de marketing**. A continuación, rellene la [información de configuración de API en Administración de mercadotecnia](#set-up-marketo-sales-insight). Haga clic en **Guardar cambios** cuando haya terminado.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Si falla la prueba de diagnóstico, es posible que tenga que [agregar más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115).

¡Y eso es todo! Debería poder ver los campos de perspectiva de ventas de marketing para posibles clientes, contactos, cuentas y oportunidades.

![](assets/twenty-six.png)

>[!NOTE]
>
>En el caso de las cuentas, la perspectiva de ventas incluirá todos los correos electrónicos, pero sólo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

## Acceder a la perspectiva de ventas de marketing {#access-marketo-sales-insight}

1. En Salesforce, haga clic en **+** al final de la barra de fichas y haga clic en **Configuración de perspectiva de ventas de marketing**.

1. Seleccione la casilla **Habilitar API de marketing**.

1. Copie las credenciales del panel API de Soap en la página de administración de perspectiva de ventas de Marketing Cloud y péguelas en la sección API de Soap de la página de configuración de la perspectiva de ventas de Salesforce.

1. Copie las credenciales del panel API de Rest en la página de administración de perspectiva de ventas de Marketing Cloud y péguelas en la sección API de Rest de la página de configuración de Perspectiva de ventas de Salesforce.

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y mejores apuestas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Añadir la ficha y los botones de perspectiva de ventas de marketing a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

