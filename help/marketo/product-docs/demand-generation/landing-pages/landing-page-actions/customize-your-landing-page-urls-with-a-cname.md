---
unique-page-id: 2359746
description: Personalice las direcciones URL de su Página de aterrizaje con un CNAME - Documentos de marketing - Documentación del producto
title: Personalización de las direcciones URL de su Página de aterrizaje con un CNAME
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Personalice las direcciones URL de su Página de aterrizaje con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Aunque Marketing aloja sus páginas de aterrizaje, la dirección URL puede personalizarse totalmente. Aspecto del producto sin un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

El aspecto que debería tener:

`https://go.YourCompany.com/UnsubscribePage.html`

## Elija un CNAME {#choose-a-cname}

Elija una palabra para ir al principio de la dirección URL de sus páginas de aterrizaje. Es sólo una palabra y debería ser relativamente corta. Ejemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

La única palabra (más YourCompany.com) se denomina CNAME. Necesitarás esto más tarde, así que haz una nota.

## Buscar la cadena de cuenta {#find-your-account-string}

1. Vaya al área **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Se requieren permisos de administración**

1. En la ficha **Aterrizaje** **Páginas**, copie la **Cuenta** **Cadena** de la sección **Configuración**.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Necesitarás más tarde, así que haz una nota.

## Enviar solicitud a TI {#send-request-to-it}

Pida a su personal de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] y [CADENA DE CUENTA] por el texto del paso anterior).

[CNAME].YourCompany.com >  [CADENA] DE CUENTA.mktoweb.com

## Configuración completa de CNAME {#complete-cname-setup}

1. Una vez que el departamento de TI haya creado el CNAME, vaya a **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. En la sección **Configuración**, haga clic en **Editar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Escriba su CNAME en **nombre de dominio para Páginas de aterrizaje**, escriba su **página de reserva**, escriba su **página de inicio** y haga clic en **Guardar**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>La página de reserva será la página a la que se redirigirán los leads si la Página de aterrizaje de marketing no está disponible.

¡Buen trabajo! Sus páginas de aterrizaje ahora están marcadas con su dominio de compañía.
