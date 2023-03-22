---
unique-page-id: 2359798
description: 'Agregar CNAME de página de aterrizaje adicionales: Documentos de Marketo: Documentación del producto'
title: Agregar CNAME de página de aterrizaje adicionales
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
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

1. Vaya a la **Administrador** .

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Desplácese hacia abajo hasta &quot;Información de soporte&quot; y copie su ID de Munchkin.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Enviar solicitud a TI {#send-request-to-it}

1. Pida a su departamento de TI que configure el siguiente CNAME: (Reemplace la palabra [CNAME] con el CNAME de su elección y [Munchkin ID] con el texto del paso anterior).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Añadir un nuevo CNAME {#add-a-new-cname}

1. Una vez que su departamento de TI haya creado el CNAME, vaya a la **Administrador** .

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Haga clic en **Nuevo** a continuación, seleccione **Nuevo alias de dominio**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Escriba la **Alias de dominio.** La variable **Página predeterminada** se muestra si el visitante no introduce una dirección URL. Escriba a dónde deben ir en ese caso.

   >[!NOTE]
   >
   >Para la página predeterminada, puede seleccionar una página de aterrizaje o una dirección URL externa, como su sitio web público.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Escriba la **Página predeterminada** y haga clic en **Crear**.

   ![](assets/add-additional-landing-page-cnames-8.png)

¡Muy bien! Ahora sabe qué hacer si alguna vez desea agregar un CNAME.
