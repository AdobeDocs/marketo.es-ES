---
unique-page-id: 1900589
description: Aprenda a añadir vínculos rastreados a correos electrónicos de solo texto. Habilite el seguimiento de vínculos para poder medir los clics en los informes de correo electrónico.
title: Añadir vínculos rastreados a un correo electrónico de texto
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/zz5DkOWG-x3y-oq-E77xRAZtcNdmimbwKsctKSChnXM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 7%
---
# Añadir vínculos rastreados a un correo electrónico de texto {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Crear un correo electrónico de solo texto](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Editar elementos en un mensaje de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

Los vínculos de correo electrónico de texto se pueden rastrear en Marketo. Vamos a ver cómo funciona.

1. Seleccione su correo electrónico y haga clic en **Editar borrador**.

1. Seleccione su correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/one-9.png)

1. Haga doble clic en el área editable a la que desee agregar el vínculo.

   ![](assets/two-8.png)

1. Escriba la dirección URL entre corchetes, de la siguiente manera: `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Si un mensaje de correo electrónico se envió hace más de 365 días **y** nadie ha hecho clic en ninguno de sus vínculos en los últimos 180 días, Marketo Engage elimina la ruta a la dirección URL de nuestra base de datos, lo que provocará que se rompa el vínculo. Si necesita que el vínculo sea permanente, no utilice el seguimiento.

1. Cierre el editor y no se olvide de aprobar el borrador.

   ![](assets/four-6.png)

>[!NOTE]
>
>La funcionalidad de la clase mktNoTok no funciona con vínculos a los que se puede realizar un seguimiento en correos electrónicos de texto. Solo para correos electrónicos de HTML.
