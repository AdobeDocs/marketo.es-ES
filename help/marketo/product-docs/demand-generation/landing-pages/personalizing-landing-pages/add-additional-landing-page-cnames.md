---
unique-page-id: 2359798
description: 'Agregar CNAME de página de aterrizaje adicionales: Documentos de Marketo: Documentación del producto'
title: Agregar CNAME de página de aterrizaje adicionales
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Agregar CNAME de página de aterrizaje adicionales {#add-additional-landing-page-cnames}

Puede que desee agregar CNAME de página de aterrizaje para permitir que distintas direcciones URL apunten a sus páginas de aterrizaje de Marketo. Los pasos siguientes le ayudarán a administrar varios dominios.

>[!CAUTION]
>
>Las cookies no se pueden compartir entre dominios.

>[!TIP]
>
>**El mismo dominio de nivel superior - ¡Bien! Las cookies se comparten**.<br/> **go**.mycompany.com > **información**.mycompany.com
>
>**Distintos dominios de nivel superior - Malos! Las cookies son _not_ shared**.<br/> vaya.**mycompany**.com > ir.**mynewcompany**.com

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Buscar la cadena de cuenta {#find-your-account-string}

1. Vaya a la **Administrador** área y haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copie el **Cadena de cuenta** de la variable **Configuración** para obtener más información.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anote para el paso siguiente.

## Enviar solicitud a TI {#send-request-to-it}

1. Pida a su departamento de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] con el CNAME de su elección y [CADENA DE CUENTA] con el texto del paso anterior).

   [CNAME].YourCompany.com > [CADENA DE CUENTA].mktoweb.com

## Añadir un nuevo CNAME {#add-a-new-cname}

1. Una vez que su departamento de TI haya creado el CNAME, vaya a **Administrador** a continuación, haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Haga clic en **Nuevo** a continuación, seleccione **Nuevo alias de dominio**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Escriba la **Alias de dominio.** La variable **Página predeterminada** se muestra si el visitante no introduce una dirección URL. Escriba a dónde deben ir en ese caso.

   >[!NOTE]
   >
   >Para la página predeterminada, puede seleccionar una página de aterrizaje o una dirección URL externa, como su sitio web público.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Escriba la **Página predeterminada** y haga clic en **Crear**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

¡Muy bien! Ahora sabe qué hacer si alguna vez desea agregar un CNAME.
