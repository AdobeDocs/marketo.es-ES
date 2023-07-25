---
unique-page-id: 2360354
description: "Agregar [!DNL Munchkin] Código de seguimiento para su sitio web - Documentos de Marketo - Documentación del producto"
title: "Agregar [!DNL Munchkin] Código de seguimiento para su sitio web"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Añadir [!DNL Munchkin] Código de seguimiento para su sitio web {#add-munchkin-tracking-code-to-your-website}

código de seguimiento personalizado de JavaScript de Marketo, denominado [!DNL Munchkin], registra todas las personas que visitan el sitio web para que pueda reaccionar a sus visitas con campañas de marketing automatizadas. Incluso los visitantes anónimos se rastrean junto con sus direcciones IP y otra información. **Sin este código de seguimiento, no podrá rastrear visitas u otras actividades en su sitio web**!

>[!PREREQUISITES]
>
>Asegúrese de tener acceso a un desarrollador de JavaScript con experiencia. El Soporte técnico de Marketo no está configurado para ayudar a solucionar problemas con JavaScript personalizado.

## Añadir código de seguimiento a su sitio web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Los clientes de Adobe Experience Cloud también pueden utilizar la integración de Marketo en Adobe Launch para incluir lo siguiente [!DNL Munchkin] script en sus páginas web. Obtener la aplicación [aquí](https://www.adobeexchange.com/experiencecloud.details.101054.html){target="_blank"}.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Clic **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Seleccionar **[!UICONTROL Asíncrona]** para **[!UICONTROL Tipo de código de seguimiento]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >En casi todos los casos, debe utilizar el código asincrónico. [Más información](#types-of-munchkin-tracking-codes).

1. Haga clic en y copie el código de seguimiento de Javascript que desea colocar en el sitio web.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >No use el código mostrado en esta captura de pantalla: debe usar el código único que aparece en su cuenta.

   >[!TIP]
   >
   >Coloque el código de seguimiento en las páginas web que desee rastrear. Esto puede ser cada página para sitios más pequeños o solo páginas clave en sitios que tienen muchas páginas web generadas dinámicamente, foros de usuarios, etc.

   Para obtener los mejores resultados, utilice la función asincrónica [!DNL Munchkin] y colóquelo dentro de la etiqueta `<head>` elementos de las páginas. Si utiliza código simple (no recomendado), justo antes del `</body>` etiqueta.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Para los sitios que ven un gran volumen de tráfico (es decir, cientos de miles de visitas al mes), le recomendamos que opte por no rastrear a personas anónimas. [Más información](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Añadir código de seguimiento al usar varios espacios de trabajo {#add-tracking-code-when-using-multiple-workspaces}

Si utiliza espacios de trabajo en su cuenta de Marketo, es probable que también tenga presencias web independientes que se correspondan con los espacios de trabajo. En ese caso, puede utilizar la variable [!DNL Munchkin] Javascript de seguimiento para asignar a sus usuarios anónimos al espacio de trabajo y la partición correctos.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Clic **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Seleccione el espacio de trabajo adecuado para las páginas web que desee rastrear.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Si no utiliza el espacio de trabajo especial [!DNL Munchkin] , las personas se asignarán a la partición predeterminada que se creó con la configuración de la cuenta. Se llama &quot;[!UICONTROL Predeterminado]&quot; inicialmente, pero es posible que lo haya cambiado en su propia cuenta de Marketo.

1. Seleccionar **[!UICONTROL Asíncrona]** para **[!UICONTROL Tipo de código de seguimiento]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Haga clic en y copie el código de seguimiento de JavaScript que desea colocar en el sitio web.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >No use el código mostrado en esta captura de pantalla: debe usar el código único que aparece en su cuenta.

1. Coloque el código de seguimiento en las páginas web en la variable `<head>` Elemento. Las personas nuevas que visiten esta página se asignarán a esta partición.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Solo puede usar uno [!DNL Munchkin] script de seguimiento para una sola partición y espacio de trabajo en una página. No incluya scripts de seguimiento para varias particiones o espacios de trabajo en el sitio web.

   >[!NOTE]
   >
   >Las páginas de aterrizaje creadas en Marketo contienen automáticamente código de seguimiento, por lo que no es necesario colocarlo.

## Tipos de [!DNL Munchkin] Códigos de seguimiento {#types-of-munchkin-tracking-codes}

Existen tres tipos de [!DNL Munchkin] códigos de seguimiento entre los que puede elegir. Cada impacto en los tiempos de carga de la página web es diferente.

1. **[!UICONTROL Sencilla]**: tiene las menos líneas de código, pero no optimiza el tiempo de carga de la página web. Este código carga la biblioteca jQuery cada vez que se carga una página web.
1. **[!UICONTROL Asíncrona]**: reduce el tiempo de carga de la página web.
1. **[!UICONTROL jQuery asincrónico]**: reduce el tiempo de carga de la página web y también mejora el rendimiento del sistema. Este código supone que ya tiene jQuery y no marca la casilla para cargarlo.

## Comprobar si su [!DNL Munchkin] El código está funcionando {#test-if-your-munchkin-code-is-working}

Para comprobar que su [!DNL Munchkin] El código de está funcionando después de agregarlo:

1. Visite su página web.

1. En su [!DNL My Marketo], haga clic en **[!UICONTROL Analytics]** mosaico.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Clic **[!UICONTROL Actividad de página web]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Haga clic en **[!UICONTROL Configurar]** pestaña, haga doble clic en **[!UICONTROL Origen de actividad]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Cambie el [!UICONTROL Origen de actividad] hasta **[!UICONTROL Visitantes anónimos (incluidos ISP)]** y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Haga clic en **[!UICONTROL Informe]** pestaña.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Si no ve ningún dato, espere unos minutos y, a continuación, haga clic en el icono de actualización situado en la parte inferior.
