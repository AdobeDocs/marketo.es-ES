---
unique-page-id: 2359746
description: Personalización de las direcciones URL de su página de aterrizaje con un CNAME - Marketo Docs - Documentación del producto
title: Personalizar las direcciones URL de su página de aterrizaje con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
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

## Encuentre su ID de Munchkin {#find-your-munchkin-id}

1. Vaya a la **Administrador** .

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Se requieren permisos de administrador**

1. Desplácese hacia abajo hasta &quot;Información de soporte&quot; y copie su ID de Munchkin.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Enviar solicitud a TI {#send-request-to-it}

Pida a su personal de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] y [Munchkin ID] con el texto del paso anterior).

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Configuración completa de CNAME {#complete-cname-setup}

1. Una vez que su TI haya creado el CNAME, vaya a la **Administrador** .

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. En el **Configuración** , haga clic en **Editar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Escriba su CNAME en **Nombre de dominio de las páginas de aterrizaje**, introduzca el **Página de reserva**, introduzca el **Página principal** y haga clic en **Guardar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>La página de reserva será la página a la que se redirigirán los posibles clientes si la página de aterrizaje de Marketo no está disponible.

¡Buen trabajo! Las páginas de aterrizaje ahora tienen marca con el dominio de la empresa.
