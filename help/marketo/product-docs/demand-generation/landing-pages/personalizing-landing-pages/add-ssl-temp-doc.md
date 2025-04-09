---
description: 'Añadir SSL a las páginas de aterrizaje: documentación de Marketo'
title: Añadir SSL a las páginas de aterrizaje
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Añadir SSL a las páginas de aterrizaje {#add-ssl-to-your-landing-pages}

El cifrado SSL (Secure Socket Layer) permite que todas las páginas de destino de una instancia de Marketo Engage sean seguras.

Cuando rellena un formulario web o visita una página de aterrizaje alojada en Marketo Engage, la información se envía de forma predeterminada a través de un protocolo no seguro (HTTP). Según la política de su empresa, es posible que desee proteger la información enviada a Marketo a través de (HTTPS). Por ejemplo, cuando visite `http://info.mydomain.com/`, ahora será `https://info.mydomain.com/`.

Marketo Engage realiza un seguimiento predeterminado de &quot;Página web visitada&quot; y &quot;Haga clic en el vínculo de la página web&quot; a través del protocolo HTTP no seguro. Si desea que los vínculos de seguimiento estén protegidos con su propio certificado, debe hacer que Marketo cree un servidor no compartido independiente para habilitarlo. Proteger todos los aspectos de la interacción de un contacto con usted suele significar proteger tanto las páginas de aterrizaje como los vínculos de seguimiento.

CAPTURA DE PANTALLA

## Habilitar la certificación SSL {#enable-ssl-certification}

Agregue automáticamente SSL para todos los alias de dominio que cree como parte de las reglas de la página de aterrizaje.

1. Vaya al área de **Admin**.

   CAPTURA DE PANTALLA

1. Seleccione **Páginas de aterrizaje** del árbol. En la ficha **Reglas**, haga clic en la lista desplegable **Nuevo** y seleccione **Nuevo alias de dominio**.

   CAPTURA DE PANTALLA

1. Seleccione la casilla de verificación **Generar certificado SSL**.

   CAPTURA DE PANTALLA

Esto agrega automáticamente un certificado SSL para este dominio.

CAPTURA DE PANTALLA

## Habilite SSL para su dominio predeterminado {#enable-ssl-default-domain}

CAPTURA DE PANTALLA

>[!NOTE]
>
>* La columna Certificado SSL de la lista muestra el estado del certificado para todos los alias de dominio creados después de liberar esta función (FECHA). Si ha habilitado SSL para un dominio mediante el Soporte técnico de Marketo, el certificado seguirá existiendo, pero no se mostrará en la tabla. Esta tabla solo refleja los certificados SSL para los dominios agregados mediante los pasos de este artículo.
>
>* SSL puede tardar hasta tres minutos en estar en estado READY. Debe actualizar la página para que aparezcan los cambios.
