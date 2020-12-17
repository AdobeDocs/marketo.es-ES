---
unique-page-id: 2360354
description: Añadir código de seguimiento de Munchkin a su sitio web - Documentos de marketing - Documentación del producto
title: Añadir código de seguimiento de Munchkin a su sitio web
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---


# Añadir código de seguimiento de Munchkin a su sitio Web {#add-munchkin-tracking-code-to-your-website}

El código de seguimiento personalizado de JavaScript de Marketing, llamado Munchkin, rastrea a todas las personas que visitan el sitio web para que pueda reaccionar a sus visitas con campañas de marketing automatizadas. Incluso los visitantes anónimos son rastreados junto con sus direcciones IP y otra información. ** Sin este código de seguimiento, no podrá rastrear visitas u otras actividades en su sitio web!**

>[!PREREQUISITES]
>
>Asegúrese de tener acceso a un desarrollador de JavaScript experimentado. La asistencia técnica de marketing no está configurada para ayudar a solucionar problemas de JavaScript personalizado.

## Añadir código de seguimiento a su sitio Web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Los clientes de Adobe Experience Cloud también pueden utilizar la integración de Marketo en Adobe Launch para incluir el script Munchkin en sus páginas web. Obtenga la aplicación [aquí](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Vaya a **Administración** y haga clic en **Munchkin** en el árbol de la izquierda.

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   Seleccione Asincrónico para Tipo de código de seguimiento.

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >En casi todos los casos, debe utilizar el código asincrónico. [Más información.](#types-of-munchkin-tracking-codes)

   Haga clic y copie el código de seguimiento de Javascript para colocarlo en su sitio web.

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >No utilice el código que se muestra en esta captura de pantalla: debe utilizar el código único que aparece en la cuenta.

   >[!TIP]
   >
   >Coloque el código de seguimiento en las páginas Web que desee rastrear. Puede ser cada página para sitios más pequeños o sólo páginas clave en sitios que tengan muchas páginas Web generadas dinámicamente, foros de usuarios, etc.

   Para obtener los mejores resultados, utilice el código Munchkin asincrónico y colóquelo dentro de los elementos `<head>` de sus páginas. Si está utilizando el código simple (no recomendado), esto es justo antes de la etiqueta `</body>`.
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>Para los sitios que ven un gran volumen de tráfico (es decir, cientos de miles de visitas al mes), recomendamos que opte por no rastrear a personas anónimas. [Más información.](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)

## Añadir código de seguimiento al utilizar varias áreas de trabajo {#add-tracking-code-when-using-multiple-workspaces}

Si utiliza Workspaces en su cuenta de Marketing, probablemente también tenga presencias web independientes que se correspondan con sus espacios de trabajo. En ese caso, puede utilizar el Javascript de seguimiento de Munchkin para asignar a sus personas anónimas el espacio de trabajo y la partición correctos.

1. Vaya a Administración y haga clic en Munchkin en el árbol de la izquierda.

![](assets/image2015-8-25-16-3a28-3a41.png)

1. Seleccione el espacio de trabajo adecuado para las páginas Web que desee rastrear.

![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>Si no utiliza el código Munchkin del espacio de trabajo especial, las personas se asignarán a la partición predeterminada que se creó cuando se configuró su cuenta. Al principio se llama &quot;Predeterminado&quot;, pero es posible que lo haya cambiado en su propia cuenta de Marketing.

1. Seleccione Asincrónico para Tipo de código de seguimiento.

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. Haga clic y copie el código de seguimiento de JavaScript para colocarlo en el sitio web.

![](assets/image2015-8-25-16-3a34-3a7.png)

>[!CAUTION]
>
>No utilice el código que se muestra en esta captura de pantalla: debe utilizar el código único que aparece en la cuenta.

1. Coloque el código de seguimiento en las páginas Web en el elemento `<head>`. Las personas nuevas que visiten esta página se asignarán a esta partición.

![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>Sólo puede utilizar un script de seguimiento Munchkin para una sola partición y espacio de trabajo en una página. No incluya scripts de seguimiento para varias particiones o espacios de trabajo en el sitio web.

>[!NOTE]
>
>Las páginas de aterrizaje creadas en Marketing contienen automáticamente código de seguimiento, por lo que no es necesario que les ponga este código.

## Tipos de códigos de seguimiento de Munchkin {#types-of-munchkin-tracking-codes}

Hay 3 tipos de códigos de seguimiento Munchkin que puede elegir. Cada uno de ellos tiene un impacto diferente en el tiempo de carga de la página web.

1. **Simple**: tiene la menor cantidad de líneas de código, pero no se optimiza para el tiempo de carga de la página web. Este código carga la biblioteca jQuery cada vez que se carga una página web.
1. **Asincrónico**: reduce el tiempo de carga de la página web.
1. **jQuery** asincrónico: reduce el tiempo de carga de la página web y también mejora el rendimiento del sistema. Este código supone que ya tiene jQuery y no comprueba para cargarlo.

## Compruebe si el código Munchkin funciona {#test-if-your-munchkin-code-is-working}

Para comprobar que su código Munchkin está funcionando después de haberlo agregado:

1. Visite su página web.
1. Vaya a **Analytics**.

   ![](assets/mainnav-analytics-hand.png)

1. Haga clic en **Actividad de página Web**.

   ![](assets/webanalytics.png)

1. Haga clic en la ficha **Configuración**, haga clic con el doble **Origen de Actividad** y cámbielo a **Visitantes anónimos (incluidos los ISP)**.

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. Haga clic en la ficha **Informe**. Si no ve ningún dato, espere unos minutos y luego haga clic en el icono de actualización en la parte inferior.

