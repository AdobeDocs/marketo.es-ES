---
unique-page-id: 2359798
description: Aprenda a añadir CNAME de página de aterrizaje adicionales en Marketo. Utilice varios dominios personalizados para las páginas de aterrizaje.
title: Añadir CNAME de página de destino adicional
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
TQID: https://experienceleague.adobe.com/IhpbLwq0syIQpnKsRApy6YtEKhe56dbDciW8lSYJ9tI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 6%

---

# Añadir CNAME de página de destino adicional {#add-additional-landing-page-cnames}

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
>**Se requieren permisos de administrador**

1. Vaya al área de **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Desplácese hacia abajo hasta &quot;Información de asistencia&quot; y copie su Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Enviar solicitud a TI {#send-request-to-it}

1. Pida al departamento de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] por el CNAME de su elección y [Munchkin ID] por el texto del paso anterior).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Añadir un nuevo CNAME {#add-a-new-cname}

1. Una vez que el departamento de TI haya creado el CNAME, vaya al área de **Admin**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Haga clic en **[!UICONTROL Nuevo]** y, a continuación, seleccione **[!UICONTROL Nuevo alias de dominio]**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Escriba su **[!UICONTROL alias de dominio].** **[!UICONTROL Página predeterminada]** se muestra si el visitante no escribe una dirección URL. Introduzca a dónde deben ir en ese caso.

   >[!NOTE]
   >
   >Para la [!UICONTROL página predeterminada], puede seleccionar una página de aterrizaje o una dirección URL externa, como un sitio web público.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Escriba su **[!UICONTROL página predeterminada]** y haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

¡Bonito! Ahora sabe qué hacer si alguna vez desea agregar un CNAME.
