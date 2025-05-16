---
unique-page-id: 2359828
description: 'Añadir SSL a las páginas de aterrizaje: documentación de Marketo'
title: Añadir SSL a las páginas de aterrizaje
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Añadir SSL a las páginas de aterrizaje {#add-ssl-to-your-landing-pages}

El cifrado SSL (Secure Socket Layer) permite que todas las páginas de destino de una instancia de Marketo Engage sean seguras.

Al rellenar un formulario web o visitar una página de aterrizaje alojada en Marketo Engage, la información se envía de forma predeterminada a través de un protocolo no seguro (HTTP). Según la política de su empresa, es posible que desee proteger la información enviada a Marketo a través de (HTTPS). Por ejemplo, cuando visite `http://info.mydomain.com/`, ahora será `https://info.mydomain.com/`.

Marketo Engage realiza un seguimiento predeterminado de &quot;Página web visitada&quot; y &quot;Haga clic en el vínculo de la página web&quot; a través del protocolo HTTP no seguro. Si desea que los vínculos de seguimiento estén protegidos con su propio certificado, debe hacer que Marketo cree un servidor no compartido independiente para habilitarlo. Proteger todos los aspectos de la interacción de un contacto con usted suele significar proteger tanto las páginas de aterrizaje como los vínculos de seguimiento.

## Habilitar la certificación SSL {#enable-ssl-certification}

Agregue automáticamente SSL para todos los alias de dominio que cree como parte de las reglas de la página de aterrizaje.

1. Vaya al área de **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Seleccione **Páginas de aterrizaje** del árbol. En la ficha **Reglas**, haga clic en la lista desplegable **Nuevo** y seleccione **Nuevo alias de dominio**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Escriba su _alias de dominio_ y _página predeterminada_. Seleccione la casilla de verificación **Generar certificado SSL**. Haga clic en **Crear** cuando haya terminado.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Esto agrega automáticamente un certificado SSL para este dominio.

## Habilite SSL para su dominio predeterminado {#enable-ssl-default-domain}

Siga los pasos a continuación para habilitar SSL para su dominio predeterminado.

1. En la sección **Admin**, seleccione **Páginas de aterrizaje**. Haga clic en el botón **Editar** naranja que está junto a _Configuración_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Si lo desea, también puede modificar el nombre de dominio aquí (se requiere un dominio válido).

1. Seleccione la casilla de verificación &quot;Generar certificado SSL&quot; y haga clic en Guardar.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* La columna Certificado SSL de la lista muestra el estado del certificado para todos los alias de dominio creados después de liberar esta función (FECHA). Si ha habilitado SSL para un dominio mediante el Soporte técnico de Marketo, el certificado seguirá existiendo, pero no se mostrará en la tabla. Esta tabla solo refleja los certificados SSL para los dominios agregados mediante los pasos de este artículo.
>
>* SSL puede tardar hasta tres minutos en estar en estado READY. Debe actualizar la página para que aparezcan los cambios.
