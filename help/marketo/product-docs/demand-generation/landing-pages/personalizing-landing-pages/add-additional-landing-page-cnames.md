---
unique-page-id: 2359798
description: 'Añadir CNAME de página de aterrizaje adicional: documentos de Marketo, documentación del producto'
title: Añadir CNAME de página de aterrizaje adicional
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Añadir CNAME de página de aterrizaje adicional {#add-additional-landing-page-cnames}

Es posible que desee añadir CNAME de página de aterrizaje para permitir que distintas URL apunten a sus páginas de aterrizaje de Marketo. Seguir los pasos a continuación le ayudará a administrar varios dominios.

>[!CAUTION]
>
>Las cookies no se pueden compartir entre dominios.

>[!TIP]
>
>**Mismo dominio de nivel superior - ¡Bien! Se comparten las cookies**.<br/> **ir**.mycompany.com > **información**.mycompany.com
>
>**Diferentes dominios de nivel superior - ¡Malo! Las cookies _no_ se han compartido**.<br/> ir.**mycompany**.com > ir.**mynewcompany**.com

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Desplácese hacia abajo hasta &quot;Información de asistencia&quot; y copie su ID de Munchkin.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Enviar solicitud a TI {#send-request-to-it}

1. Pida al departamento de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] por el CNAME de su elección y [Munchkin ID] por el texto del paso anterior).

   [CNAME].YourCompany.com > [ID de Munchkin].mktoweb.com

## Añadir un nuevo CNAME {#add-a-new-cname}

1. Una vez que el departamento de TI haya creado el CNAME, vaya al área de **Admin**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Haga clic en **Nuevo** y, a continuación, seleccione **Nuevo alias de dominio**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Escriba su alias de dominio **.**: se muestra la **página predeterminada** si el visitante no escribe una dirección URL. Introduzca a dónde deben ir en ese caso.

   >[!NOTE]
   >
   >Para la página predeterminada, puede seleccionar una página de aterrizaje o una URL externa, como un sitio web público.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Escriba su **página predeterminada** y haga clic en **Crear**.

   ![](assets/add-additional-landing-page-cnames-8.png)

¡Bonito! Ahora sabe qué hacer si alguna vez desea agregar un CNAME.
