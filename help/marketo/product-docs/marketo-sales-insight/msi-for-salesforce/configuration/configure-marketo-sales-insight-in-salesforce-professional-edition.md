---
unique-page-id: 3571743
description: Configurar la perspectiva de ventas de Marketo en Salesforce Professional Edition - Marketo Docs - Documentación del producto
title: Configurar Marketo Sales Insight en Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
source-git-commit: 2fb887e38ec2832b4b62f323d5f72baab24bf41e
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 3%

---

# Configurar Marketo Sales Insight en Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Estos son los pasos que debe seguir para configurar Marketo Sales Insight en Salesforce Professional Edition. Empecemos.

>[!PREREQUISITES]
>
>* Instale Marketo en Salesforce Professional Edition.
>
>* [Instalación del paquete de perspectivas de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}


>[!NOTE]
>
>**Se requieren permisos de administrador**

## Configurar la perspectiva de ventas en Marketo {#configure-sales-insight-in-marketo}

1. Abra una nueva ventana del explorador para obtener las credenciales de Marketo Sales Insight de su cuenta de Marketo.
1. Vaya al área Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Escriba una clave secreta de API de su elección y haga clic en **Guardar**. NO use un signo &amp; en la clave secreta de API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >La clave secreta de API es como una contraseña para su organización y debe ser segura.

1. Haga clic en **Ver** en el panel Configuración de la API restante para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Verá una ventana emergente de confirmación. Haga clic en **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de host de Marketo desde el panel Configuración de la API Soap en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Haga clic en **Nuevo sitio remoto** de nuevo.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoRestAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de API del panel Configuración de la API de Rest en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Rest.

## Configurar Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Inicie sesión en la instancia de Marketo y haga clic en **Administrador**.

   ![](assets/login-admin-1.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Introduzca un **Clave secreta de API** y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No use un signo &amp; en la clave secreta de API.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

1. Vuelva a Salesforce y haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;sitio remoto&quot; y haga clic en **Configuración del sitio remoto** under **Controles de seguridad**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Entrar **Nombre del sitio remoto** y **Dirección URL del sitio remoto** y haga clic en **Guardar**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Elija su **Nombre del sitio remoto** (La API de Marketo se utiliza aquí). La variable **Dirección URL del sitio remoto** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API del paso 4.

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;diseño de página&quot; y seleccione el **Diseño de página** under **Posibles clientes**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Haga clic en **Páginas de VisualForce** a la izquierda. Arrastrar **Sección** vaya al diseño debajo de la sección Vínculos personalizados .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Marketo Sales Insight&quot; como el valor **Nombre de sección**. Select **1 columna** y haga clic en **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastrar y soltar **Posible cliente** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >El nombre de este cuadro cambiará según el tipo de objeto. Por ejemplo, si está modificando el diseño de página de Contactos, dirá Contacto.

1. Haga doble clic en el **Posible cliente** bloque que acaba de añadir.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editar altura a **450** píxeles y clic **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marque **Mostrar barras de desplazamiento** si necesita acceder a las actividades de desplazamiento.

   >[!TIP]
   >
   >Se recomienda una altura de 410 píxeles para los objetos Cuentas y oportunidades .

1. Haga clic en **Campos** a la izquierda. A continuación, busque y arrastre el **Participación** en el **Perspectiva de ventas de Marketo** diseño.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

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

1. Repita este proceso para agregar secciones de página de Visualización y campos de Perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.
1. Repita los pasos del 5 al 7 para agregar secciones de página de Visualforce para Contacto, Cuenta y Oportunidad. A continuación, repita los pasos 8-10 para agregar campos de perspectivas de ventas para **Contacto**. Asegúrese de guardar después de cualquier cambio.

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Así es como.

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Campos** under **Posibles clientes**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Haga clic en **Asignar campos de posible cliente**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Select **Contact.Engagement** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Ficha Configuración de la perspectiva de ventas de Marketo {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en la **+** al final de la barra de pestañas y haga clic en **Configuración de perspectiva de ventas de Marketo**.

1. Copie las credenciales del panel API de Soap en [Página de administración de la perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} y péguelos en la sección API de Soap de la página Configuración de la perspectiva de ventas de Salesforce.

1. Copie las credenciales del panel de la API de Rest en [Página de administración de la perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} y péguelos en la sección API Rest de la página Configuración de la perspectiva de ventas de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

¡Y eso es todo! Debería poder ver los campos de Perspectiva de ventas de Marketo para Posibles clientes, Contactos, Cuentas y Oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, es posible que tenga que [añadir más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115){target=&quot;_blank&quot;}.

>[!NOTE]
>
>En el caso de las cuentas, Perspectiva de ventas incluirá todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y mejores apuestas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target=&quot;_blank&quot;}
>* [Añadir la ficha Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target=&quot;_blank&quot;}
>* [Agregar el acceso a la perspectiva de ventas a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

