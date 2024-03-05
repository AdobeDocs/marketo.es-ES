---
unique-page-id: 3571743
description: Obtenga información sobre cómo configurar Marketo Sales Insight en Salesforce Professional Edition.
title: Configuración de Marketo Sales Insight en Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 68abebb5e1f9dc0780aedcff51d46ed12d5b4d0a
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Configuración de Marketo Sales Insight en Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Para configurar Marketo Sales Insight en Salesforce Professional Edition, complete los siguientes pasos.

>[!PREREQUISITES]
>
>* Instale Marketo en su Salesforce Professional Edition.
>
>* [Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Se requieren permisos de administrador.**

## Configuración del conocimiento de ventas en Marketo Engage {#configure-sales-insight-in-marketo}

1. Para obtener las credenciales de Marketo Sales Insight de su cuenta de Marketo, abra una nueva ventana del explorador.

1. Vaya a la **[!UICONTROL Administrador]** y seleccione **[!UICONTROL Perspectiva de ventas]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Clic **[!UICONTROL Editar configuración de API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Introduzca una clave secreta de API de su elección y haga clic en **[!UICONTROL Guardar]**. NO use un signo &amp; (`&`) en su clave secreta de la API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >La clave secreta de la API es como una contraseña para su organización y debe ser segura.

1. Para rellenar las credenciales, haga clic en **[!UICONTROL Ver]** en el _[!UICONTROL Configuración de API de REST]_ panel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Cuando vea un cuadro de diálogo de confirmación, haga clic en **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configuración de Sales Insight en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **[!UICONTROL Configurar]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **[!UICONTROL Configuración del sitio remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Clic **[!UICONTROL Nuevo sitio remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Escriba el nombre del sitio remoto (puede ser similar a `MarketoSoapAPI`). Introduzca la URL del sitio remoto, que es la URL del host de Marketo desde el panel de configuración de la API de SOAP en Marketo Engage. Haga clic en **[!UICONTROL Guardar]**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Clic **[!UICONTROL Nuevo sitio remoto]** otra vez.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoRestAPI&quot;). Introduzca la URL del sitio remoto, que es la URL de la API desde el panel Configuración de la API de REST en Marketo. Haga clic en **[!UICONTROL Guardar]**. Ahora ha creado la configuración del sitio remoto para la API de REST.

## Conceder acceso al perfil de los usuarios de Sales Insight a objetos de Salesforce estándar {#grant-sales-insight-users-profile-access}

Debido a las mejoras de seguridad de Salesforce, los paquetes de AppExchange ya no pueden conceder permiso a objetos estándar y se debe conceder acceso a los objetos de Salesforce relevantes desde el perfil del usuario de Salesforce. Conceda los permisos necesarios siguiendo estos pasos.

1. Clic **[!UICONTROL Configurar]**.

1. Buscar &quot;Perfiles&quot; en Búsqueda rápida.

1. Clic **[!UICONTROL Editar]** junto al perfil que utilizan los usuarios de Salesforce.

1. En la sección Permiso de objeto estándar, habilite el acceso de lectura para los siguientes objetos: Posible cliente, Contacto, Cuenta y Oportunidad.

1. Haga clic en **[!UICONTROL Guardar]**.

## Personalizar diseños de página {#customize-page-layouts}

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;diseño de página&quot; y seleccione **[!UICONTROL Diseño de página]** bajo **[!UICONTROL Posibles clientes]**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Clic **[!UICONTROL Visualforce Pages]** a la izquierda. Arrastrar **[!UICONTROL Sección]** al diseño debajo de la sección Vínculos personalizados.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Marketo Sales Insight&quot; como **[!UICONTROL Nombre de sección]**. Seleccionar **[!UICONTROL 1 columna]** y haga clic en **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastrar y soltar **Posible cliente** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >El nombre de este cuadro cambia según el tipo de objeto. Por ejemplo, si está modificando el diseño de página de Contactos, se mostrará Contacto.

1. Haga doble clic en **[!UICONTROL Posible cliente]** que acaba de agregar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite la altura a 450 píxeles y haga clic en **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marque **[!UICONTROL Mostrar barras de desplazamiento]** si necesita acceso a las actividades de desplazamiento.

   >[!TIP]
   >
   >La altura recomendada para los objetos Cuentas y oportunidades es de 410 píxeles.

1. Clic **[!UICONTROL Campos]** a la izquierda. A continuación, busque y arrastre el **[!UICONTROL Participación]** etiqueta en el **[!UICONTROL Perspectiva de ventas de Marketo]** diseño.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Repita el paso anterior para los campos siguientes:

   * [!UICONTROL Participación]
   * [!UICONTROL Valor de puntuación relativa]
   * [!UICONTROL Valor de urgencia]
   * [!UICONTROL Fecha del último momento interesante]
   * [!UICONTROL Desc de último momento interesante]
   * [!UICONTROL Origen del último momento interesante]
   * [!UICONTROL Tipo de último momento interesante]

1. Clic **[!UICONTROL Guardar]** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Para agregar secciones de página de Visualforce para **[!UICONTROL Contacto]**, **[!UICONTROL Cuenta]**, y **[!UICONTROL Oportunidad]**, repita los pasos 5-7.

1. Repita los pasos 8-10 para añadir los campos de Perspectiva de ventas para **[!UICONTROL Contacto]**. Asegúrese de guardar después de realizar cualquier cambio.

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la conversión funcione correctamente. Siga estos pasos para asignarlos.

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **[!UICONTROL Campos]** bajo **[!UICONTROL Posibles clientes]**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Clic **[!UICONTROL Asignar campos de posibles clientes]**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Haga clic en el menú desplegable de la derecha para **[!UICONTROL Participación]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Seleccionar **[!UICONTROL Contact.Engagement]** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Repita y asigne también estos campos.

   | Campo personalizado de persona de Marketo | Campo personalizado de contacto de Salesforce |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. Cuando haya terminado, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Pestaña Configuración de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en **+** al final de la barra de pestañas y haga clic en **[!UICONTROL Configuración de Marketo Sales Insight]**.

1. Copie las credenciales del panel API de Soap en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de Soap de la página Configuración de Sales Insight de Salesforce.

1. Copie las credenciales de la **[!UICONTROL API de REST]** panel en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de REST de la página Configuración de Sales Insight de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Debería poder ver los campos de perspectiva de ventas de Marketo para posibles clientes, contactos, cuentas y oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, [agregar más campos al diseño de página](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} podría solucionar el problema.

>[!NOTE]
>
>En el caso de las cuentas, Sales Insight incluye todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y resultados más probables](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Añadir la pestaña Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Añadir el acceso de Sales Insight a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
