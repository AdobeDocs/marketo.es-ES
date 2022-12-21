---
unique-page-id: 2360189
description: 'Personalización de las direcciones URL de su página de aterrizaje con un CNAME (administración): documentos de Marketo: documentación del producto'
title: Personalizar las direcciones URL de las páginas de aterrizaje con un CNAME (administración)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Personalizar las direcciones URL de las páginas de aterrizaje con un CNAME (administración) {#customize-your-landing-page-urls-with-a-cname-administration}

Aunque Marketo aloje sus páginas de aterrizaje, la dirección URL debe personalizarse para su empresa.

>[!NOTE]
>
>Sin CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marca:
>
>https://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Se requieren permisos de administrador**

¡Vamos a ponerte en marcha!

1. Elija un CNAME.

   Es la parte frontal de la URL. Ejemplos:

   * **go**.YourCompany.com/NameOfPage.html
   * **información**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   La palabra (más YourCompany.com) se denomina CNAME. Necesitará esto más tarde, así que tenga en cuenta.

1. Busque la cadena de cuenta.

1. Vaya a la **Administrador** área y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. En el **Páginas de aterrizaje** , copie la cadena de cuenta en la sección Configuración .

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. También lo necesitará más tarde, así que tenga en cuenta.

1. Envíe la solicitud a TI.

1. Pida a su personal de TI que configure el siguiente CNAME (reemplace la palabra [CNAME] y [CADENA DE CUENTA] con el texto del paso anterior):

   [CNAME].YourCompany.com > [CADENA DE CUENTA].mktoweb.com

1. Completar la configuración de CNAME.

1. Una vez que su TI haya creado el CNAME, vaya a **Administrador** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. En el **Configuración** , haga clic en **Editar**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Escriba su CNAME en **Nombre de dominio de las páginas de aterrizaje**, introduzca el **Página de reserva**, introduzca el **Página principal** y haga clic en **Guardar**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

En la página de reserva se redirigirá a las personas si la página de aterrizaje de Marketo no está disponible.

¡Buen trabajo! Las páginas de aterrizaje ahora tienen marca con el dominio de la empresa.
