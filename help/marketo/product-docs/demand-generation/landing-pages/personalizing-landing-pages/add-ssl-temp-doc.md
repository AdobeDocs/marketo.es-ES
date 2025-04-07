---
description: 'Añadir SSL a las páginas de aterrizaje: documentación de Marketo'
title: Añadir SSL a las páginas de aterrizaje
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: f41d0595db695fc485a209aa2f9646a76e57acdf
workflow-type: tm+mt
source-wordcount: '199'
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

Nota:

La columna Certificado SSL de la lista mostrará el estado del certificado SSL para todos los alias de dominio creados después de liberar esta función. Si tiene SSL habilitado para un dominio mediante soporte, el certificado SSL respectivo seguirá existiendo, pero esta tabla solo refleja los certificados SSL para el dominio agregado con esta función

SSL puede tardar hasta 3 minutos en estar en estado READY y es necesario actualizar la página para que los cambios se propaguen en la interfaz de usuario.
