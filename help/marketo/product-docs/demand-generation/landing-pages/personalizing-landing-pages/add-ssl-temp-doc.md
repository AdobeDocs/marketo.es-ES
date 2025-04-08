---
description: 'Añadir SSL a las páginas de aterrizaje: documentación de Marketo'
title: Añadir SSL a las páginas de aterrizaje
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Añadir SSL a las páginas de aterrizaje {#add-ssl-to-your-landing-pages}

Aprenda a agregar el alias de su dominio de marca (por ejemplo, `http://business.adobe.com`) a las páginas de aterrizaje creadas en Marketo Engage para que se pueda acceder a ellas desde sus dominios de marca.

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

## Habilite SSL para su dominio predeterminado

CAPTURA DE PANTALLA

>[!NOTE]
>
>* La columna Certificado SSL de la lista muestra el estado del certificado para todos los alias de dominio creados después de liberar esta función (FECHA). Si ha habilitado SSL para un dominio mediante el Soporte técnico de Marketo, el certificado seguirá existiendo, pero no se mostrará en la tabla. Esta tabla solo refleja los certificados SSL para los dominios agregados mediante los pasos de este artículo.
>
>* SSL puede tardar hasta tres minutos en estar en estado READY. Debe actualizar la página para que aparezcan los cambios.
