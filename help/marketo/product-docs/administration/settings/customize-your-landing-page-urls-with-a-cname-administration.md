---
unique-page-id: 2360189
description: Personalización de las direcciones URL de su Página de aterrizaje con un CNAME (administración) - Documentos de marketing - Documentación del producto
title: Personalización de las direcciones URL de su Página de aterrizaje con un CNAME (administración)
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Personalización de las direcciones URL de su Página de aterrizaje con un CNAME (administración) {#customize-your-landing-page-urls-with-a-cname-administration}

Aunque Marketing aloja sus páginas de aterrizaje, la dirección URL debe personalizarse para su compañía.

>[!NOTE]
>
>**Ejemplo**
>
>Sin CNAME:
>
>http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marca:
>
>http://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Se requieren permisos de administración**

¡Vamos a ponerte en marcha!

1. Elija un CNAME

   Es la parte frontal de la dirección URL. Ejemplos:

   * **vaya**.YourCompany.com/NameOfPage.html
   * **información**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.htmlás

   La única palabra (más YourCompany.com) se denomina CNAME. Necesitarás esto más tarde, así que haz una nota.

1. Buscar la cadena de cuenta
1. Vaya al área **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. En la ficha **Páginas de aterrizaje **, copie la cadena de cuenta de la sección Configuración.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. También necesitarás esto más tarde, así que ten en cuenta.
1. Enviar solicitud al departamento de TI
1. Pida a su personal de TI que configure el siguiente CNAME (reemplace la palabra [CNAME] y [ACCOUNT STRING] por el texto del paso anterior):

   [CNAME].YourCompany.com > [CADENA]DE CUENTA.mktoweb.com

1. Configuración completa de CNAME
1. Una vez que el departamento de TI haya creado el CNAME, vaya a **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. En la sección **Configuración** , haga clic en **Editar**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Introduzca su CNAME en el nombre **de dominio para Páginas de aterrizaje**, introduzca su página **de** reserva, introduzca su **página de inicio** y haga clic en **Guardar**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

   La página de reserva es donde se redirigirá a las personas si la página de aterrizaje de marketing no está disponible.
¡Buen trabajo! Sus páginas de aterrizaje ahora están marcadas con su dominio de compañía.

