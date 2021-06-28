---
unique-page-id: 2360368
description: Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited - Marketo Docs - Documentación del producto
title: Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: fbd8640d55a9a38936d060086f361b2281add47f
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 3%

---

# Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estos son los pasos que debe seguir para configurar Marketo Sales Insight en Salesforce Enterprise/Unlimited Editions. Empecemos.

>[!PREREQUISITES]
>
>* [Instalación del paquete de perspectivas de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
**Se requieren permisos de administrador**

## Configurar la perspectiva de ventas en Marketo {#configure-sales-insight-in-marketo}

1. Abra una nueva ventana del explorador para obtener las credenciales de Marketo Sales Insight de su cuenta de Marketo.

1. Vaya al área Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Escriba una clave secreta de API de su elección y haga clic en **Guardar**. NO use un signo &amp; en la clave secreta de API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   La clave secreta de API es como una contraseña para su organización y debe ser segura.

1. Haga clic en **Ver** en el panel Configuración de la API restante para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verá una ventana emergente de confirmación. Haga clic en **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración de sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de host de Marketo desde el panel Configuración de la API Soap en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Vuelva a hacer clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoRestAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de API del panel Configuración de la API de Rest en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Rest.

## Configurar Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Inicie sesión en la instancia de Marketo y haga clic en **Admin**.

   ![](assets/login-admin.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Introduzca una **Clave secreta de API** y haga clic en **Guardar**.

   >[!CAUTION]
   No use un signo &amp; en la clave secreta de API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

1. Vuelva a Salesforce y haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;sitio remoto&quot; y haga clic en **Configuración de sitio remoto** en **Controles de seguridad**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Introduzca **Remote Site Name** y **Remote Site URL** y, a continuación, haga clic en **Save**.

   ![](assets/remote-site.png)

   >[!NOTE]
   Usted elige su **Nombre del sitio remoto** (MarketoAPI se usa aquí). La **URL del sitio remoto** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API del paso 4.

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;page layout&quot; y seleccione el **Page Layout** en **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Haga clic en **Visualforce Pages** a la izquierda. Arrastre **Sección** al diseño debajo de la sección Vínculos personalizados .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Marketo Sales Insight&quot; como **Section Name**. Seleccione **1-Column** y haga clic en **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastre y suelte **Lead** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   El nombre de este cuadro cambiará según el tipo de objeto. Por ejemplo, si está modificando el diseño de página de Contactos, dirá Contacto.

1. Haga doble clic en el bloque **Lead** que acaba de añadir.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite la altura a **450** píxeles y haga clic en **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   Se recomienda una altura de 410 píxeles para los objetos Cuentas y oportunidades .

1. Haga clic en **Fields** a la izquierda. A continuación, busque y arrastre la etiqueta **Participación** al diseño **Perspectiva de ventas de Marketo** .

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Repita el paso anterior también para estos campos.

   <table> 
    <tbody> 
     <tr> 
      <td colspan="1">Compromiso</td> 
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
      <td colspan="1" rowspan="1"><p>Descripción del último momento interesante</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Origen del último momento interesante</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Tipo del último momento interesante</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita este proceso para agregar secciones de página de Visualforce y campos de Perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.

1. Repita los pasos del 5 al 7 para agregar secciones de página de Visualforce para Contacto, Cuenta y Oportunidad. A continuación, repita los pasos 8-10 para agregar campos de perspectiva de ventas para **Contacto**. Asegúrese de guardar después de cualquier cambio.

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Así es como.

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Fields** en **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Haga clic en **Asignar campos de posible cliente**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleccione **Contact.Engagement** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita y asigne también estos campos.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Campo personalizado de persona de Marketo</th> 
      <th colspan="1" rowspan="1">Campo personalizado de contacto de Salesforce</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Compromiso</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valor de puntuación relativo</p></td> 
      <td colspan="1" rowspan="1"><p>Valor de puntuación de contacto.relativo</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valor de urgencia</p></td> 
      <td colspan="1" rowspan="1"><p>Valor de Contact.Urgency</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Fecha del último momento interesante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Última fecha de momento interesante</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Descripción del último momento interesante</p></td> 
      <td colspan="1" rowspan="1"><p>Contacto.Último momento interesante Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Origen del último momento interesante</p></td> 
      <td colspan="1" rowspan="1"><p>Contacto.Última fuente de momento interesante</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Tipo del último momento interesante</p></td> 
      <td colspan="1" rowspan="1"><p>Contacto.Último tipo de momento interesante</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** cuando haya terminado.

## Configuración de perspectiva de ventas de Marketo {#marketo-sales-insight-config}

1. Haga clic en **+** y, a continuación, seleccione **Marketo Sales Insight Config**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Marque **Habilitar la API de Marketo**. A continuación, rellene la información de configuración de la API [en Administración de Marketo](#set-up-marketo-sales-insight). Haga clic en **Guardar cambios** cuando haya terminado.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   Si la prueba de diagnóstico falla, es posible que tenga que [agregar más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115).

¡Y eso es todo! Debería poder ver los campos de Perspectiva de ventas de Marketo para Posibles clientes, Contactos, Cuentas y Oportunidades.

![](assets/twenty-six.png)

>[!NOTE]
En el caso de las cuentas, Perspectiva de ventas incluirá todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

## Acceso a la perspectiva de ventas de Marketo {#access-marketo-sales-insight}

1. En Salesforce, haga clic en **+** al final de la barra de pestañas y haga clic en **Marketo Sales Insight Config**.

1. Seleccione la casilla **Enable Marketo API**.

1. Copie las credenciales del panel API de Soap en la página de administración de Sales Insight de Marketo y péguelas en la sección API de Soap de la página Configuración de Salesforce Sales Insight .

1. Copie las credenciales del panel de la API Rest en la página de administración de la perspectiva de ventas de Marketo y péguelas en la sección de la API Rest de la página de configuración de la perspectiva de ventas de Salesforce.

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
* [Prioridad, urgencia, puntuación relativa y mejores apuestas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
* [Agregar la ficha Perspectiva de ventas de Marketo y los botones a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
* [Configuración de la perspectiva de ventas para su equipo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

