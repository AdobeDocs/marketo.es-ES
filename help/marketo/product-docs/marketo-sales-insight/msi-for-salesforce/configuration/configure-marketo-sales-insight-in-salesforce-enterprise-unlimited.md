---
unique-page-id: 2360368
description: Aprenda a configurar Marketo Sales Insight en las ediciones de Salesforce Enterprise/Unlimited.
title: Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Para configurar Marketo Sales Insight en las ediciones de Salesforce Enterprise/Unlimited, complete los siguientes pasos.

>[!PREREQUISITES]
>
>[Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Se requieren permisos de administrador.**

## Configuración del conocimiento de ventas en Marketo Engage {#configure-sales-insight-in-marketo}

1. Para obtener las credenciales de Marketo Sales Insight en Marketo Engage, vaya a **[!UICONTROL Administrador]** y seleccione **[!UICONTROL Perspectiva de ventas]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clic **[!UICONTROL Editar configuración de API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Introduzca una clave secreta de API de su elección y haga clic en **[!UICONTROL Guardar]**. NO utilice una y comercial (`&`) en la clave secreta de la API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La clave secreta de API gustar es un contraseña de su organización y debe ser segura.

1. Para completar las credenciales, haga clic **[!UICONTROL en Ver]** en el panel Configuración de _[!UICONTROL API de REST]_ .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Cuando vea un cuadro de diálogo de confirmación, haga clic en **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenga esta ventana abierta. Necesitará esta información más adelante para la configuración de Salesforce.

## Configuración de Sales Insight en Salesforce {#configure-sales-insight-in-salesforce}

1. En Salesforce, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Search &quot;sitio remoto&quot; y seleccione **[!UICONTROL Sitio remoto Configuración]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Haga clic en **[!UICONTROL Nuevo sitio]** remoto.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Introduzca el nombre del sitio remoto (puede ser similar a `MarketoSoapAPI`). Ingrese al URL sitio remoto, que es su URL de host de Marketo desde el panel Configuración de la _[!UICONTROL API Soap]_ en Marketo Engage. Haga clic en **[!UICONTROL Guardar]**. Ahora ha creado la configuración del sitio remoto para la API de Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clic **[!UICONTROL Nuevo sitio remoto]** otra vez.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Escriba el nombre del sitio remoto (puede ser similar a `MarketoAPI`). Introduzca la URL del sitio remoto, que es la URL de la API desde _[!UICONTROL Configuración de API de REST]_ panel en el Marketo Engage. Haga clic en **[!UICONTROL Guardar]**. Ahora ha creado la configuración del sitio remoto para la API de REST.

   >[!NOTE]
   >
   >_Usted_ elija su **[!UICONTROL Nombre de sitio remoto]** (`MarketoAPI` se utiliza aquí). El **[!UICONTROL URL del sitio remoto]** se encuentra en el campo Host de Marketo del cuadro de diálogo Editar configuración de API desde el paso 3 de la sección Configurar Sales Insight en Marketo.

## Conceder acceso al perfil de los usuarios de Sales Insight a objetos de Salesforce estándar {#grant-sales-insight-users-profile-access}

Debido a las mejoras de seguridad de Salesforce, los paquetes de AppExchange ya no pueden conceder permiso a objetos estándar y se debe conceder acceso a los objetos de Salesforce relevantes desde el perfil del usuario de Salesforce. Para conceder los permisos necesarios, siga estos pasos.

1. Clic **[!UICONTROL Configurar]**.

1. Buscar &quot;Perfiles&quot; en Búsqueda rápida.

1. Clic **[!UICONTROL Editar]** junto al perfil que utilizan los usuarios de Salesforce.

1. En el _[!UICONTROL Permiso de objeto estándar]_ sección, habilitar **[!UICONTROL Leer]** acceso para los siguientes objetos: [!UICONTROL Posible cliente], [!UICONTROL Contacto], [!UICONTROL Cuenta], y [!UICONTROL Oportunidad].

1. Haga clic en **[!UICONTROL Guardar]**.

## Personalizar diseños de página {#customize-page-layouts}

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;diseño de página&quot; y seleccione **[!UICONTROL Diseño de página]** bajo **[!UICONTROL Posibles clientes]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clic **[!UICONTROL Visualforce Pages]** a la izquierda. Arrastrar **[!UICONTROL Sección]** al diseño debajo de la _[!UICONTROL Vínculos personalizados]_ sección.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Introduzca &quot;Marketo Sales Insight&quot; como **[!UICONTROL Nombre de sección]**, seleccione **[!UICONTROL 1 columna]** y haga clic en **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastrar y soltar **[!UICONTROL Posible cliente]** en la nueva sección.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >El nombre de este cuadro cambia según el tipo de objeto. Por ejemplo, si está modificando el diseño de página de Contactos, se mostrará Contacto.

1. Haga doble clic en **[!UICONTROL Posible cliente]** que acaba de agregar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editar altura a **450** píxeles y clic **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marque **[!UICONTROL Mostrar barras de desplazamiento]** si necesita acceso a las actividades de desplazamiento.

   >[!TIP]
   >
   >La altura recomendada para los objetos Cuentas y oportunidades es de 410 píxeles.

1. Clic **[!UICONTROL Campos]** a la izquierda. A continuación, busque y arrastre el **[!UICONTROL Urgencia]** etiqueta en el **[!UICONTROL Perspectiva de ventas de Marketo]** diseño.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Repita el paso anterior también para estos campos.

   * Último momento interesante
   * Fecha del último momento interesante
   * Descripción del último momento interesante
   * Origen del último momento interesante
   * Tipo del último momento interesante
   * Última actividad por ventas
   * Último compromiso por ventas
   * ID de contacto MSI
   * Puntaje relativo
   * Valor de puntuación relativa
   * Urgencia
   * Valor de urgencia
   * Ver en Marketo

1. Clic **[!UICONTROL Guardar]** cuando termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita los pasos 5-7 para añadir secciones de página de Visualforce y campos de perspectiva de ventas para **[!UICONTROL Contacto]**, **[!UICONTROL Cuenta]**, y **[!UICONTROL Oportunidad]**.

1. Repita los pasos 8-10 para añadir estos campos de perspectiva de ventas para **[!UICONTROL Contacto]**. Asegúrese de guardar los cambios.

   * Último momento interesante
   * Fecha del último momento interesante
   * [!UICONTROL Desc de último momento interesante]
   * [!UICONTROL Origen del último momento interesante]
   * [!UICONTROL Tipo de último momento interesante]
   * [!UICONTROL Última actividad de Marketo por ventas]
   * [!UICONTROL Última participación de Marketo por ventas]
   * [!UICONTROL MKTO Lead Score]
   * [!UICONTROL Puntuación relativa]
   * [!UICONTROL Puntuación relativa Valor]
   * [!UICONTROL Perspectiva de ventas] - Abre la página de lista completa de contactos
   * [!UICONTROL Urgencia]
   * [!UICONTROL Urgencia Valor]

## Asignar campos de persona personalizados {#map-custom-person-fields}

Los campos de persona de Marketo deben asignarse a los campos de contacto de Salesforce para garantizar que la Conversión funcione correctamente. Siga estos pasos para asignarlos.

1. Clic **[!UICONTROL Configurar]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Busque &quot;campos&quot; en la barra de búsqueda y haga clic en **[!UICONTROL Campos]** bajo **[!UICONTROL Posibles clientes]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clic **[!UICONTROL Asignar campos de posibles clientes]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Haga clic en el menú desplegable de la derecha para **[!UICONTROL Participación]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleccionar **[!UICONTROL Contact.Engagement]** en la lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

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

1. Clic **[!UICONTROL Guardar]** cuando hayas terminado.

## Pestaña Configuración de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. En Salesforce, haga clic en **+** al final de la barra de pestañas y haga clic en **[!UICONTROL Configuración de Marketo Sales Insight]**.

1. Copie las credenciales del panel API de Soap en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de Soap de la página Configuración de Sales Insight de Salesforce.

1. Copie las credenciales del panel API de REST en [Página de administración de Sales Insight de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} y péguelos en la sección API de REST de la página Configuración de Sales Insight de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Debería poder ver los campos de perspectiva de ventas de Marketo para posibles clientes, contactos, cuentas y oportunidades.

>[!NOTE]
>
>Si la prueba de diagnóstico falla, [agregar más campos al diseño de página](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} podría solucionar el problema.

>[!NOTE]
>
>En el caso de las cuentas, Sales Insight incluye todos los correos electrónicos, pero solo los momentos interesantes más recientes, la actividad web y los cambios de puntuación.

>[!MORELIKETHIS]
>
>* [Prioridad, urgencia, puntuación relativa y resultados más probables](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Añadir la pestaña Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Añadir el acceso de Sales Insight a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
