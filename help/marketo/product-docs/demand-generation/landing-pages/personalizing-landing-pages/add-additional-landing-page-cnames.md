---
unique-page-id: 2359798
description: Añadir CNAME de Página de aterrizaje adicionales - Documentos de marketing - Documentación del producto
title: Añadir CNAME de Página de aterrizaje adicionales
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Añadir CNAME de Página de aterrizaje adicionales {#add-additional-landing-page-cnames}

Puede que desee agregar CNAME de página de aterrizaje para permitir que distintas direcciones URL señalen a sus páginas de aterrizaje de marketing. Si sigue los pasos a continuación, podrá administrar varios dominios.

>[!CAUTION]
>
>Las cookies no se pueden compartir entre dominios.

>[!TIP]
>
>**El mismo dominio de nivel superior - ¡Bien! Las cookies son shared.go**.mycompany.com > **info**.mycompany.**comDominios de nivel superior diferentes - ¡Malos! Las cookies no se comparten.**
>vaya.**miempresa**.com > ir.**mynewcompany**.com

>[!NOTE]
>
>**Se requieren permisos de administración**

## Buscar la cadena de cuenta {#find-your-account-string}

1. Vaya al área **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copie la cadena **de** cuenta de la sección **Configuración** .

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anote esto para el paso siguiente.

## Enviar solicitud al departamento de TI {#send-request-to-it}

1. Pida a su departamento de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] por el CNAME de su elección y [ACCOUNT STRING] por el texto del paso anterior).

   [CNAME].YourCompany.com > [CADENA]DE CUENTA.mktoweb.com

## Añadir un nuevo CNAME {#add-a-new-cname}

1. Una vez que el departamento de TI haya creado el CNAME, vaya a **Administración** y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Haga clic en **Nuevo** y, a continuación, seleccione **Nuevo alias** de dominio.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Introduzca el alias **de dominio.** La página **** predeterminada se muestra si el visitante no incluye una dirección URL. Ingrese adónde deben ir en ese caso.

   >[!NOTE]
   >
   >Para la página predeterminada, puede seleccionar una página de aterrizaje o una dirección URL externa, como el sitio web público.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Introduzca la página **** predeterminada y haga clic en **Crear**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

¡Bonito! Ahora sabe qué hacer si alguna vez desea agregar un CNAME.
