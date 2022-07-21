---
unique-page-id: 2360368
description: Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited - Marketo Docs - Documentación del producto
title: Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: 2fb887e38ec2832b4b62f323d5f72baab24bf41e
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 6%

---

# Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estos son los pasos que debe seguir para configurar Marketo Sales Insight en Salesforce Enterprise/Unlimited Editions. Empecemos.

>[!PREREQUISITES]
>
>[Instalación del paquete de perspectivas de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Configurar la perspectiva de ventas en Marketo {#configure-sales-insight-in-marketo}

1. Obtenga sus credenciales de MSI en Marketo. Vaya al área Administración y seleccione **Perspectiva de ventas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Haga clic en **Editar configuración de API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Escriba una clave secreta de API de su elección y haga clic en **Guardar**. NO use un signo &amp; en la clave secreta de API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La clave secreta de API es como una contraseña para su organización y debe ser segura.

1. Haga clic en **Ver** en el panel Configuración de la API restante para rellenar las credenciales.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verá una ventana emergente de confirmación. Haga clic en **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante en Salesforce.

## Configurar la perspectiva de ventas en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoSoapAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de host de Marketo desde el panel Configuración de la API Soap en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Haga clic en **Nuevo sitio remoto** de nuevo.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoAPI&quot;). Introduzca la URL del sitio remoto, que es su URL de API del panel Configuración de la API de Rest en Marketo. Haga clic en **Guardar**. Ahora ha creado la configuración del sitio remoto para la API de Rest.

   >[!NOTE]
   >
   >_You_ elija su **Nombre del sitio remoto** (La API de Marketo se utiliza aquí). La variable **Dirección URL del sitio remoto** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API del paso 3 de la sección &quot;Configurar perspectivas de ventas en Marketo&quot;.

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;diseño de página&quot; y seleccione el **Diseño de página** under **Posibles clientes**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

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

1. Haga clic en **Campos** a la izquierda. A continuación, busque y arrastre el **Urgencia** en el **Perspectiva de ventas de Marketo** diseño.

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
      <td>Última actividad de Marketo por ventas</td> 
     </tr> 
     <tr> 
      <td>Última participación de Marketo por ventas</td> 
     </tr> 
     <tr> 
      <td>ID de contacto de MSI</td> 
     </tr> 
     <tr> 
      <td>Puntaje relativo</td> 
     </tr> 
     <tr> 
      <td>Valor de puntuación relativo</td> 
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

1. Haga clic en **Guardar** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita los pasos del 5 al 7 para agregar secciones de página de Visualforce y campos de perspectiva de ventas para **Contacto**, **Cuenta** y **Oportunidad**.

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
      <td>Última actividad de Marketo por ventas</td> 
     </tr> 
     <tr> 
      <td>Última participación de Marketo por ventas</td> 
     </tr> 
     <tr> 
      <td>Puntuación de posibles clientes de MKTO</td> 
     </tr> 
     <tr> 
      <td>Puntaje relativo</td> 
     </tr> 
     <tr> 
      <td>Valor de puntuación relativo</td> 
     </tr> 
     <tr> 
      <td>Perspectiva de ventas: abre la página de lista completa de contactos</td> 
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

1. Haga clic en **Configuración**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **Campos** under **Posibles clientes**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Haga clic en **Asignar campos de posible cliente**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Haga clic en el menú desplegable de la derecha para **Participación**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Select **Contact.Engagement** en la lista.

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

## Ficha Configuración de la perspectiva de ventas de Marketo {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en la **+** al final de la barra de pestañas y haga clic en **Configuración de perspectiva de ventas de Marketo**.

1. Seleccione el **Habilitar la API de Marketo** casilla de verificación.

1. Copie las credenciales del panel API de Soap en [Página de administración de la perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} y péguelos en la sección API de Soap de la página Configuración de la perspectiva de ventas de Salesforce.

1. Copie las credenciales del panel de la API de Rest en [Página de administración de la perspectiva de ventas de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} y péguelos en la sección API Rest de la página Configuración de la perspectiva de ventas de Salesforce.

   ![](assets/access-msi.png)

¡Y eso es todo! Debería poder ver los campos de Perspectiva de ventas de Marketo para Posibles clientes, Contactos, Cuentas y Oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, es posible que tenga que [añadir más campos al diseño de página](https://nation.marketo.com/docs/DOC-1115){target=&quot;_blank&quot;}.

>[!NOTE]
>
>En el caso de las cuentas, Perspectiva de ventas incluirá todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y mejores apuestas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Añadir la ficha Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Agregar el acceso a la perspectiva de ventas a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

