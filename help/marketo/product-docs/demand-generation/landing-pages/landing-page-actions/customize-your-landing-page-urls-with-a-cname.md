---
unique-page-id: 2359746
description: Personalice las direcciones URL de su Página de aterrizaje con un CNAME - Documentos de marketing - Documentación del producto
title: Personalización de las direcciones URL de su Página de aterrizaje con un CNAME
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Personalización de las direcciones URL de su Página de aterrizaje con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Aunque Marketing aloja sus páginas de aterrizaje, la dirección URL puede personalizarse totalmente. Aspecto del producto sin un CNAME:
`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` El aspecto que debería tener:
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## Elija un CNAME {#choose-a-cname}

Elija una palabra para ir al principio de la dirección URL de sus páginas de aterrizaje. Es sólo una palabra y debería ser relativamente corta. Ejemplos:

* vaya. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* información. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* páginas. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

La única palabra (más [YourCompany.com](http://YourCompany.com)) se denomina CNAME. Necesitarás esto más tarde, así que haz una nota.

## Buscar la cadena de cuenta {#find-your-account-string}

1. Vaya al área **Administración** y haga clic en **Páginas de aterrizaje.**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Se requieren permisos de administración**

1. En la ficha **Páginas** de **aterrizaje** , copie la **cadena de cuenta****de la sección** Configuración **** .

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Necesitarás más tarde, así que haz una nota.

## Enviar solicitud al departamento de TI {#send-request-to-it}

Pida a su personal de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] y [ACCOUNT STRING] con el texto del paso anterior).

[CNAME]. [YourCompany.com](http://yourcompany.com/) > CADENA [DE CUENTA]. [mktoweb.com](http://mktoweb.com/)

## Configuración completa de CNAME {#complete-cname-setup}

1. Una vez que el departamento de TI haya creado el CNAME, vaya a **Administración** y haga clic en **Páginas de aterrizaje******.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. En la sección **Configuración** , haga clic en **Editar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Introduzca su CNAME en el **nombre** de **dominio** **para** las **páginas** de **aterrizaje****** ******** ****, introduzca suFallbackpage, introduzca suPágina de inicioy haga clic en Guardar.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>La página de reserva será la página a la que se redirigirán los leads si la Página de aterrizaje de marketing no está disponible.

¡Buen trabajo! Sus páginas de aterrizaje ahora están marcadas con su dominio de compañía.