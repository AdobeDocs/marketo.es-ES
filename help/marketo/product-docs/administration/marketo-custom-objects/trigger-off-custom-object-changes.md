---
unique-page-id: 11378713
description: Cómo utilizar objetos personalizados para agregar o cambiar déclencheur en una lista inteligente de campañas inteligentes para objetos personalizados de Marketo, con pasos para agregar el déclencheur y establecer restricciones.
title: Desactivar cambios en objetos personalizables
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
TQID: 'https://experienceleague.adobe.com/KjZuM-gPLIFa1umPF4pzN2OTak51i9I5TUcC7SacmZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 8%
---
# Desactivar cambios en objetos personalizables {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Esta función solo está disponible:
>
>* Solo se puede usar con objetos personalizados de Marketo, no con objetos personalizados sincronizados mediante la integración nativa de [!DNL Salesforce] o [!DNL Microsoft Dynamics]
>
>* Como déclencheur, no como filtro
>
>Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para que se habiliten los Déclencheur de cambio de objeto personalizado.

En la lista inteligente de una campaña inteligente, puede almacenar en déclencheur una acción de flujo cuando se agrega un objeto personalizado a una persona o compañía. También puede crear una lista inteligente que use _change_ en un objeto personalizado como déclencheur. Por ejemplo, utilícelo para enviar un correo electrónico cuando se actualice un nombre de curso.

>[!NOTE]
>
>No se crea una entrada de registro de actividad cuando se cambia un registro de objeto personalizado.

1. En Marketo Engage, vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Cree o abra una campaña inteligente existente y seleccione la lista inteligente.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Busque el déclencheur que necesite y arrástrelo al lienzo.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Seleccione [!UICONTROL atributo de déclencheur].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Si lo desea, defina una restricción.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. El cambio se guarda automáticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
