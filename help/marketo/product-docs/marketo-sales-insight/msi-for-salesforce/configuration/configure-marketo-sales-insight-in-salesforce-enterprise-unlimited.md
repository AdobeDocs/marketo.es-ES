---
unique-page-id: 2360368
description: 'Configuración del conocimiento de ventas de Marketo en Salesforce Enterprise/Unlimited: documentos de Marketo: documentación del producto'
title: Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: c85f544f2c06a2f5bb92d6e7cad5f801e73fdaed
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 8%

---

# Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

A continuación se indican los pasos que debe seguir para configurar Marketo Sales Insight en Salesforce Enterprise/Unlimited Editions. Comencemos.

>[!PREREQUISITES]
>
>[Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Permisos de administración necesarios**

## Configuración de Sales Insight en Marketo {#configure-sales-insight-in-marketo}

1. Obtenga sus credenciales de MSI en Marketo. Vaya al área de Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clic **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Introduzca una clave secreta de API de su elección y haga clic en **Guardar**. NO use el signo &amp; en la clave secreta de la API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La clave secreta de la API es como una contraseña para su organización y debe ser segura.

1. Clic **Ver** en el panel Configuración de la API de REST para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verá una ventana emergente de confirmación. Clic **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

## Configuración de Sales Insight en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic **Configurar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clic **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es la URL del host de Marketo desde el panel Configuración de la API de SOAP en Marketo. Clic **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clic **Nuevo sitio remoto** otra vez.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoAPI&quot;). Introduzca la URL del sitio remoto, que es la URL de la API desde el panel Configuración de la API de REST en Marketo. Clic **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de REST.

   >[!NOTE]
   >
   >_Usted_ elija su **Nombre de sitio remoto** (La API de Marketo se utiliza aquí). El **URL del sitio remoto** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API desde el paso 3 de la sección &quot;Configuración de Sales Insight en Marketo&quot;.

## Conceder acceso al perfil de los usuarios de Sales Insight a objetos de Salesforce estándar {#grant-sales-insight-users-profile-access}

Debido a las mejoras de seguridad de Salesforce, los paquetes de App Exchange ya no pueden conceder permiso a objetos estándar y deberá concederse acceso a los objetos de Salesforce relevantes desde el perfil del usuario de Salesforce.  Siga los pasos a continuación para conceder los permisos necesarios.

1. Clic **Configurar**.

1. Buscar &quot;Perfiles&quot; en Búsqueda rápida.

1. Clic **Editar** junto al perfil que utilizan los usuarios de Salesforce.

1. En la sección Permiso de objeto estándar, habilite el acceso de lectura para los siguientes objetos: Posible cliente, Contacto, Cuenta y Oportunidad.

1. Clic **Guardar**.

## Personalizar diseños de página {#customize-page-layouts}

1. Clic **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;diseño de página&quot; y seleccione **Diseño de página** bajo **Posibles clientes**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

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

1. Haga clic en **Campos** a la izquierda. A continuación, busque y arrastre el **Urgencia** etiqueta en el **Perspectiva de ventas de Marketo** diseño.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Repita el paso anterior también para estos campos.

   <table> 
    <tbody> 
     <tr> 
      <td>Último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Fecha del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Descripción del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Origen del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Tipo del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Última actividad de por parte de ventas</td> 
     </tr> 
     <tr> 
      <td>Última participación de por parte de ventas</td> 
     </tr> 
     <tr> 
      <td>ID de contacto MSI</td> 
     </tr> 
     <tr> 
      <td>Puntaje relativo</td> 
     </tr> 
     <tr> 
      <td>Valor de puntuación relativa</td> 
     </tr> 
     <tr> 
      <td>Urgencia</td> 
     </tr> 
     <tr> 
      <td>Valor de urgencia</td> 
     </tr> 
     <tr> 
      <td>Ver en Marketo</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Guardar** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita los pasos 5-7 para añadir secciones de página de Visualforce y campos de perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.

1. Repita los pasos 8-10 para añadir los campos de Perspectiva de ventas de la lista siguiente para **Contacto**. Asegúrese de guardar los cambios.

<table> 
    <tbody> 
     <tr> 
      <td>Último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Fecha del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Descripción del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Origen del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Tipo del último momento interesante</td> 
     </tr> 
     <tr> 
      <td>Última actividad de Marketo por parte de ventas</td> 
     </tr> 
     <tr> 
      <td>Última participación de Marketo por parte de ventas</td> 
     </tr> 
     <tr> 
      <td>Puntuación de clientes potenciales de MKTO</td> 
     </tr> 
     <tr> 
      <td>Puntaje relativo</td> 
     </tr> 
     <tr> 
      <td>Valor de puntuación relativa</td> 
     </tr> 
     <tr> 
      <td>Perspectiva de ventas - Abre la página de lista completa de contactos</td> 
     </tr> 
     <tr> 
      <td>Urgencia</td> 
     </tr> 
     <tr> 
      <td>Valor de urgencia</td> 
     </tr> 
    </tbody> 
   </table>

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Así es como.

1. Clic **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Campos** bajo **Posibles clientes**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clic **Asignar campos de posibles clientes**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleccionar **Contact.Engagement** en la lista.

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

1. Clic **Guardar** cuando hayas terminado.

## Pestaña Configuración de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en **+** al final de la barra de pestañas y haga clic en **Configuración de Marketo Sales Insight**.

1. Copie las credenciales del panel API de Soap en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de Soap de la página Configuración de Sales Insight de Salesforce.

1. Copie las credenciales del panel API de REST en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de REST de la página Configuración de Sales Insight de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

¡Y eso es todo! Debería poder ver los campos de perspectiva de ventas de Marketo para posibles clientes, contactos, cuentas y oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, es posible que tenga que [agregar más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>En el caso de las cuentas, Sales Insight incluirá todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y resultados más probables](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Añadir la pestaña Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Añadir el acceso de Sales Insight a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
