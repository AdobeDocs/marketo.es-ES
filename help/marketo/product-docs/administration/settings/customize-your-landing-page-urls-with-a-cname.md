---
unique-page-id: 2360189
description: 'Personalización de las direcciones URL de su página de aterrizaje con un CNAME (administración): documentos de Marketo, documentación del producto'
title: Personalización de las direcciones URL de la página de aterrizaje con un CNAME (Administración)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Personalización de las direcciones URL de la página de aterrizaje con un CNAME  {#customize-your-landing-page-urls-with-a-cname}

Aunque Marketo aloja sus páginas de aterrizaje, la dirección URL debe personalizarse para su empresa.

>[!NOTE]
>
>No hay CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marca:
>
>https://go.**Su empresa**.com/UnsuscribePage.html

>[!NOTE]
>
>**Permisos de administración necesarios**

Lo ayudaremos a prepararse!

1. Elija un CNAME.

   Es la parte frontal de la URL. Ejemplos:

   * **ir**.YourCompany.com/NameOfPage.html
   * **información**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   La única palabra (más YourCompany.com) se llama CNAME. Lo necesitará más tarde, así que anótelo.

1. Busque la cadena de cuenta.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clic **[!UICONTROL Páginas de aterrizaje]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. En el **[!UICONTROL Páginas de aterrizaje]** pestaña, copie la cadena de cuenta de la sección Configuración.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. También lo necesitará más tarde, así que anótelo.

1. Enviar solicitud al departamento de TI.

1. Solicite a su personal de TI que configure el siguiente CNAME (sustituya la palabra [CNAME] y [CADENA DE CUENTA] con el texto del paso anterior):

   [CNAME].YourCompany.com > [CADENA DE CUENTA].mktoweb.com

1. Complete la configuración de CNAME.

1. Una vez que el equipo de TI haya creado el CNAME, vuelva a la **[!UICONTROL Administrador]** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clic **[!UICONTROL Páginas de aterrizaje]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. En el **[!UICONTROL Configuración]** , haga clic en **[!UICONTROL Editar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Introduzca su CNAME en **[!UICONTROL Nombre de dominio para páginas de aterrizaje]**, introduzca su **[!UICONTROL Página de reserva]**, introduzca su **[!UICONTROL Homepage]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

En la página de reserva se redirigirá a las personas si la página de aterrizaje de Marketo no está disponible.

¡Buen trabajo! Las páginas de aterrizaje ahora están etiquetadas con el dominio de la compañía.
