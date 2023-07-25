---
unique-page-id: 3571743
description: 'Configuración de Marketo Sales Insight en Salesforce Professional Edition: documentación del producto de Marketo'
title: Configuración de Marketo Sales Insight en Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 4%

---

# Configuración de Marketo Sales Insight en Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Estos son los pasos que debe seguir para configurar Marketo Sales Insight en Salesforce Professional Edition. Comencemos.

>[!PREREQUISITES]
>
>* Instale Marketo en su Salesforce Professional Edition.
>
>* [Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Permisos de administración necesarios**

## Configuración de Sales Insight en Marketo {#configure-sales-insight-in-marketo}

1. Abra una nueva ventana del explorador para obtener las credenciales de Marketo Sales Insight de su cuenta de Marketo.
1. Vaya al área de Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Clic **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Introduzca una clave secreta de API de su elección y haga clic en **Guardar**. NO use el signo &amp; en la clave secreta de la API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >La clave secreta de la API es como una contraseña para su organización y debe ser segura.

1. Clic **Ver** en el panel Configuración de la API de REST para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Verá una ventana emergente de confirmación. Clic **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configuración de Sales Insight en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic **Configurar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Clic **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es la URL del host de Marketo desde el panel Configuración de la API de SOAP en Marketo. Clic **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Clic **Nuevo sitio remoto** otra vez.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoRestAPI&quot;). Introduzca la URL del sitio remoto, que es la URL de la API desde el panel Configuración de la API de REST en Marketo. Clic **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de REST.

## Configuración de Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Inicie sesión en la instancia de Marketo y haga clic en **Administrador**.

   ![](assets/login-admin-1.png)

1. Clic **Perspectiva de ventas**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Clic **Editar configuración de API**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Introduzca una **Clave secreta de API** y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

1. Vuelva a Salesforce y haga clic en **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;sitio remoto&quot; y haga clic en **Configuración del sitio remoto** bajo **Controles de seguridad**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Clic **Nuevo sitio remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Entrar **Nombre de sitio remoto** y **URL del sitio remoto**, luego haga clic en **Guardar**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Usted elige su **Nombre de sitio remoto** (La API de Marketo se utiliza aquí). El **URL del sitio remoto** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API del paso 4.

## Personalizar diseños de página {#customize-page-layouts}

1. Clic **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;diseño de página&quot; y seleccione **Diseño de página** bajo **Posibles clientes**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Clic **Visualforce Pages** a la izquierda. Arrastrar **Sección** al diseño debajo de la sección Vínculos personalizados.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Marketo Sales Insight&quot; como **Nombre de sección**. Seleccionar **1 columna** y haga clic en **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastrar y soltar **Posible cliente** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >El nombre de este cuadro cambiará en función del tipo de objeto. Por ejemplo, si está modificando el diseño de página para Contactos, indicará Contacto.

1. Haga doble clic en **Posible cliente** que acaba de agregar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editar altura a **450** píxeles y clic **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marque **Mostrar barras de desplazamiento** si necesita acceso a las actividades de desplazamiento.

   >[!TIP]
   >
   >Se recomienda una altura de 410 píxeles para los objetos Accounts y Opportunity.

1. Haga clic en **Campos** a la izquierda. A continuación, busque y arrastre el **Participación** etiqueta en el **Perspectiva de ventas de Marketo** diseño.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Repita el paso anterior también para estos campos.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Participación</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de puntuación relativa</p></td> 
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

1. Clic **Guardar** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita este proceso para añadir secciones de página de Visualforce y campos de perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.
1. Repita los pasos 5-7 para agregar secciones de página de Visualforce para Contacto, Cuenta y Oportunidad. A continuación, repita los pasos 8-10 para añadir los campos de Perspectiva de ventas para **Contacto**. Asegúrese de guardar después de realizar cualquier cambio.

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Así es como.

1. Clic **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Campos** bajo **Posibles clientes**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Clic **Asignar campos de posibles clientes**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Seleccionar **Contact.Engagement** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Repita y asigne también estos campos.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Campo personalizado de persona de Marketo</th> 
   <th colspan="1" rowspan="1">Campo personalizado de contacto de Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Participación</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de puntuación relativa</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Relative Score Value</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgencia</p></td> 
   <td colspan="1" rowspan="1"><p>Valor Contact.Urgency</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Fecha del último momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Fecha del último momento interesante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Descripción del último momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Último momento interesante Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Origen del último momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Último momento interesante origen</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo del último momento interesante</p></td> 
   <td colspan="1" rowspan="1"><p>Contacto.Último tipo de momento interesante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clic **Guardar** cuando haya terminado.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Pestaña Configuración de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en **+** al final de la barra de pestañas y haga clic en **Configuración de Marketo Sales Insight**.

1. Copie las credenciales del panel API de Soap en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de Soap de la página Configuración de Sales Insight de Salesforce.

1. Copie las credenciales del panel API de REST en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de REST de la página Configuración de Sales Insight de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

¡Y eso es todo! Debería poder ver los campos de perspectiva de ventas de Marketo para posibles clientes, contactos, cuentas y oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, es posible que tenga que [agregar más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>En el caso de las cuentas, Sales Insight incluirá todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y resultados más probables](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Añadir la pestaña Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Añadir el acceso de Sales Insight a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
