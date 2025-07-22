---
unique-page-id: 2359746
description: 'Personalización de las direcciones URL de su página de aterrizaje con un CNAME: documentos de Marketo: documentación del producto'
title: Personalización de las direcciones URL de su página de aterrizaje con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Personalización de las direcciones URL de su página de aterrizaje con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Aunque Marketo aloja sus páginas de aterrizaje, la dirección URL se puede personalizar completamente. Aspecto sin un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

El aspecto que debería tener:

`https://go.YourCompany.com/UnsubscribePage.html`

## Elija un CNAME {#choose-a-cname}

Elija una palabra para ir al principio de la dirección URL de sus páginas de aterrizaje. Es solo una palabra y debería ser relativamente corta. Ejemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

La única palabra (más YourCompany.com) se llama CNAME. Lo necesitarás más tarde, así que toma nota.

## Búsqueda de su Munchkin ID {#find-your-munchkin-id}

1. Vaya al área de **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Se requieren permisos de administración**

1. Desplácese hacia abajo hasta &quot;Información de asistencia&quot; y copie su Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Enviar solicitud a TI {#send-request-to-it}

Pida al personal de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] y [Munchkin ID] por el texto del paso anterior).

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Configuración completa de CNAME {#complete-cname-setup}

1. Una vez que el equipo de TI haya creado el CNAME, vaya al área de **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. En la sección **Configuración**, haga clic en **Editar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Escriba su CNAME en **[!UICONTROL Nombre de dominio para páginas de aterrizaje]**, ingrese su **[!UICONTROL página de reserva]**, ingrese su **[!UICONTROL página principal]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Su página de reserva será la página a la que se redirigirán los posibles clientes si la página de aterrizaje de Marketo no está disponible.

¡Buen trabajo! Las páginas de aterrizaje ahora están etiquetadas con el dominio de la compañía.
