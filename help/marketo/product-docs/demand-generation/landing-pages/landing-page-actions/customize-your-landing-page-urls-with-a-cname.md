---
unique-page-id: 2359746
description: Personalización de las direcciones URL de su página de aterrizaje con un CNAME - Marketo Docs - Documentación del producto
title: Personalizar las direcciones URL de su página de aterrizaje con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Personalizar las direcciones URL de su página de aterrizaje con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Aunque Marketo aloje sus páginas de aterrizaje, la URL se puede personalizar completamente. Qué aspecto tiene sin un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

El aspecto que debería tener:

`https://go.YourCompany.com/UnsubscribePage.html`

## Elegir un CNAME {#choose-a-cname}

Elija una palabra para ir al principio de la dirección URL de las páginas de aterrizaje. Es solo una palabra y debería ser relativamente corto. Ejemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

La palabra (más YourCompany.com) se denomina CNAME. Necesitarás esto más tarde, así que ten en cuenta.

## Buscar la cadena de cuenta {#find-your-account-string}

1. Vaya a la **Administrador** área y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Se requieren permisos de administrador**

1. En el **Aterrizaje** **Páginas** , copie la **Cuenta** **Cadena** de la variable **Configuración** para obtener más información.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Necesitará más tarde, así que anónela.

## Enviar solicitud a TI {#send-request-to-it}

Pida a su personal de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] y [CADENA DE CUENTA] con el texto del paso anterior).

[CNAME].YourCompany.com > [CADENA DE CUENTA].mktoweb.com

## Configuración completa de CNAME {#complete-cname-setup}

1. Una vez que su TI haya creado el CNAME, vaya a **Administrador** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. En el **Configuración** , haga clic en **Editar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Escriba su CNAME en **Nombre de dominio de las páginas de aterrizaje**, introduzca el **Página de reserva**, introduzca el **Página principal** y haga clic en **Guardar**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>La página de reserva será la página a la que se redirigirán los posibles clientes si la página de aterrizaje de Marketo no está disponible.

¡Buen trabajo! Las páginas de aterrizaje ahora tienen marca con el dominio de la empresa.
